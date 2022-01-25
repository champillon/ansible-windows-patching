#patch windows with ansible
1. download following script to windows vm
```
https://raw.githubusercontent.com/ansible/ansible/devel/examples/scripts/ConfigureRemotingForAnsible.ps1
```
2. open "Powershell" as Admin on windows
3. run the downloaded script
```
ConfigureRemotingForAnsible.ps1
```
4. change the ip of windows vm and admin username/password on "hosts"
5. run the following command to patch windows
```
ansible-playbook patch-windows-vm.yaml -i hosts
```
