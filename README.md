# NetworkLogger
****

>New tool to generate TCP traffic and packet capture according to your needs.

--------

### Simple tutorial on how to work with NetworkLogger.

#### The folder will have the following files:

 ![image](https://user-images.githubusercontent.com/110167869/182664997-c2cb6b01-15c8-465e-a8f3-5a7596acec68.png)


#### We can then open the highlighted “NetworkLogger.exe” file that would lead us to the following window:

 ![image](https://user-images.githubusercontent.com/110167869/182665122-fc5973e7-1816-49d1-a207-36baa904f197.png)

```
1 - Text box to insert the test string.
2 - Button to leave the program.
3 - Button to start the program.
4 - Information on the string Syntax.
```

#### Now we can insert the string following the syntax:

```
Generate TCP traffic and Packet Capture:  "<DestinationIP>,<TCPport>,<Normal/Circular>" Ex: 1.1.1.1,80,normal
Simply packet capture: "**"
````

### A packet capture choice of either Normal or Circular would lead us to the next window:

 ![image](https://user-images.githubusercontent.com/110167869/182665288-6b4fbc5a-80b0-4626-aad2-f5676179a120.png)

```
1 - TCP Statistics
2 - Packet Capture details
3 - Txt file information
4 - Path of created files
5 - TCP output 
6 - Revert to initial window
7 - Redo the tests
8 - Close the Application
  ``` 
>Throughout the process we have various messages, showing what's being written on the CMD and the output of the same. Making the application as transparant as possible to the end user.

##### Initial Pop up with Netsh command inserted on the CMD.

 ![image](https://user-images.githubusercontent.com/110167869/182665480-6d5de6f1-27a0-4ff6-8089-2d55d87dcc5d.png)

 
##### After concluding the TCP connections:
  
```
Normal : 10 TCP connections.
Circular: Loop until it finds an issue, if one connection fails, it will do 15 more TCP connections and conclude the proccess.
```
  
##### Pop up indicating Netsh packet stopped and files generated.
  
 ![image](https://user-images.githubusercontent.com/110167869/182665526-0eb8bd7a-9450-4207-8a8a-ac1c5c81419b.png)

 
##### Pop up indicating file conversion from Etl to Pcapng.
  
 ![image](https://user-images.githubusercontent.com/110167869/182665553-a66feca9-0bcb-4d16-ad01-b7781099a6d4.png)


### After this, if you reach your output folder, you’ll be able to find the following:

![image](https://user-images.githubusercontent.com/110167869/182665598-f6f00a78-196f-45a0-83f0-2301e624a624.png)
                                                                                                        
-------
  
## How to simply use the tool to packet capture on a windows device?
  
 >Simply use the string "**" on the first 
  
### The window you would see is as follows:
  
![image](https://user-images.githubusercontent.com/110167869/182667041-e1ab301c-8b44-46e4-bf77-69cb85261be7.png)

 
 ```                                                 
1 – State of the packet capture
2 – Files generated Location
3 – Button to stop the capture
  ``` 
  
****

## FAQ
#### What is used to generate the packet captures?
> Netsh is used to packet capture via CMD.
  
#### How is the file converted from ETL to PCAPNG?
> The utility etl2pcapng is used. You can review more on about it on https://github.com/microsoft/etl2pcapng.
 
#### Do i need to open the file in admin mode?
>Yes, otherwise it's not possible to run Netsh on the CMD.

 #### Can i see the source code?
>Yes, you can see it here https://github.com/jose-slv/NetworkLoggerSourceC.
