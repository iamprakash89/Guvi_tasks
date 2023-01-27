<h3> Day-3 Tasks</h3>

Platform: AWS  
OS: Amazon linux  


<h1> 1. Get me IP address of particular domain (guvi.in) </h1>

     The below commands used for identifying the IP address of the guvi.in domain.   
     1. ping -c 3 guvi.in   
     2. nslookup guvi.in   
     3. dig guvi.in   
     4. you can also use the online ipchecker webiste to identify the IP address (MXtoolbox->DNS Lookup)   

![alt text](https://github.com/devopskvk/Guvi_tasks/blob/main/Day-3-Network%20Basics/images/Day3_Task1.png)
![alt text](https://github.com/devopskvk/Guvi_tasks/blob/main/Day-3-Network%20Basics/images/Day3_Task1_dig.png)



<h1> 2. How do I find my CPU/memory usage of my server? </h1>
    
    The below commands used for verifyung the conectivity beween two nodes.
     1. top (it shows CPU and RAM memory)
     2. sar (It shows the hisotry of CPU utilization)
     3. sar -r  (It shows the hisotry of memory utilization)
     4. sar 2 5 ( display sar current utilization with 5 times interval of 2 seconds)
     5. mpstat command for displaying the CPU utilization
     6. vmstat command for displaying the memory utilization
     
![alt text](https://github.com/devopskvk/Guvi_tasks/blob/main/Day-3-Network%20Basics/images/Day3_Task2.png)
![alt text](https://github.com/devopskvk/Guvi_tasks/blob/main/Day-3-Network%20Basics/images/Day3_Task2_mpstat.png)


<h1> 3. Test the connectivity between 2 nodes? </h1>

     The below commands used for verifyung the conectivity beween two nodes.
     1.nmap
     2.ping (sometimes you cannot able to ping the ip address even the connection established, becuase the ICMP protocol will be blocked from the firewall end due to the ddos attack)
     3.ssh
     4.traceroute

![alt text](https://github.com/devopskvk/Guvi_tasks/blob/main/Day-3-Network%20Basics/images/Day3_Task3.png)
![alt text](https://github.com/devopskvk/Guvi_tasks/blob/main/Day-3-Network%20Basics/images/Day3_Task3_ssh.png)
![alt text](https://github.com/devopskvk/Guvi_tasks/blob/main/Day-3-Network%20Basics/images/Day3_Task3_traceroute.png)


<h1> 4. I have deployed an application in guvi.com:9000, and logs shows my app is running, but I’m unable to view the page. Check whether my port is open or not ? </h1>

    The below commands will help you to identify the port has been opened or not.
    1. nc -vz guvi.com 9000 
    2. namp 9000 guvi.com
    3.telnet guvi.com 9000
    4. The output shows clearly the port has been not opened form the firewall end.
    
![alt text](https://github.com/devopskvk/Guvi_tasks/blob/main/Day-3-Network%20Basics/images/Day3_Task4.png)
