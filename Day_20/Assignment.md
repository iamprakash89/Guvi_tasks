Launch Jenkins and explore creating projects, users

Create a new project.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/1.png)

Select the new Item for creating the project.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/2.png)

 Enter the Project name and select what type of project you want to create. Here I am going with a freestyle project.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/3.png)
 
Press an OK button to create a project. The new page landing into configuration. Here you need to specify the project description and other configurations.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/5.png)
 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/6.png)
 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/7.png)

The new project has been created and has to wait for 5 mins more to auto-build.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/8.png)

Here I am creating for the pipeline project.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/9.png)

Now the configuration page is different from the normal project. You have to select the option which is required for you.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/10.png)

Now, I am going for the basic level.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/11.png)

Enabling the Poll SCM to run the script every five minutes. And I selected the hello world script for testing purposes.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/12.png)

Pipeline projected created and added into the dashboard.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/13.png)

I can see, the project has been executing every five minutes as per our periodic configuration.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/14.png)

The project has been run on the Jenkins server and can see the console output

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/15.png)

The output from the pipeline project. It has been triggered after 5 mins of project deployment.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/16.png)

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/17.png)

Now I am going to create a user and add users to the group. For this, you need to select the manage Jenkins options.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/18.png)

From manage Jenkins, select the Users options

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/19.png)

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/20.png)

Create a user as per your requirement and provide a reasonable name to remember.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/21.png)

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/22.png)

Enabling the Role-based Authorization Strategy plugins to provide user authorization using a Role-Based strategy. Roles can be defined globally or for particular jobs or nodes selected by regular expressions.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/23.png)

Once installed the plugin, I enabled the Role-Based strategy.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/24.png)

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/25.png)

I have created a new item role for user access. Creating item roles, allowing to set item-specific permissions (e.g Job, Run or Credentials) on Jobs, Pipelines and Folders.
You have to provide overall permission to access the jenkins page.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/26.png)

Now I assigned the role to users from the Assign role options.

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/27.png)

Likewise, I have assigned a role to the user.  The condition is Assignment role and pattern are the same projects, wise versa for the other project as well. 

 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/28.png)

Now While Assigning the project to specific users below
 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/29.png)

I am logging the Jenkins by user developer. The developer should be login and should see only the pipeline project.
 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/30.png)

We provided full access to run a job. It works as expected.
 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/31.png)
 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/32.png)

Tester users can able to log in and the assignment project has been displayed.
 ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/Day_20/images/33.png)


