# ansible_training
## Notes from the training
### Useful commands
if you don't have a local ansible cfg file
ping all hosts
```bash
ansible all --key-file ~/.ssh/id_ed25519 -i inventory -m ping
```
if you have the appropiate cfg this is only whats needed
```bash
ansible all -m ping
```
if want to see the list of hosts in your inventory you are currently using
```bash
ansible all --list-hosts
```
with this command you get data about your clients - much output
without the --limit all hosts are queried / --limit only this one
```bash
ansible all -m gather_facts --limit <IP>
```
