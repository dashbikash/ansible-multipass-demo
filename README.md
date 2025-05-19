# Multipaas Virtual Machines

## Generate SSH Key
ssh-keygen -t ed25519 -C "ubuntu" -f "$HOME/.ssh/multipass_vm"

## View and Copy Public key
cat ~/.ssh/multipass_vm.pub 

## Launch VM
multipass launch -c 1 -m 512m --cloud-init ./cloud-init.yml --name vm1