## NAME: AK PREETHI
## REG NO:212223230156
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


## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\MyLab

![image](https://github.com/PREETHI3312/Windows-basic-commands-batchscript/assets/151625222/134f1377-76b7-4145-bf7b-e7685d94ed1f)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
 cd %userprofile%\Desktop\MyLab
![image](https://github.com/PREETHI3312/Windows-basic-commands-batchscript/assets/151625222/aeab7967-f014-4fd0-b183-f447f2305c47)

 type nul > MyFile.txt
![image](https://github.com/PREETHI3312/Windows-basic-commands-batchscript/assets/151625222/1f79e0c7-71d9-4669-a3bf-53aec5cc31be)

List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT

 dir %userprofile%\Desktop\MyLab
 
![image](https://github.com/PREETHI3312/Windows-basic-commands-batchscript/assets/151625222/aa36c7e3-275e-46c0-a77f-6308f0ef1a07)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup
![image](https://github.com/PREETHI3312/Windows-basic-commands-batchscript/assets/151625222/680564bd-44b3-4dca-a128-91b83e92d44e)

 copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/PREETHI3312/Windows-basic-commands-batchscript/assets/151625222/9c59a0c6-e21a-4410-ac84-f82faa13c022)



Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT

 mkdir %userprofile%\Desktop\Documents
 
  move MyLab Documents
  
![image](https://github.com/PREETHI3312/Windows-basic-commands-batchscript/assets/151625222/da670a55-b756-4d44-812a-ba2c99153daf)





## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.


## COMMAND:

 @echo off mkdir %userprofile%\Desktop\DocBackup copy %userprofile%\Documents*.docx
  %userprofile%\Desktop\DocBackup echo Backup completed successfully!

## OUTPUT
![image](https://github.com/PREETHI3312/Windows-basic-commands-batchscript/assets/151625222/1ef4c9d1-634b-4711-99c7-0d11c91d7269)

## COMMAND

@echo off mkdir %userprofile%\Desktop\DocBackup copy %userprofile%\Documents*.docx
 %userprofile%\Desktop\DocBackup del %userprofile%\Documents*.docx echo Backup and deletion
 completed successfully!

 ## OUTPUT:
 ![image](https://github.com/PREETHI3312/Windows-basic-commands-batchscript/assets/151625222/f5e5b1c2-5c2e-4766-af18-8342fc039160)







# RESULT:
The commands/batch files are executed successfully.

