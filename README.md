# linux-command
linux command for files creation and modification



## Task Description
This project demonstrates various file operations using shell commands on AWS EC2 instance.

## Tasks Performed

### 1. Directory and File Operations
- Created directory `my_folder`
- Created `my_file.txt` with sample text
- Created `another_file.txt` with sample text
- Concatenated `another_file.txt` to `my_file.txt`
- Displayed updated content

### 2. Bulk File Operations
- Created 20 files with `.txt` extension
- Renamed first 5 files to `.yml` extension
- Displayed latest 5 created files

## Commands Used

```bash
# Create directory and navigate
mkdir my_folder && cd my_folder

# Create files with content
echo "This is the first line of my_file.txt" > my_file.txt
echo "Got output for the first file and this is the second line" >> my_file.txt

echo "Content from another_file.txt - Line 1" > another_file.txt
echo "Content from another_file.txt - Line 2" >> another_file.txt
echo "Content from another_file.txt - Line 3" >> another_file.txt

# Concatenate files
cat another_file.txt >> my_file.txt

# Display content
cat my_file.txt

create exactly 20 .txt files
touch file1.txt file2.txt file3.txt file4.txt file5.txt file6.txt file7.txt file8.txt file9.txt file10.txt
touch file11.txt file12.txt file13.txt file14.txt file15.txt file16.txt file17.txt file18.txt file19.txt file20.txt

# List all files sorted by name
ls -l

# rename first 5 files (file1.txt to file5.txt)
mv another_file.txt another_file.yml
mv file1.txt file1.yml
mv file10.txt file10.yml
mv file11.txt file11.yml
mv file12.txt file12.yml


# List all files sorted by modification time (newest first) and show top 5
ls -lt | head -6

