🧪 LAB 4 – Process Monitoring & Threat Detection
🎯 Objective

Detect suspicious background processes.

📌 Tasks

1. Run background processes
2. Identify running processes
3. Monitor CPU usage
4. Kill suspicious process
5. Log process details

======================Bash Commands===================











=======================Hint========================
# Start multiple background processes
sleep 500 &
sleep 600 &
sleep 700 &

# List background jobs
jobs

# View all processes
ps aux

# Sort processes by CPU usage
ps aux --sort=-%cpu | head

# Identify sleep processes
ps aux | grep sleep

# Kill a process (replace PID)
kill PID

# Log current processes
ps aux > process_snapshot.log
