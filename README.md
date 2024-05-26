File Packer Unpacker 

- This project is used to perform packing and unpacking activity for multiple types of files.

- In case of Packing activity me maintain one file which contains metadata and data of multiple files from specified directory.

- In case of Unpacking activity we extract all data from packed files and according to its metadata we create all files.


  Packing Activity :

  •In case of Packing activity we accept directory name and file name from user. 
  •We have to create new regular file as the name specified by the user. 
  •Now open the directory and traverse each file from that directory. In newly created file write Metadata as header and actual file data in sequence.
  •While writing data perform encryption.
  •Each name of file ,its size and checksum should be written in log file which gets created in system directory. 
  •After packing display packing report.

  UnPacking Activity :

  •In case of UnPacking activity we accept packed file name from user. 
  •for authentication of packed file use any logic like Magic Number. 
  •Open the packed file in read mode and perform below activity as 
    •Read header 
    •From the name specified in header create new file. 
    •Write data into newly created file from packed file. 
  •After unpacking display unpacking report.
