# Shell Scripting Day-7

####  TASK1 Create a shell script to print the HTTP error code of guvi.in & print, the success/failure message based on the error code response 

The below script will check teh status code of the domain name. IF the status code is 200 then it will display a up and running otherwise the output shows not accessible.

--write-out used for capturing the status code.
--silent and --output options are used to prevent curl from printing any output to the console.

```
[root@testmachine ~]# cat statuscheck.sh 
#!/bin/bash

# Send HTTP request to guvi.in and capture the error code
HTTP_STATUS=$(curl --write-out "%{http_code}\n" --silent --output /dev/null https://www.guvi.in)

# Check the HTTP error code and print a message accordingly
if [ $HTTP_STATUS -eq 200 ]; then
    echo "Success: guvi.in is up and running (HTTP code $HTTP_STATUS)"
else
    echo "Failure: guvi.in is not accessible (HTTP code $HTTP_STATUS)"
fi
```

![alt text](https://github.com/devopskvk/Guvi_tasks/blob/main/Day7-ShellScriptingPart-2/Task1.PNG)


#### TASK2 Given a file, replace all occurrence of the word ""give"" with ""learning"" from 5th line till the end in only those lines that contain the word "welcome"Open Positions for Referrals


Before:

![alt text](https://github.com/devopskvk/Guvi_tasks/blob/main/Day7-ShellScriptingPart-2/task2.png)

command used to replace the string ```sed -i '5,${/welcome/s/give/learning/g}' filename.txt``` 

After: 

![alt text](https://github.com/devopskvk/Guvi_tasks/blob/main/Day7-ShellScriptingPart-2/task2_1.png)

Note: I used question as a input.
