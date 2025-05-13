```
NAME : THIRUMALAI K
DEPT : AIML
REG NO : 212224240176

```




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

```
mkdir %userprofile%\Desktop\MyLab
```
![alt text](image.png)

```
mkdir my-folder

```

![alt text](<img/Screenshot 2025-05-13 233805.png>)

```
rmdir my-folder

```
![alt text](<img/Screenshot 2025-05-13 233831.png>)

## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
mkdir %userprofile%\Desktop\MyLab
```
![alt text](image-1.png)

```
COPY CON Rose.txt
A clock in a office can never get stolen
Too many employees watch it all the time


```
![alt text](<img/Screenshot 2025-05-13 234028.png>)

```
dir Rose.txt

```
![alt text](<img/Screenshot 2025-05-13 234108.png>)

```
echo hello world > hello.txt

```
![alt text](<img/Screenshot 2025-05-13 234237.png>)

```
type hello.txt
copy hello.txt hello1.txt
del hello1.txt

```
![alt text](<img/Screenshot 2025-05-13 234237.png>)

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![alt text](image-2.png)

```
type nul > MyFile.txt
```
![alt text](image-3.png)
```
assoc | more

```
![alt text](<img/Screenshot 2025-05-13 234309.png>)

```
fc hello.txt Rose.txt

```
![alt text](<img/Screenshot 2025-05-13 234408.png>)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![alt text](image-4.png)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup
```

![alt text](image-5.png)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![alt text](image-6.png)

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents
```
![alt text](image-7.png)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.







## OUTPUT

## 1.BAT:
```
@echo off
set name=John
echo Hello, %name%!
pause


```
![alt text](<img/Screenshot 2025-05-13 234648.png>)

## 2.BAT
```
@echo off
:main
set /p number=Enter a number: 
set /a remainder=%number% %% 2
if %remainder%==1 (
    echo %number% is an odd number.
) else (
    echo %number% is not an odd number.
)
:choice
set /p continue=Do you want to check another number? (Y/N): 
if /i "%continue%"=="Y" goto main
if /i "%continue%"=="N" goto end
echo Invalid choice, please enter Y or N.
goto choice
:end
echo Thank you for using the odd number checker!
pause

```
![alt text](<img/Screenshot 2025-05-13 234734.png>)

## 3.BAT

```
@echo off
for %%i in (1 2 3 4 5) do (
    echo Number: %%i
)
pause


```
![alt text](<img/Screenshot 2025-05-13 234806.png>)

## 4.BAT

```
@echo off
echo Reading lines from sample.txt...
for /f "tokens=*" %%i in (sample.txt) do (
    echo Fruit: %%i
)
pause

```
![alt text](<img/Screenshot 2025-05-13 234827.png>)

## 5.BAT

```
@echo off
echo Displaying Even or Odd for numbers 1 to 10
for /l %%i in (1,1,10) do (
    set /a rem=%%i %% 2
    if %%i %% 2 == 0 (
        echo %%i is Even
    ) else (
        echo %%i is Odd
    )
)
pause

```
![alt text](<img/Screenshot 2025-05-13 234928.png>)


# RESULT:
The commands/batch files are executed successfully.

