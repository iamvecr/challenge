## Challenge Kiratech 

Seguendo la [guida](https://www.hamvocke.com/blog/local-ansible-testing/) per testare tutto in locale, installo Vagrant.

- `files` cartella dove sono presenti i file che verranno sincronizzati sulla VM.

  - `local.yml` playbook di Ansible che verrà eseguito sulla VM

- `Vagrantfile`: file di configurarzione per Vagrant che definisce la VM 

  



**TODO** 

- Fare il controllo sul disco delle vm, aumentare lo spazio (deafult 40GB) 
- Allocare <u>almeno</u> 40GB a Docker
- Impostare Docker, possibile impletazione usando Ansible Galaxy con [questo](https://galaxy.ansible.com/ericsysmin/docker) modulo compatibile con *CentOS **7***


