Introduction:
The objective of this project is to build a python program that runs as a command-line tool. Basically, as a lazy programmer, my desktop is full of files as shown below. Due to a large number of files, it is a daunting task to sit and organize each file. To make that task easy, we need a Python script that comes in handy and returns a folder where all the files are organized in a well-manner within seconds. It should organize by size, last used or even extensions.

Python Modules used in the project:

OS Module:
The OS module in Python provides functions for interacting with the operating system. OS comes under Python’s standard utility modules. This module provides a portable way of using operating system dependent functionality.
os.scandir() method in Python is used to get an iterator of os.DirEntry objects corresponding to the entries in the directory given by specified path.
is_dir() method on os.DirEntry object is used to check if the entry is a directory or not.
os.stat() method in Python performs stat() system call on the specified path. This method is used to get the status of the specified path.
os.makedirs() method in Python is used to create a directory recursively.

Shutil Module:
The Shutil module in Python provides many functions of high-level operations on files and collections of files. It comes under Python’s standard utility modules. This module helps in automating the process of copying and removal of files and directories.
shutil.move() method Recursively moves a file or directory (source) to another location (destination) and returns the destination.

DateTime Module:
It's a combination of date and time along with the attributes year, month, day, hour, minute, second, microsecond, and tzinfo.
Python time method strptime() parses a string representing a time according to a format.
Approach Used:
Organizing by File Extension:
Checking the extension of the file in the computer directory and then comparing it with the dictionary values of extensions if matched then creating the new directory and inside it moving the different files according to the specified new directories.

Organizing by Size:
Checking the file size by using the if and elif conditions and then arranging the files into their specific folders by creating new directories as per the size of the files. All the files are first moved into (Organized Directory) then inside this folder all the other directories are created accordingly. files are arranged in the subsequent folders(BYTES,KB,MB,GB)

Organizing by Date Modified:
The values of date and time for the files are taken and stored inside the directories. After finding out the days it has been stored, the files are then moved to different directories according to the number of days by comparing it using the if else conditional statements.
