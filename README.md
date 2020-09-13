# disk_mem-management
The program sets a platphorm simulating the managment of the disk by the operating system. 
The disk managment means accessing to files, storing their content and executing action on them such as writing, reading, deleting etc.
Each file stored on the disk, is stored in small "units" called blocks - the sizes of these blocks and the disk are changing from one system to another.
That managment system from that type is called UNIX-fs, there are direct blocks to store the data of the file and one more single indirect block which holds (if needed) more block size optional blocks for storage.
On this simulation, we consider the OS to hold one directory and max size of the disk of 256 bits.
In case the input is illegal or there is an error (not executable, or no such command), the cause for the error will show on the screen and the action won't be executed.

The user's input is a number according to the command he wishes to make. The possible commands are:
0 - delete the disk and exit.
1 - print the whole content of the disk.
      A list of the files, their fd and their status (open/closed) will show on screen.
2 - format the disk. After this action the user should enter number of direct blocks and block size.
      amount of free blocks (at this point) will show on screen.
3 - create a new file. The user should enter the name of the file.
      The file's file descriptor will show.
4 - open a file. The user should enter the file's name.
       The file's file descriptor will show.
5 - close a file. The user should enter the file's name.
      The file's file descriptor will show.
6 - write to a file. The user should enter the file's file descriptor, a string he wishes to write and its length.
7 - read from a file. The user should enter the file's file descriptor and how many characters he wants to read from the file.
      What was read from the file will show on screen.
8 - delete a file. The user should enter the file's name.
