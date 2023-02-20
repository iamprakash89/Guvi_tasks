1. Create a shell script to print the HTTP error code of guvi.in & print, the success/failure message based on the error code response 

#!/bin/bash

# Send HTTP request to guvi.in and capture the error code
HTTP_STATUS=$(curl --write-out "%{http_code}\n" --silent --output /dev/null https://www.guvi.in)

# Check the HTTP error code and print a message accordingly
if [ $HTTP_STATUS -eq 200 ]; then
    echo "Success: guvi.in is up and running (HTTP code $HTTP_STATUS)"
else
    echo "Failure: guvi.in is not accessible (HTTP code $HTTP_STATUS)"
fi



2. Given a file, replace all occurrence of the word ""give"" with ""learning"" from 5th line till the end in only those lines that contain the word "welcome"Open Positions for Referrals

sed -i '5,${/welcome/s/give/learning/g}' filename.txt


sed is a stream editor that can perform text transformations on an input stream (such as a file).
-i is an option that tells sed to edit the file in place (i.e., modify the file directly instead of printing the output to the console).
5,$ specifies the range of lines that should be modified, from the 5th line till the end ($).
{/welcome/...} is a pattern matching expression that matches lines that contain the word "welcome".
s/give/learning/g is a substitution command that replaces all occurrences of the word "give" with "learning".
