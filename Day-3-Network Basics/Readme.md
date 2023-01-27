Day-3 Tasks

<h1> 1. Get me IP address of particular domain (guvi.in) </h1>
    The below commands used for identifying the IP address of the guvi.in domain.   
    ping -c 3 guvi.in   
    nslookup guvi.in   
    dig guvi.in   
    you can also use the online ipchecker webiste to identify the IP address (MXtoolbox->DNS Lookup)   
    

![alt text](https://github.com/devopskvk/Guvi_tasks/blob/main/Day-3-Network%20Basics/images/Day3_Task1.png)
![alt text](https://github.com/devopskvk/Guvi_tasks/blob/main/Day-3-Network%20Basics/images/Day3_Task1_dig.png)

<h1> 2. How do I find my CPU/memory usage of my server? </h1>
![alt text](https://github.com/devopskvk/Guvi_tasks/blob/main/Day-3-Network%20Basics/images/Day3_Task2.png)

<h1> 4. I have deployed an application in guvi.com:9000, and logs shows my app is running, but I’m unable to view the page. Check whether my port is open or not ?</h1>

    The below commands will help you to identify the port has been opened or not.
    nc -vz guvi.com 9000
    namp 9000 guvi.com
    telnet guvi.com 9000
    The output shows clearly the port has been not opened form the firewall end.
![alt text](https://github.com/devopskvk/Guvi_tasks/blob/main/Day-3-Network%20Basics/images/Day3_Task4.png)
