# Process
# Task-01
curl https://jsonplaceholder.typicode.com/todos/1

curl https://jsonplaceholder.typicode.com/todos/1 | out-file .\task01.txt

get-content .\task01.txt | select-string "userid","status"

git add task01.txt

git commit -m "master commit" task01.txt

git push https://github.com/EdwardHsu-bot/Task.git master

# Task-02
$env:COMPUTERNAME | out-file .\computername.txt

Get-CimInstance -ClassName Win32_LogicalDisk -Filter "DriveType=3" | Format-List |out-file .\disk.txt

Get-CimInstance -ClassName Win32_ComputerSystem -Property UserName| Out-File .\user.txt

# Task-03
Set-Location D:\Task

Get-ChildItem | Out-File .\list.txt

Get-Content list.txt
