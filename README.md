# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file . Save each script in a file with a .bat extension. Ensure you have the necessary permissions to perform the operations. Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.

## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/2b3acc25-c56c-4d79-a7d5-cb13b1828200)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT

```
cd %userprofile%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/dfe11a6e-4d15-49fa-bc29-930ed95520da)

```
type nul > MyFile.txt
```

![image](https://github.com/user-attachments/assets/5fb641bb-749a-49c8-8097-b921b4e208e4)

List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT

```
dir %userprofile%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/e37529fe-7b59-4449-9c79-68d35d1b56fc)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\Backup
```

![image](https://github.com/user-attachments/assets/beb93d64-6cc9-4bab-a2cc-e1f8be292766)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```

![image](https://github.com/user-attachments/assets/e3b07ac4-1301-4b6a-a7d7-f3fca9bb44c2)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\Documents
```

```
move MyLab Documents
```

![image](https://github.com/user-attachments/assets/9f10774d-8b68-49a2-a76f-cf9d85562312)


## COMMAND AND OUTPUT

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.csv %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
No files for backup
```

## OUTPUT

![image](https://github.com/user-attachments/assets/61572379-e948-4781-a569-b15bb0d0285c)

```
  @echo off
  mkdir %userprofile%\Desktop\DocBackup
  copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
  del %userprofile%\Documents\*.docx
  echo Backup and deletion completed successfully!
```

## OUTPUT

![image](https://github.com/user-attachments/assets/fe3bfeef-8953-4c7e-a2f5-a57de4f91766)


# RESULT:
The commands/batch files are executed successfully.

