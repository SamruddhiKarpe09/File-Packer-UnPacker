# File-Packer-UnPacker

 In this project we have use Java as Front end as well as Backend for platform independency.

# Front end

1. We have create one window which accept username and password from user for authentication purpose.
2. When user Submit the username and  password we have to check whether user is "MarvellousAdmin" and password is "MarvellousAdmin". 
3. After successful authentication we have to open new window which displays two option as Pack and Unpack.
4. When user press Pack button a new window is opened. From this newly opened window we have to accept name of directory that we want to pack and name of the packed file from user.
5. Name of the packed file gets newly created which contains data and metadata of all file from that directory.
6. When user click submit button we have to perform "Packing Activity". After that previous window shouls be displayed.
7. When user click Unpack button a new window is diplayed. from this window accept name of packed file
8. When user click Extract button we have to [erform " Unpacking Activity".  




#Backend Logic

# Packing Acitivity:
 In case of packing activity we accept directory name and file name from user
 We have to create new regular file as the name specified by the user.
 Now open the directory and traverse each file from that directory . In newly created file write Metadata as header and actual file data in sequence.
 While writing the data perform encryption.
 Each name of file , its size and checksum should be written in log file which gets created in system directory.
 After packing display packing report.

# Unpacking Activity:
 In case of UnPacking activity we accept packed file name from user
 For authentication of packed file use any logic like Magic Numbers
 Open the Packed file in read mode and perform below activity as Read Header, from the name specifies in the header create new file, Write data into newly created file from packed file, Repeat all above steps till we reach at end of the file unpacked file.
 After unpacking display unpacking report.
