# File-System
This project implements a file system within a 128 KB file which acts as the "disk" for the system. To create a disk, run 
create_fs <diskname>. The functions for the file system are in fs.cpp. The first block in the system is the super block,
which stores the free block list and index nodes for each file. There are 16 inodes which allows for 16 files on the 
system. The functions I implemented were create_file() which creates a new file in the system if enough space is
available, delete_file() which deletes a specified file, read() which reads data from a block into a buffer, write()
which writes data from a buffer into a block, ls() which lists all files and their sizes in the system, and close_disk()
which closes the disk file. The main file reads in a txt file that names the disk and lists actions to be performed on
the disk.
