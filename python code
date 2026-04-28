import socket

target = "scanme.nmap.org"

for port in range(1, 44):  
    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
    sock.settimeout(1)
    
    result = sock.connect_ex((target, port))
    
    if result == 0:
        print(f"Port {port} --> OPEN")
    else:
        print(f"Port {port} --> closed")
    
    sock.close()
