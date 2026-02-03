🧪 LAB 1 – Advanced Linux Basics & File Operations
🎯 Objective

Practice directory traversal, file operations, searching, and cleanup like a real Linux user.

📌 Tasks
1. Create a project directory linux_lab1
2. Create 3 subdirectories: docs, scripts, logs
3. Create 5 text files inside docs
4. Search for a specific file
5. Count total files and directories
6. Compress the project directory
7. Remove the original directory




=========Bash Commands==============
# Create main directory and subdirectories
mkdir -p linux_lab1/{docs,scripts,logs}
cd linux_lab1

# Create files inside docs
touch docs/file{1..5}.txt

# Search for a file
find . -name "file3.txt"

# Count total files
find . -type f | wc -l

# Count total directories
find . -type d | wc -l

# Compress the directory
cd ..
tar -czvf linux_lab1.tar.gz linux_lab1

# Remove original directory
rm -rf linux_lab1
