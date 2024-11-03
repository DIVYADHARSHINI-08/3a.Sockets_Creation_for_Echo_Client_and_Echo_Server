# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
# AIM
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server .
4. Send and receive the message using the send function in socket.
## PROGRAM
## CLIENT :
```
Developed by: DIVYA DHARSHINI R
Reg no: 212223040042
import socket 
s=socket.socket() 
s.connect(('localhost',8000)) 
while True: 
    msg=input("Client > ") 
    s.send(msg.encode()) 
    print("Server > ",s.recv(1024).decode())
```
## SERVER :
```
import socket 
s=socket.socket() 
s.bind(('localhost',8000)) 
s.listen(5) 
c,addr=s.accept() 
while True: 
    ClientMessage=c.recv(1024).decode() 
    c.send(ClientMessage.encode())
```
## OUPUT
![WhatsApp Image 2024-11-03 at 14 28 58_d2b7f4c7](https://github.com/user-attachments/assets/16ee188d-3d2b-44ca-a6a5-ae6461d8d085)

![WhatsApp Image 2024-11-03 at 14 28 59_a09011be](https://github.com/user-attachments/assets/66fa2f94-732e-4052-9609-0233fd5089ff)

## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
