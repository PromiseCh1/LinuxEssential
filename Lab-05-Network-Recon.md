🧪 LAB 5 – Linux Networking & Reconnaissance
🎯 Objective

Perform basic network reconnaissance using Linux tools.

📌 Tasks

1. Identify IP configuration
2. Detect listening services
3. Perform DNS investigation
4. Capture packets
5. Save network evidence

=========================Bash Commands====================
# Show IP information
ip a

# Show routing table
ip route

# Show listening services
sudo ss -tulnp

# DNS resolution
dig google.com
nslookup facebook.com

# Capture packets (run for 10 seconds)
sudo tcpdump -i any -w capture.pcap

# Analyze capture file
tcpdump -r capture.pcap

# Test connectivity
ping -c 4 8.8.8.8
