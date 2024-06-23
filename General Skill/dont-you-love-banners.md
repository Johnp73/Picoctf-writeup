# Overview #
`300 point`

# Description #
Can you abuse the banner? The server has been leaking some crucial information on tethys.picoctf.net 64908. Use the leaked information to get to the server. To connect to the running application use nc tethys.picoctf.net 60366. From the above information abuse the machine and find the flag in the /root directory.

# Write up #
1. Use the nc to log tethys.picoctf.net with port 64908 and 60366
   ![image](https://github.com/Johnp73/Picoctf-writeup/assets/109839076/0e055814-0cf9-4990-a3c2-7bbd9769b242)
   ![image](https://github.com/Johnp73/Picoctf-writeup/assets/109839076/3848e9f9-33b1-47e4-b07a-8d88f432057a)
   Some question can search on Google to find the answer

2. See in list /root
   ![image](https://github.com/Johnp73/Picoctf-writeup/assets/109839076/72f941df-58de-400b-8cbd-7a057daeef95)

   This is script.py
   ![image](https://github.com/Johnp73/Picoctf-writeup/assets/109839076/f011ea53-2209-4d4a-918c-3b80589487f0)
   
4. In script.py, see the code is print("*Please supply banner in /home/player/banner*"). So i use symlink to change flag.txt to banner (change name banner)
   ![image](https://github.com/Johnp73/Picoctf-writeup/assets/109839076/06565d63-a6bc-4514-83e3-3cfa176dd470)
   And there, banner ---> flag.txt

5. Exit the ctf-player and see the result
  ![image](https://github.com/Johnp73/Picoctf-writeup/assets/109839076/7e86c84a-8b95-4945-9073-c4c30b95d1ab)


   

  
    
   
