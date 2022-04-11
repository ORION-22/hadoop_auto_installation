# hadoop_auto_installation
Hadoop 3.2.2 on Ubuntu20.04 
# hadoop


Please follow the following steps.

1 - Download hadoop installer from https://hadoop.apache.org/   (Download-> check version -> binary download link)

Hadoop 3.2.2:: https://drive.google.com/drive/folders/1Ez02Rp1JGKp0suoOQlDBFbddpzJ6zJ_1?usp=sharing

2 - In the folder where hadoop tar.gz file is availabale, open the TERMINAL.

3 - Issue the following command to download this project's shells script


    
4 - Now you must have only two files in the directoy i.e. hadoop_auto.sh and apache hadoop tar.gz file.

5 - Issue the following command to make the shell script executeable.
    
    chmod 777 hadoop-<.tar.gz file name >
    chmod 777 hadoop_auto.sh
    
6 - Issue the following command to run the shell script.

    sudo ./hadoop_auto.sh
    
7 - Script will automatically install hadoop in your linux machine and create a new user with following credentials.

    User Name : huser        Password  : huser

8 - To start hadoop daemons, use the following commands.

    hdfs namenode -format
    /home/huser/hadoop/hadoop-3.2.2/sbin/start-dfs.sh
    /home/huser/hadoop/hadoop-3.2.2/sbin/start-yarn.sh
    jps

9 - For graphical interface, open firefox or any other web browser and visit the following locations.

    NAME NODE :  http://localhost:9870
    DATA NODE :  http://localhost:9864
    HADOOP :  http://localhost:8088
    
    
 Youtube Video Referred
 1. https://youtu.be/rThBuuedgcw
 ( https://github.com/khawajagan/hadoop)
