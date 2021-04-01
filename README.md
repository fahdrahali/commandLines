<div align="center">
  <h1>Basic Command Lines</h1>
</div>


  - [Basic Command Lines](#basic-command-lines)
    - [Current working directory](#current-working-directory)
    - [Navigating directory](#navigating-directory)
    - [Making Directory](#making-directory)
    - [List files and directories](#list-files-and-directories)
    - [Detail list](#detail-list)
    - [Creating file](#creating-file)
    - [Opening and writing on file](#opening-and-writing-on-file)
    - [Opening file to read](#opening-file-to-read)
    - [Copy file](#copy-file)
    - [Rename file](#rename-file)
    - [Moving file and directory](#moving-file-and-directory)
    - [Delete file and directory](#delete-file-and-directory)



## Basic Command Lines


### Current working directory

Checking the working directory using the command _pwd_.

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~$ pwd
/home/exploitation
```

### Navigating directory

Now, let's go to the Desktop using cd(change directory).

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~$ cd Desktop
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop$
```

To check where you are at, use the _pwd_ command age

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop$ pwd
/home/exploitation/Desktop
```

We use _cd_ to get into a directory(folder) and we use _cd.._ to get out from a directory, in other words, we use _cd_ to go forward into a directory and _cd .._ to go backward from a directory.

### Making Directory

Now, let's create a directory inside the Desktop. Call the name of the directory, 10-days-of-code. You give it any name but I am in favor of this name.
Use the _mkdir_ command to make a directory(folder)

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop$ mkdir 10-days-of-code
```

Now let's go to the 10-days-of-code folder using _cd_ command.

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop$ cd 10-days-of-code
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ pwd
/home/exploitation/Desktop/10-days-of-code
```

### List files and directories

We can check the files and directories we have in a directory(folder) using the _ls_ command.

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ ls
```

No files or directories were found in the 10-days-of-code folder because we didn't create them yet. Let's create some directories

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ mkdir day-1
```

Now let's check if there are some files or directories in the 10-days-of-code folder.

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ ls
day-1
```

Now, you see a day-1 folder that you created.

Now let's create multiple folders at one and use _ls_ to see all the directories we have in the 10-days-of-code folder.

Making multiple folders at once

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ mkdir day-2 day-3 day-4 day-5 day-6 day-7 day-8 day-9 day-10
```

Using _ls_ we can see all the directories we have in the 10-days-of-code

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code
$ ls
day-1  day-10  day-2  day-3  day-4  day-5  day-6  day-7  day-8  day-9
```

### Detail list

Let's see a detailed list of the directories using multiple commands, _ls -la_.

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code
$ ls -la
total 20
drwxr-xr-x 1 exploitation 197121 0 Jan 19 02:16 .
drwxr-xr-x 1 exploitation 197121 0 Jan 19 02:05 ..
drwxr-xr-x 1 exploitation 197121 0 Jan 19 02:12 day-1
drwxr-xr-x 1 exploitation 197121 0 Jan 19 02:16 day-10
drwxr-xr-x 1 exploitation 197121 0 Jan 19 02:16 day-2
drwxr-xr-x 1 exploitation 197121 0 Jan 19 02:16 day-3
drwxr-xr-x 1 exploitation 197121 0 Jan 19 02:16 day-4
drwxr-xr-x 1 exploitation 197121 0 Jan 19 02:16 day-5
drwxr-xr-x 1 exploitation 197121 0 Jan 19 02:16 day-6
drwxr-xr-x 1 exploitation 197121 0 Jan 19 02:16 day-7
drwxr-xr-x 1 exploitation 197121 0 Jan 19 02:16 day-8
drwxr-xr-x 1 exploitation 197121 0 Jan 19 02:16 day-9
```

Using the above command, we can see the detailed view of a directory or a file

### Creating file

Now, let's see how to create a file. We can use the _touch_ command to write a file.

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ touch day-1.txt
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ ls
day-1  day-1.txt  day-10  day-2  day-3  day-4  day-5  day-6  day-7  day-8  day-9
```

As you can see, there is day-1.txt in the list. That means we have created the day-1.txt file inside the 10-days-of-code folder. You can also you _ls -la_ command to use the detailed view of the folders and file.

### Opening and writing on file

Now, let's open the day-1.txt file and add some text to it. We use the _nano_ command to open and write.

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ nano day-1.txt
```

![](/images/nano.png)

As you can see from the above figure, the cursor is active and you can write on the pad. You can only use arrow keys to move the cursor left, right, up, and down. Let's write some text on the opened pad. There are instructors at the bottom that tells how to exit. For instance ctrl + x is to exit. When you exit either you save or cancel which comes when you click ctrl + x.

![](/images/writting_on_nano.png)

Now you can save the modified file by writing Y or you can cancel it by clicking ctrl + c.

After you write Y then click enter.

### Opening file to read

We can use the _cat_ command just only to read the file.

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ cat day-1.txt
This is my first text. I have never written on nano text editor before
```

### Copy file

Let's have day-1-backup.txt from day-1.txt by copying using the _cp_ command.

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code
$ cp day-1.txt day-1-backup.txt

exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code $ ls
day-1  day-1.txt  day-10  day-1-backup.txt  day-2  day-3  day-4  day-5  day-6  day-7  day-8  day-9
```

### Rename file

The _mv_ command is used both to change the name of a file and to move a file into a different directory.

Let's have more files in the 10-days-of-code folder. We can use the _touch_ command to create files.

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ touch day-2.txt day-3.txt day-4.txt day-5.txt
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ ls
day-1      day-10          day-2      day-3      day-4      day-5      day-6  day-8
day-1.txt  day-1-backup.txt  day-2.txt  day-3.txt  day-4.txt  day-5.txt  day-7  day-9
```

Now, let's rename the day-2.txt to second-day.txt using the _mv_ command.

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ mv day-2.txt second-day.txt

exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ ls
day-1      day-10          day-2  day-3.txt  day-4.txt  day-5.txt  day-7  day-9
day-1.txt  day-1-backup.txt  day-3  day-4      day-5      day-6      day-8  second-day.txt

```

Let's rename the day-10 directory to day-ten.

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ mv day-10 day-ten
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ ls
day-1      day-1-backup.txt  day-3      day-4      day-5      day-6  day-8  day-ten
day-1.txt  day-2           day-3.txt  day-4.txt  day-5.txt  day-7  day-9  second-day.txt
```

### Moving file and directory

The _mv_ and _cp_ commands can be used to put files into a directory. The _cp_ moves the copy of the file or the folder to another folder, however, mv just move it without copying.
Let's move the day-1.txt day-1 folder.

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ mv day-1.txt day-1
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ ls
day-1           day-2  day-3.txt  day-4.txt  day-5.txt  day-7  day-9    second-day.txt
day-1-backup.txt  day-3  day-4      day-5      day-6      day-8  day-ten
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ cd day-1
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code/day-1$ ls
day-1.txt
```

Let's try to move a file using the _cp_ command. Let's move the day-1-backup.txt to day-1 folder

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-git/10-days-of-code
$ cp day-1-backup.txt day-1

exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-git/10-days-of-code
$ cd day-1
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-git/10-days-of-code/day-1
$ ls
day-1.txt  day-1-backup.txt

exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-git/10-days-of-code/day-1
$ cd ..
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-git/10-days-of-code
$ ls
day-1             day-2  day-3.txt  day-4.txt  day-5.txt  day-7  day-9    second-day.txt
day-1-backup.txt  day-3  day-4      day-5      day-6      day-8  day-ten
```

The copied version of day-1-backup.txt moved to a day-1 folder.
Now let's create multiple backup files first and move them to a backup folder

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ mkdir backups
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ cd backups
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code/backups$ touch day-2-backup.txt day-3-backup.txt
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code/backups$ ls
day-2-backup.txt  day-3-backup.txt
```

Moving multiple files

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code
$ mv -t backups day-1-backup.txt day-2-backup.txt  day-3-backup.txt
```

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code
$ cd backups/
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code/backups
$ ls
day-1-backup.txt  day-2-backup.txt  day-3-backup.txt
```

### Delete file and directory

Let's remove the file using the _rm_ command. Let's remove the day-1-backup.txt file from the day-1 folder.

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code
$ cd day-1

exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code/day-1
$ ls
day-1.txt  day-1-backup.txt

exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code/day-1
$ rm  day-1-backup.txt

exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code/day-1$ ls
day-1.txt
```

Let's delete the day-ten folder using _rmdir_ command. The _rmdir_ delete a folder.

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code
$ rmdir day-ten

exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code
$ ls
backups  day-2  day-3.txt  day-4.txt  day-5.txt  day-7  day-9
day-1    day-3  day-4      day-5      day-6      day-8  second-day.txt
```

Now, let's copy the backups folder to backups-2 and backup-3 using _cp_ command. Then we will delete backups-3. The _cp_ with _-r_ has been used to copy it recursively.

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ cp -r backups backups-2

exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ ls
backups    day-1  day-3      day-4      day-5      day-6  day-8  second-day.txt
backups-2  day-2  day-3.txt  day-4.txt  day-5.txt  day-7  day-9
```

Now let's do the above step to create backups-3

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code
$ cp -r backups backups-3
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code
$ ls
backups    backups-3  day-2  day-3.txt  day-4.txt  day-5.txt  day-7  day-9
backups-2  day-1      day-3  day-4      day-5      day-6      day-8  second-day.txt
```

Now the backups-3 has files and neither the _rm_ nor the _rmdir_ deletes it. Therefore, we can use multiple commands to delete it. Let's try it with the following command.

```sh
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ rm -rf backups-3
exploitation@DESKTOP-KGC1AKC MINGW64 ~/Desktop/10-days-of-code$ ls
backups    day-1  day-3      day-4      day-5      day-6  day-8  second-day.txt
backups-2  day-2  day-3.txt  day-4.txt  day-5.txt  day-7  day-9
```

_Congratulations! Now you knew basic command lines_
