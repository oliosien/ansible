
$ ansible -i hosts javadev -m shell -a "ls -la" -u eoliosi [-vvv for verbose]

ansible-playbook -i hosts playbook.yml [-k for ask password]

Docker reference

Dockerfile reference
https://docs.docker.com/engine/reference/builder/

Compose specification
https://docs.docker.com/compose/compose-file/

TODO
Creare una immagine con Dockerfile ed iniziare container con docker compose
Configurare via script ansible il container 