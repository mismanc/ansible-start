# ansible-start

This is an ansible starter project
#### Check inventories accessible
`ansible all --key-file ~/.ssh/id_ed25519 -i inventory -m ping`
##
#### After we move configurations to ansible.cfg file
`ansible all -m ping`

##
#### List hosts
###
`ansible all --list-hosts`

##
**Execute 'apt update' on every host**
###
`ansible all -m apt -a update_cache=true`

##
**Execute 'apt update' on every host with login (sudo)**
###
`ansible all -m apt -a update_cache=true --become --ask-become-pass`
