1. Installing VScode 
![image1](/images/week-1-lab-report-image1.png) 
a. I had Visual Studio installed prior to this course. I updated and confirmed it is a working version on my workstation. <br />
b. If not installed yet, [Visual Studio](https://code.visualstudio.com/) , and follow the instructions to install 
2. Remotely Connecting
![image2](/images/week-1-lab-report-image2.png)
a. I went to the link provided in the lab guide and reseted my password. After a successful reset, I was able to ssh onto the server with my account. <br />
b. Link for course-specific account: [Course-Account](https://sdacs.ucsd.edu/~icc/index.php) <br/> 
c. Steps to ssh: `ssh cs15lfa22@ieng6.ucsd.edu` then select yes when prompted then enter in password. You should recieve a message with your last login time, this means you have successfully ssh! 

3. Trying Some Commands
![image3](/images/week-1-lab-report-image3.png)
a. In this step, I was testing commands on the server side. I created a new folder and removed the folder. I accessed different directories and created new folders within. I was able to navigate between directories. 
4. Moving Files with scp
![image4](/images/week-1-lab-report-image4.png)
a. In this step, I created a java file named WhereAmI with sample code. I was able to successfully scp to the server. I was able to confirm the file was copied successfully by ssh into the server and checking if it is there. <br/>
b. Commands I used: <br/>
Starting on the client:
`scp WhereAmI.java cs15lfa22@ieng6.ucsd.edu`
To confirm the file is there:
`ssh cs15lfa22@ieng6.ucsd.edu "cat WhereAmI.java"`
5. Setting an SSH key 
![image5](/images/week-1-lab-report-image5.png)
![image6.2](/images/week-1-lab-report-image6.2.png)
a.After adding the public key to the directory on the server, I am still being prompted to enter my password when I login. I have confirmed the folder does exist on the server side so the scp command was successful. I viewed the authorized_keys folder and confirmed the key is in there. I am on a Mac device. Also, I am awaiting the Professor's advice on Piazza. I have looked into allowing permissions but I am not sure if I am able to do that with the server. <br />
b. Confirmed pub key is the same on both client and server. I have deleted and re-did the process. <br/>
c. Update 10/11/2022: I was able to fix with assistance 

6. Optimizing Remote Running
![image6](/images/week-1-lab-report-image6.png)
a. In this step, I used the terminal command ‘nano’ to edit within the terminal. I then copied the file WhereAmI.java to the server. I went ahead and compiled and ran the java file. Unfortunately, java is not installed on the server so the file was not able to run. In theory, this would have worked. 







