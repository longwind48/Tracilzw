# Getting Hive to work for Windows users

Hi Windows Users, don't lose hope.

There is actually a much simpler way to run the components in the hadoop ecosystem (HDFS, Hive, Pig, etc) without installing them. We will make use of Hortonworks HDP Sandbox, Oracle VM virtualbox, Putty, WinSCP.

Requirements:
  - 8GB Ram (can try it with 4GB)
  - at least 25GB of storage in your local drive.
  - Patience.

# 1st Step
Follow the tutorial given by this video. 
This is the bulk of the installation, i.e. getting Ambari UI to work. 
https://www.youtube.com/watch?v=7sxqHgBdxB8

Let's configure the settings of the sandbox so that it will run with less lag.
- Open Oracle VM VirtualBox, Click on Hortonworks Docker Sandbox -> Settings -> System -> MotherBoard -> 
- In 'Base Memory', Shift the threshold pointer to the cutoff point of the green and red bar. 
- In 'Processor', Shift the threshold pointer too.

# 2nd Step
Follow the tutorial given by this video.
This is to setup putty to connect to the sandbox (because the first step only gives you the UI to work with). After this is done, we'll get the command line working.
https://www.youtube.com/watch?v=jWfv_62I1R4

# 3rd Step
Now, with the Ambari UI and command line working, we will now worry about transferring files from your local system to the remote computer (Hortonworks sandbox). 
 - install WinSCP: https://winscp.net/eng/download.php
 - Let it import the settings from Putty to it. (It automatically does that when you have it installed)
 
 And now, with winSCP, you can transfer local files to your sandbox, which allows you to follow the steps given in ST446 github, (because you need to transfer the data files to the sandbox before you can do anything).

# Finally

A couple of us has created a ST446 Whatsapp group for Windows users. Add yourself in. Say hi. Ask some questions.
https://chat.whatsapp.com/CvTMcCGaGuK0RagpHqATUx



