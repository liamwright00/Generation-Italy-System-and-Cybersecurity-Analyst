

### Exercises with Hard Links

1. **Simple Hard Link (Level: Easy)**
   1. Create a file named `/home/user/original.txt`.
   2. Add some text to the file `original.txt`.
   3. Create a hard link named `/home/user/hard_link.txt` that points to `original.txt`.
   4. Modify the file `hard_link.txt` and verify that the content of `original.txt` is updated.

2. **Modify a File via Hard Link (Level: Medium)**
   1. Create a file named `/home/user/document.txt`.
   2. Create a hard link named `/home/user/link_document.txt` that points to `document.txt`.
   3. Delete `document.txt` and modify `link_document.txt`.
   4. Verify that the data is still accessible through the hard link.

3. **Check the Same Inode Usage (Level: Difficult)**
   1. Create a file `/home/user/file.txt` and a hard link `/home/user/link_file.txt`.
   2. Use the command `ls -i` to display the inodes of both files.
   3. Verify that the two files point to the same inode.
   > **Note:** The inodes for `file.txt` and `link_file.txt` should be the same.

### Exercises with Soft Links

4. **Simple Soft Link (Level: Easy)**
   1. Create a file `/home/user/original.txt` and add some text.
   2. Create a soft link named `/home/user/soft_link.txt` that points to `original.txt`.
   3. Modify `original.txt` and verify that the content of the soft link is updated.

5. **Link a Directory with a Soft Link (Level: Medium)**
   1. Create a directory `/home/user/original_folder` and inside it, create a file `file.txt`.
   2. Create a soft link named `/home/user/link_folder` that points to `original_folder`.
   3. Verify that you can access `file.txt` through the soft link.

6. **Broken Soft Link (Level: Difficult)**
   1. Create a file `/home/user/file.txt` and a soft link `/home/user/soft_link.txt`.
   2. Delete the original file `file.txt`.
   3. Check the status of the soft link and what happens when you try to access the file.
   > **Note:** The soft link will be "broken" and will produce an error when you try to access the file.

### Exercises with Hard Links and Soft Links

7. **Difference Between Hard Link and Soft Link (Level: Easy)**
   1. Create a file `/home/user/document.txt` with some text.
   2. Create a hard link `/home/user/hard_link_document.txt` and a soft link `/home/user/soft_link_document.txt` that both point to `document.txt`.
   3. Delete `document.txt` and verify the difference between the hard link and the soft link.

8. **Link a File in Another Directory (Level: Medium)**
   1. Create a file `/tmp/source.txt`.
   2. Create a hard link `/home/user/hard_link_src.txt` and a soft link `/home/user/soft_link_src.txt` that point to `/tmp/source.txt`.
   3. Verify that both links work, then delete `/tmp/source.txt` and check the difference.

9. **Change the Destination of the Soft Link (Level: Difficult)**
   1. Create a file `/home/user/file1.txt` and a soft link `/home/user/link.txt` that points to `file1.txt`.
   2. Modify the soft link to point to a new file `/home/user/file2.txt`.
   3. Verify that the link now points to the new file without touching the hard links.
