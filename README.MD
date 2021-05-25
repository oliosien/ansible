### Example ansible commands 

If you test groups node from inventory you can execute:

`$ ansible -i hosts.yml intesys --list-hosts`

We can execute a single module by command line:

`$ ansible -i hosts.yml javadev -m shell -a "ls -la" -u eoliosi [-vvv for verbose]`

If we are in a playbook context, we can choose a better way to execute more tasks using `ansible-playbook` command:

`$ ansible-playbook -i hosts.yml playbook.yml [-k for ask password or -K for becoming sudo]`
