# File-Packer-UnPacker

# Packing Acitivity:
# In case of packing activity we accept directory name and file name from user
# We have to create new regular file as the name specified by the user.
# Now open the directory and traverse each file from that directory . In newly created file write Metadata as header and actual file data in sequence.
# While writing the data perform encryption.
# Each name of file , its size and checksum should be written in log file which gets created in system directory.
# After packing display packing report.

# Unpacking Activity:
# In case of UnPacking activity we accept packed file name from user
# For authentication of packed file use any logic like Magic Numbers
# Open the Packed file in read mode and perform below activity as Read Header, from the name specifies in the header create new file, Write data into newly created file from packed file, Repeat all above steps till we reach at end of the file unpacked file.
# After unpacking display unpacking report.
