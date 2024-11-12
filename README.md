# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.

    mkdir %userprofile%\Desktop\MyLab
  
  
  ![image](https://github.com/user-attachments/assets/7afcae01-6fd9-4cde-b8ea-93013260c849)
  
## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
      
    cd %userprofile%\Desktop\MyLab
    type nul > MyFile.txt


![image](https://github.com/user-attachments/assets/da174949-5650-458e-8393-a59f160017c5)

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.

    dir %userprofile%\Desktop\MyLab


![image](https://github.com/user-attachments/assets/1be10505-56c3-4672-b3e0-2d6cf164e6b8)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

    mkdir %userprofile%\Desktop\Backup
    copy MyFile.txt %userprofile%\Desktop\Backup



![image](https://github.com/user-attachments/assets/2bc9b25b-a448-4c60-89b4-604656c960ee)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.

    move MyLab C:\Users\admin\Documents

![image](https://github.com/user-attachments/assets/e233df89-4558-4ea2-8da0-c1dba68cb63c)



## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

    @echo off
    mkdir %userprofile%\Desktop\DocBackup
    copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
    echo Backup completed successfully!

    @echo off
    mkdir %userprofile%\Desktop\DocBackup
    copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
    del %userprofile%\Documents\DocBackup\*.docx
    echo Backup and deletion completed successfully!




## OUTPUT

![image](https://github.com/user-attachments/assets/647afc97-1603-4702-930b-8f936bcb676e)




# RESULT:
The commands/batch files are executed successfully.

