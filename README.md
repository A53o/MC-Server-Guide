In this guide I will show you how to setup and install a Minecraft server on windows without port forwarding.

# Lets Start
1 First goto [Papermc.io/downloads/all](https://papermc.io/downloads/all) click on the version of Minecraft you Want in the side bar e.g.

 ![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/15414e6e-15f4-452f-b26c-06c8d156a304)

 2 Click download on the latest build of that version e.g.

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/6f9f9cc7-dc72-4123-8ff7-a8e946a8fa83)

3 Open files and create a folder in somewhere like documents and call it something memorable like "MC Server"

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/4a3b688c-00a2-43f3-91c6-24dbfc637ed6)

4 Move the file you downloaded in step 2 to the folder you just made, then rename it to paper.jar

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/a98b1873-a89f-412b-b6d4-b2fdca47b6ad)

If when before you rename the file it does not have the .jar extension the you need to turn file name extensions on

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/bd416bd4-7fe4-44f1-b658-6adc7e834f78)

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/98edfd38-ba01-4f4c-823c-a3f016d82a78)

5 Now right click and create a text file called ```run.bat```

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/e39063b8-05aa-44ff-8e1a-50fd1f4f7abc)

If you get this popup when renaming the file don't worry just click yes

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/5328b71c-e92f-40f2-ae7b-02e9b7f63ce7)

6 Open the file with notepad and write ```java -Xmx1024M -Xms1024M -jar paper.jar``` but change both of the "1024M" with the amount of ram you want to allocate in MBs

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/c0a9ec2a-ed95-4f08-9979-29472c5ebd80)

Then press Ctrl + S to save the file

# Install Java
To run the server you need to install java 17 (not minecraft java the java runtime)

1 goto this [page](https://www.oracle.com/java/technologies/downloads/#jdk17-windows)

2 click on the link for the x64 installer to download it

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/e6040caf-b8be-4e2d-b1b7-d615fecc09b1)

3 goto downloads in your files then double click the installer you just downloaded and click yes

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/85c9849e-c7d3-490f-b4ec-de47b45f31bf)

4 It will open the installer, click next>

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/0df74032-a0bf-494e-a9fd-1d3afbdd9ad6)

Next again

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/9b4f3536-96a5-4387-83a9-ef564acc41b6)

Now wait for it to install

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/16ef244c-2f6a-4bf3-abda-4f1bd8a316e2)

Then click close

![Screenshot from 2024-05-17 11-29-21](https://github.com/A53o/MC-Server-Guide/assets/146792539/c3709a5d-1794-40ea-b502-c17361b99cef)

java is now installed ;)

# Runing The Server

1 goto the MC Server folder you made then right click and create a text file called ```eula.txt```

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/66d788e1-8a25-4e44-b370-c7aed1fa3960)

2 in that eula.txt file write ```eula=true```

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/c28b3e8e-5e52-4493-91f1-97a5463ac649)

Then Press Ctrl + S to save

Now it should look like this

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/a6b081d9-36ae-4b46-8190-b33d20382e4e)

3 then just double click the run.bat file then it will install the server and run it if you get this popup click allow

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/b88ba6ee-40a4-4753-87f7-88e52c62fbb3)

Now Your server is runing! but we are not done yet

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/556fe723-9c67-40ff-893b-19ba3bf9d9a0)

# Opening The Server To The internet

First stop the server by typing ```stop``` in the console then hit enter

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/f1ed2737-881e-4189-9c3c-f25557b26dbd)

1 Click on this [link](https://github.com/minekube/connect-java/releases/download/latest/connect-spigot.jar) to download a plugin called Minekube Connect, this will help us open the server to the internet so other people can join.

2 Then goto the plugins folder in the MC Server folder, then move the file we just downloaded into there

3 Then double click the run.bat file again, then once the server is fully runing stop it

4 Now go back to the plugins folder then there should be a folder called connect (if there isn't then the plugin didin't enable) in that folder open the config.yml file with notepad

5 where it says ```endpoint: endpoint-name``` you can call it what ever you want I'm doing ```mcserverguide``` then press Ctrl + S to save

![image](https://github.com/A53o/MC-Server-Guide/assets/146792539/d821754b-a9e8-4174-b902-553a31a4fe0d)

6 finally you can double click the run.bat file and connect to your server at ```endpoint-name.play.minekube.net``` but replace endpoint-name with the name of the endpoint you set in step 5

# Turning on The Whitelist
the whitelist stops random people joining the server and to enable it join the server and type in chat ```/whitelist on``` and hit enter. now add your self to the whitelist and anyother people you want playing by typing ```/whitelist add  mc-username``` and hit enter but replace the mc-username with the user name of your player or any other player.


**Your Done Great Job I Hope This Guide Helped**
if you have an issue please open an [issue](https://github.com/A53o/MC-Server-Guide/issues)

&copy; 2024 A53o
