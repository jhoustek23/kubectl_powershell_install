PS > Set-ExecutionPolicy -ExecutionPolicy RemoteSigned
PS > [Net.ServicePointManager]::SecurityProtocol = "Tls12, Tls11, Tls, Ssl3"
PS > Install-Script -Name install-kubectl -Scope CurrentUser -Force
PS > install-kubectl.ps1
PS > cd C:\Users\xxxxxxxxx\AppData\Local\Temp\
PS > .\kubectl.exe version
copy your config to C:\Users\xxxxxxxxx\.kube\
PS > .\kubectl.exe get all
profit :)
