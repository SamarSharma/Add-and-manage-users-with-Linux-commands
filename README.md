# Add-and-manage-users-with-Linux-commands

-The following demonstrates how I used Linux commands to add and manage users.

<p align="center">
Add a new user: <br/>
<img src="https://i.imgur.com/xwNVn0W.png" height="80%" width="80%" alt="File-Permissions-in-Linux"/>
<br />

- The screenshot's first line captures the command I typed using the "sudo useradd" command that added the user to the system. 
- The screenshot's second line captures the command I typed using the "sudo usermod -g" command, this put the added user "researcher9" to the research_team group as their primary group.



<p align="center">
Assign file ownership: <br/>

- The new user, researcher9, will take responsibility for project_r. We will be making them the owner of the project_r.txt file.
- The project_r.txt file is located in the /home/researcher2/projects directory, and owned by the researcher2 user.
- We will be using the "chown" command to make researcher9 the owner of project_r.txt.

<p align="center">
<img src="https://i.imgur.com/bvOOmAm.png" height="80%" width="80%" alt="File-Permissions-in-Linux"/>

- In this screenshot I checked if project_r.txt is in /home/researcher2/projects directory

<p align="center">
<img src="https://i.imgur.com/uMuWOpn.png" height="80%" width="80%" alt="File-Permissions-in-Linux"/>

- In this screenshot I made researcher9 the owner of project_r.txt



<p align="center">
Add the user to a secondary group: <br/>

- The user will now be added to a secondary group "sales_team".
- We will using -a amd -G to add the user into an existing group.

<p align="center">
<img src="https://i.imgur.com/gYLZ7YV.png" height="80%" width="80%" alt="File-Permissions-in-Linux"/>

<p align="center">
Delete a user: <br/>

- Now we will be deleting the user.
- We will be using the "userdel" or "groupdel" to delete the user

<p align="center">
<img src="https://i.imgur.com/XhTJ0P6.png" height="80%" width="80%" alt="File-Permissions-in-Linux"/>

- As seen in the screenshot, using "userdel" deletd the user. However, did not delete the group that was made for the user to be in.
- So I used the "groupdel" command to delete the group.




