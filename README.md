# Windows-Commands
***40 essential Windows commands***

*The Windows command line is one of the most powerful utilities on a Windows PC. With it, we can interact with the OS directly and do a lot of things not available in the graphical user interface (GUI).*

__Basic File and Directory Navigation:__

- **dir**: Lists the files and directories in the current directory.

```
C:\Users\dassu\windowsCommands>dir
 Volume in drive C has no label.
 Volume Serial Number is 5633-654B

 Directory of C:\Users\dassu\windowsCommands

14-04-2024  06:58 PM    <DIR>          .
14-04-2024  06:54 PM    <DIR>          ..
14-04-2024  06:57 PM                13 test1.txt
14-04-2024  06:58 PM                13 test2.txt
14-04-2024  06:58 PM                13 test3.txt
               3 File(s)             39 bytes
               2 Dir(s)  108,630,683,648 bytes free
```

- **cd**: Changes the current directory.

Example: cd Documents (changes to the Documents directory)
```
 Directory of C:\Users\dassu\windowsCommands

14-04-2024  07:03 PM    <DIR>          .
14-04-2024  06:54 PM    <DIR>          ..
14-04-2024  06:57 PM                13 test1.txt
14-04-2024  06:58 PM                13 test2.txt
14-04-2024  06:58 PM                13 test3.txt
14-04-2024  07:03 PM    <DIR>          testFolder
               3 File(s)             39 bytes
               3 Dir(s)  108,629,594,112 bytes free

C:\Users\dassu\windowsCommands>cd testFolder

C:\Users\dassu\windowsCommands\testFolder>

C:\Users\dassu\windowsCommands\testFolder>cd ..

C:\Users\dassu\windowsCommands>
```

- **mkdir**: Creates a new directory.

Example: mkdir NewFolder (creates a new folder named "NewFolder")
```
C:\Users\dassu\windowsCommands\testFolder>mkdir NewFolder

C:\Users\dassu\windowsCommands\testFolder>dir
 Volume in drive C has no label.
 Volume Serial Number is 5633-654B

 Directory of C:\Users\dassu\windowsCommands\testFolder

14-04-2024  07:08 PM    <DIR>          .
14-04-2024  07:03 PM    <DIR>          ..
14-04-2024  07:08 PM    <DIR>          NewFolder
               0 File(s)              0 bytes
               3 Dir(s)  108,627,693,568 bytes free
```

- **rmdir**: Removes a directory.

Example: rmdir OldFolder (removes the folder named "OldFolder")
```
C:\Users\dassu\windowsCommands\testFolder>rmdir NewFolder

C:\Users\dassu\windowsCommands\testFolder>dir
 Volume in drive C has no label.
 Volume Serial Number is 5633-654B

 Directory of C:\Users\dassu\windowsCommands\testFolder

14-04-2024  07:18 PM    <DIR>          .
14-04-2024  07:03 PM    <DIR>          ..
               0 File(s)              0 bytes
               2 Dir(s)  108,617,166,848 bytes free
```

- **del**: Deletes one or more files.

Example: del file.txt (deletes a file named "file.txt")
```
 Directory of C:\Users\dassu\windowsCommands

14-04-2024  07:03 PM    <DIR>          .
14-04-2024  06:54 PM    <DIR>          ..
14-04-2024  06:57 PM                13 test1.txt
14-04-2024  06:58 PM                13 test2.txt
14-04-2024  06:58 PM                13 test3.txt
14-04-2024  07:18 PM    <DIR>          testFolder
               3 File(s)             39 bytes
               3 Dir(s)  108,616,282,112 bytes free

C:\Users\dassu\windowsCommands>del test1.txt

C:\Users\dassu\windowsCommands>dir
 Volume in drive C has no label.
 Volume Serial Number is 5633-654B

 Directory of C:\Users\dassu\windowsCommands

14-04-2024  07:22 PM    <DIR>          .
14-04-2024  06:54 PM    <DIR>          ..
14-04-2024  06:58 PM                13 test2.txt
14-04-2024  06:58 PM                13 test3.txt
14-04-2024  07:18 PM    <DIR>          testFolder
               2 File(s)             26 bytes
               3 Dir(s)  108,616,282,112 bytes free
```

- **copy**: Copies one or more files from one location to another.

Example: copy file1.txt C:\DestinationFolder (copies "file1.txt" to "DestinationFolder")

```
C:\Users\dassu\windowsCommands>copy test2.txt testFolder
        1 file(s) copied.

C:\Users\dassu\windowsCommands>cd testFolder

C:\Users\dassu\windowsCommands\testFolder>dir
 Volume in drive C has no label.
 Volume Serial Number is 5633-654B

 Directory of C:\Users\dassu\windowsCommands\testFolder

14-04-2024  07:28 PM    <DIR>          .
14-04-2024  07:22 PM    <DIR>          ..
14-04-2024  06:58 PM                13 test2.txt
               1 File(s)             13 bytes
               2 Dir(s)  108,623,585,280 bytes free
```

- **move**: Moves one or more files from one location to another.

Example: move file2.txt C:\NewLocation (moves "file2.txt" to "NewLocation")

```
C:\Users\dassu\windowsCommands>move test3.txt testFolder
        1 file(s) moved.

C:\Users\dassu\windowsCommands>dir
 Volume in drive C has no label.
 Volume Serial Number is 5633-654B

 Directory of C:\Users\dassu\windowsCommands

14-04-2024  07:33 PM    <DIR>          .
14-04-2024  06:54 PM    <DIR>          ..
14-04-2024  06:58 PM                13 test2.txt
14-04-2024  07:33 PM    <DIR>          testFolder
               1 File(s)             13 bytes
               3 Dir(s)  108,623,994,880 bytes free

C:\Users\dassu\windowsCommands>cd testFolder

C:\Users\dassu\windowsCommands\testFolder>dir
 Volume in drive C has no label.
 Volume Serial Number is 5633-654B

 Directory of C:\Users\dassu\windowsCommands\testFolder

14-04-2024  07:33 PM    <DIR>          .
14-04-2024  07:33 PM    <DIR>          ..
14-04-2024  06:58 PM                13 test2.txt
14-04-2024  06:58 PM                13 test3.txt
               2 File(s)             26 bytes
               2 Dir(s)  108,623,994,880 bytes free
```

- **ren**: Renames a file or directory.

Example: ren oldname.txt newname.txt (renames "oldname.txt" to "newname.txt")

```
 Directory of C:\Users\dassu\windowsCommands

14-04-2024  07:33 PM    <DIR>          .
14-04-2024  06:54 PM    <DIR>          ..
14-04-2024  06:58 PM                13 test2.txt
14-04-2024  07:33 PM    <DIR>          testFolder
               1 File(s)             13 bytes
               3 Dir(s)  108,623,339,520 bytes free

C:\Users\dassu\windowsCommands>ren test2.txt newNamedFile.txt

C:\Users\dassu\windowsCommands>dir
 Volume in drive C has no label.
 Volume Serial Number is 5633-654B

 Directory of C:\Users\dassu\windowsCommands

14-04-2024  07:35 PM    <DIR>          .
14-04-2024  06:54 PM    <DIR>          ..
14-04-2024  06:58 PM                13 newNamedFile.txt
14-04-2024  07:33 PM    <DIR>          testFolder
               1 File(s)             13 bytes
               3 Dir(s)  108,623,204,352 bytes free
```

