# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript
#### NAME : SARGURU K
#### REG NO : 212222230134

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

![image](https://github.com/Pooja-sri45/Windows-basic-commands-batchscript/assets/147081893/43c04a80-2aeb-46c5-926c-dc8e6f32eb95)



Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

cd %userprofile%\Desktop\MyLab

![image](https://github.com/Pooja-sri45/Windows-basic-commands-batchscript/assets/147081893/67a009f1-b4d6-4356-b87f-15dc157396be)



![image](https://github.com/Pooja-sri45/Windows-basic-commands-batchscript/assets/147081893/1082b00c-0af1-4445-ad80-605b91e07f80)



List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT

dir %userprofile%\Desktop\MyLab

![image](https://github.com/Pooja-sri45/Windows-basic-commands-batchscript/assets/147081893/1963245a-65be-45ce-a433-e8384d5c1fd4)




Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/Pooja-sri45/Windows-basic-commands-batchscript/assets/147081893/4704e7db-c415-4d86-b996-15dc2fb25948)


![image](https://github.com/Pooja-sri45/Windows-basic-commands-batchscript/assets/147081893/c2c436fe-4aca-4f50-915c-eb02d0fea19d)



Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents


![image](https://github.com/Pooja-sri45/Windows-basic-commands-batchscript/assets/147081893/162f89f0-00e4-49ac-ae5e-c284c52246e0)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```




## OUTPUT
![image](https://github.com/Pooja-sri45/Windows-basic-commands-batchscript/assets/147081893/a2556985-0ae8-474d-8c3a-8fc3cc08b9a1)






# RESULT:
The commands/batch files are executed successfully.

