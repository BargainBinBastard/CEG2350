## Lab 08

- Name: Robert croop
- Email

## Part 1 Answers

1. Xvda. FOund by using lsblk
2. Yes, in addition to xvda there is xvdb
3. `gdisk` main menu options
   - `p` Print the partituion table
   - `o`create a new empty guid partition table
   - `n` add a new partition
   - `i`show detailed information on a partition
   - `w` write table to disk and exit
4. Using the `gdisk` utility on the disk: O and w to create a partition table, then open gdisk again, use n, go though the prompt, then w again.
5. sudo mkfs.ext4 xvdb1
6. mkdir expanse
7.sudo mount -t ext4 /dev/xvdb1 expanse
8. Skip - trust you to do it ;)
9. The command lists all the printable strings from within the file
10. The deleted file is still there.
11. shred -zvu -n  5 text.tst, file is no longer on the disk as aobservale from direectory.
12. sudo umount/mnt/expanse. No, all the files are gone.

## Part 2 Answers

1.
2. For `original.txt` identify:
   - Command to find the following info about `original.txt`:
   - inode number of `original.txt`: stat
   - number of blocks storing `original.txt`: stat
   - number of links to `original.txt`: stat
3. Command to create a hard link to `original.txt`:
   - What identifiers indicate a hard link was created? the presence of a new file-name in ls
   - Does modifying the hard linked file modify `original.txt`? Explain Yes, as the hard link is simply another path to the original file
4. Command to create a symbolic link to `original.txt` ln -s origninal.txt orignialer
   - What identifiers indicate a symbolic link was created? A new, blue string appears whne ysing ls
   - If `original.txt` was deleted, and a new `original.txt` was created, would the sym link still work? Explain yes, as they symbolic link points to the location of the file.
5. Command to create a copy of `original.txt` cp originalk.txt lab08
   - Does modifying the copied file modify `original.txt`? Explain 
6. Command to move `original.txt` to another directory. mv orgignnal.txt lab07
   - Does it have the same inode? Explain Yes, as the content of the file has not changed.
   - Was the hard link you created affected? Explain. No, as it is simply anotehr filename.
   - Was the symbolic link you created affected? Explain Yes, as it points to a specific location in the drive

## Extra Credit Answers

Line added to `/etc/fstab`:

```
Insert line here
```

```
Insert line here
```
