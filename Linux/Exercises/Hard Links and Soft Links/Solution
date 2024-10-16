
### Exercises with Hard Links

1. **Simple Hard Link (Level: Easy)**

    ```bash
    # Create a file
    echo "This is some text in the original file." > /home/user/original.txt

    # Create a hard link
    ln /home/user/original.txt /home/user/hard_link.txt

    # Modify the hard link
    echo "This text is added via the hard link." >> /home/user/hard_link.txt

    # Check content of the original file
    cat /home/user/original.txt
    ```

2. **Modify a File via Hard Link (Level: Medium)**

    ```bash
    # Create a file
    echo "This is a document." > /home/user/document.txt

    # Create a hard link
    ln /home/user/document.txt /home/user/link_document.txt

    # Delete the original document
    rm /home/user/document.txt

    # Modify the hard link
    echo "Data accessed via hard link." >> /home/user/link_document.txt

    # Verify data through the hard link
    cat /home/user/link_document.txt
    ```

3. **Check the Same Inode Usage (Level: Difficult)**

    ```bash
    # Create a file and hard link
    echo "This is a file." > /home/user/file.txt
    ln /home/user/file.txt /home/user/link_file.txt

    # Display the inodes of both files
    ls -i /home/user/file.txt /home/user/link_file.txt
    ```

### Exercises with Soft Links

4. **Simple Soft Link (Level: Easy)**

    ```bash
    # Create a file
    echo "This is some original text." > /home/user/original.txt

    # Create a soft link
    ln -s /home/user/original.txt /home/user/soft_link.txt

    # Modify the original file
    echo "New text added." >> /home/user/original.txt

    # Check content of the soft link
    cat /home/user/soft_link.txt
    ```

5. **Link a Directory with a Soft Link (Level: Medium)**

    ```bash
    # Create a directory and a file inside it
    mkdir /home/user/original_folder
    echo "File inside original folder." > /home/user/original_folder/file.txt

    # Create a soft link to the directory
    ln -s /home/user/original_folder /home/user/link_folder

    # Access the file via the soft link
    cat /home/user/link_folder/file.txt
    ```

6. **Broken Soft Link (Level: Difficult)**

    ```bash
    # Create a file and a soft link
    echo "This is a file." > /home/user/file.txt
    ln -s /home/user/file.txt /home/user/soft_link.txt

    # Delete the original file
    rm /home/user/file.txt

    # Check the status of the soft link
    ls -l /home/user/soft_link.txt  # Shows it's broken
    cat /home/user/soft_link.txt     # Attempt to access will fail
    ```

### Exercises with Hard Links and Soft Links

7. **Difference Between Hard Link and Soft Link (Level: Easy)**

    ```bash
    # Create a file
    echo "Text for the document." > /home/user/document.txt

    # Create hard and soft links
    ln /home/user/document.txt /home/user/hard_link_document.txt
    ln -s /home/user/document.txt /home/user/soft_link_document.txt

    # Delete the original document
    rm /home/user/document.txt

    # Check the hard link
    cat /home/user/hard_link_document.txt  # Should still work

    # Check the soft link
    cat /home/user/soft_link_document.txt   # Should fail
    ```

8. **Link a File in Another Directory (Level: Medium)**

    ```bash
    # Create a file in /tmp
    echo "This is a source file." > /tmp/source.txt

    # Create hard and soft links
    ln /tmp/source.txt /home/user/hard_link_src.txt
    ln -s /tmp/source.txt /home/user/soft_link_src.txt

    # Verify both links work
    cat /home/user/hard_link_src.txt
    cat /home/user/soft_link_src.txt

    # Delete the original source file
    rm /tmp/source.txt

    # Check both links after deletion
    cat /home/user/hard_link_src.txt   # Should still work
    cat /home/user/soft_link_src.txt    # Should fail
    ```

9. **Change the Destination of the Soft Link (Level: Difficult)**

    ```bash
    # Create a file and a soft link
    echo "This is file 1." > /home/user/file1.txt
    ln -s /home/user/file1.txt /home/user/link.txt

    # Change the soft link to point to a new file
    echo "This is file 2." > /home/user/file2.txt
    ln -sf /home/user/file2.txt /home/user/link.txt

    # Verify the soft link now points to the new file
    cat /home/user/link.txt
    ```

