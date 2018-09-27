Set-ExecutionPolicy -ExecutionPolicy RemoteSigned
[Net.ServicePointManager]::SecurityProtocol = "Tls12, Tls11, Tls, Ssl3"
Install-Script -Name install-kubectl -Scope CurrentUser -Force
install-kubectl.ps1
cd C:\Users\xxxxxxxxx\AppData\Local\Temp\
.\kubectl.exe version
copy your config to C:\Users\xxxxxxxxx\.kube\
.\kubectl.exe get all
profit :)
