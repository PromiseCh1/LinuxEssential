🧪 LAB 3 – Users, Permissions & Security Audit
🎯 Objective

Understand permission misconfigurations and ownership risks.

📌 Tasks

1. Create two users
2. Create confidential files
3. Apply incorrect permissions
4. Identify insecure files
5. Fix permissions


==============Bash Command================
# Create users
sudo adduser analyst
sudo adduser attacker

# Create sensitive directory
mkdir secure_data
echo "Bank Credentials" > secure_data/finance.txt

# Apply insecure permissions
chmod 777 secure_data/finance.txt

# Find world-writable files
find . -type f -perm -o+w

# Fix permissions
chmod 640 secure_data/finance.txt

# Change ownership
sudo chown analyst:analyst secure_data/finance.txt

# Verify permissions
ls -l secure_data/finance.txt
