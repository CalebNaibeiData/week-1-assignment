# My Submission
*This submission includes the completed tasks and explanation.
The attached PDF contains all screenshots showing how I executed esch command and completed*

## Here is how I performed the assignment covering key Linux fundamentals
I learned how to navigate directories, create files/folders, perform file operations, manage permissions, and review command `history`.

---

### Login Verification
> First, I logged into the Ubuntu server to confirm I could access my assigned account. The screenshot below shows a successful login and my current working directory

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ufqetcqw32fk13bl8f5z.png)
> *I used the following commands*
`root` is the username
`143.110.224.135` is the server IP address
`-p` 22 specifies the SSH port
`whoami` username of the currently logged-in user(*it's screenshot found in the pdf folder at the end*)
`pwd` I used it to shows the exact directory I was currently working in (*it's screenshot found in the pdf folder at the end*)

---
### Folder & File Structure
> After logging in, I created my main project directory using my name, and added subfolders for raw_data, processed_data, logs, and scripts.




![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/8c7zqv7drvep378xspur.png)
> Using `mkdir` I created "Caleb_data_engineering" as my folder name and `mkdir raw_data processed_data logs scripts` to create Subfolders


The screenshot below shows the directory structure using the `ls -R` command, I used it to list all files and folders I had created

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/elw6tt5owp1pgay1gnri.png)

> The Subfolder Created stored:
`raw_data`  stores original data
`processed_data` stores cleaned/modified data
`logs`  stores log files
`scripts`  stores shell scripts

---

`nano` I used it to open and edit files directly from the command line.(terminal-based text editor)

### Raw and Processed Data Files
> I created sample CSV files to simulate real data: stock_data.csv in raw_data and cleaned_stock_data.csv in processed_data.


![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/39x8m9el04d7q9rl4bew.png)


These screenshots show the contents of each file.
> raw data
![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/424q2frmilfb2wryso5i.png)

> processed data
![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/prs6iuy7vt3qzyzevzns.png)


---
### Scripts and Logs
> I also created a simple script and a log file to track operations.
This screenshot shows the process_stock.sh script and the corresponding log file in action.


![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/jv0isuaevoc1wxqyizj6.png)

*I used command `touch` create empty files in each subfolder*
 
---
### Permissions and Navigation
> To practice Linux permissions, I restricted access to my main folder and made the script executable.
I also practiced navigating directories and listing hidden files.


![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/qo5u3p02uypybkkthhq7.png)

> At the end, I ran the `history` command to review all the commands I had executed during the assignment. As shown in the screenshot below 


![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/mkvb33witchz2u7h9uru.png)

---

## More commands Used in my assignment

For file operations, I used `cp` to create a backup file, `mv` to move and rename files, and `rm` to delete unnecessary files and keep the workspace organized.

For permissions, I used `chmod` to control access to my files and folders:

`chmod 700 ~/Caleb_data_engineering` was used to restrict access to my main project folder so that only the owner could access it.
In Linux permission terms, `700` means:
7 = read, write, and execute for the owner
0 = no access for group
0 = no access for others
`chmod 600` was used on important files such as the raw data file, cleaned data file, and log file.
This ensures that only the owner can read and write the file.
In this case:
6 = read and write for the owner
0 = no access for group
0 = no access for others

I also used `chmod +x` to make my shell script executable, allowing it to run directly from the terminal.

To confirm that the permission changes were applied correctly, I used ls -l, which displays file permissions and ownership details.

I then ran `./process_stock.sh` to execute my script, `ls -la` to list all files including hidden ones, and `!!` to re-run the previous command.

## Supporting Evidence

All screenshots showing how I completed the assignment are compiled in the PDF document below:
[Caleb_data_engineering_assignment_screenshot.pdf](https://github.com/user-attachments/files/26388413/Caleb_data_engineering_assignment_screenshot.pdf)

---

## Conclusion

> This assignment gave me practical exposure to essential Linux fundamentals for beginner Data Engineers.  
> By creating and organizing files, performing file operations, managing permissions, navigating directories, and reviewing command `history`, I strengthened my confidence in using the Linux terminal.  
> Mastering these basic skills is an important first step toward efficiently managing data workflows on remote servers.
