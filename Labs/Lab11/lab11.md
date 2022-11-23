## Lab 11

- Name:
- Email

## Part 1 Answers

1. Hostname of the device: Wireless LAN adapter Wi-Fi 4:
2. MAC address of the NIC connected to the network: 00-13-EF-5F-3B-F3
3. IP address: 130.108.220.148
4. Subnet mask: 255.255.252.0
5. Gateway address: 130.180.220.1
6. DHCP server address:192.168.151.43
7. DNS server address: 130.108.128.200
8. Public IP used for communications outside subnet: 130.108.220.148

## Part 2 Answers

1. `tcpdump` command: sudo tcpdump -i any

   - How many packets were captured? 437445
   - Looking through the output, what traffic are you seeing? Traffic on my public IP.

2. Fancy `tcpdump` command: sudo tcpdump -i eth0 -A -vv host www.google.com

3. Capturing `google.com` traffic:
   - Was there a difference in output from `curl` when using `http` or `https`? No difference that I could notice.
   - Was there a difference in packet content in `tcpdump` when using `http` or `https`? the https version had a lot of dots in it.
   - What caused the difference? HTTPS is encrypted.
4. Save capture to a file:  sudo tcpdump -w eth0.pcap -i eth0 host www.bargainbinsbetterzone.ytmnd.com
   Read capture from a file:   tcpdump -r eth0.pcap
   Don't forget to `commit` and `push` your capture to your `Lab11` folder.

## Part 3 Answers

1. Command(s) to install `python3` and `pip3`: sudo apt install python3-pip (python3 was already installed)
2. Run web server with `index.html` contents in your folder: python3 -m http.server 9000
3. Confirm content is being served:
   - Using `localhost`: curl localhost:9000
   - Using the system's private IP: curl 44.211.102.140:9000
   - Using the system's public IP:  curl 10.0.0.25:9000
4. What's playing? Rick astley. I copied and pasted the link.
5. Command to show `LISTEN`ing processes:sudo lsof -nP -iTCP -sTCP:LISTEN
6. Command to `kill`: Kill 20013
