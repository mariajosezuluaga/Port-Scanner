# PortScanner: A simple TCP port scanner that uses the 'socket' library to scan for open ports on a target machine.

import socket
def scan(t, p):  
        try:       
            stay = socket.socket()       
            stay.settimeout(2)        
            stay.connect((t, p))       
            b = sock.recv(1024)        
            print(f"Port {p} is open on {t} with banner: {b}")    
          except:      
            pass  
        finally:       
            stay.close()

def check_ip(ip):
    try:
        IP(ip)
        return (ip)
    except ValueError:


target = input("[+] Enter target website in format 'www.amazon.com': ")
targetIp = socket.gethostbyname(amazon)

for port in range(1, 100):
    scan(targetIp, port)

print("Scan complete!")
