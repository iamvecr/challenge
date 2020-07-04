## Challenge Kiratech 

Seguendo la [guida](https://www.hamvocke.com/blog/local-ansible-testing/) per testare tutto in locale, usando Vagrant.

#### How to

```bash
git clone https://github.com/vecr25/challenge
cd challenge
vagrant up
```



#### Contents

- `challenge.pdf`: la cosegna da rispettare, in particolare i primi tre punti
- `docker.yml`: playbook di Ansible che verrà eseguito sulle VM
- `Vagrantfile`: file di configurarzione per Vagrant che definisce le VM 
- `hosts`: contiene l'inventario per Ansible con il percorso per le private keys per connettersi alle VM
- `requriements.yml`: contiene la [collection](https://galaxy.ansible.com/ericsysmin/docker) che viene utilizzata per installare Docker*



*Scaricare questo modulo da Ansible Galaxy usando le API presenta un qualche bug che non viene trovato, quindi viene scaricato direttamente dalla repo.

**~~TODO~~ **

- ~~Fare il controllo sul disco delle vm, aumentare lo spazio (deafult 40GB)~~ 
- ~~Allocare <u>almeno</u> 40GB a Docker~~
- ~~Impostare Docker, possibile impletazione usando Ansible Galaxy con [questo](https://galaxy.ansible.com/ericsysmin/docker) modulo compatibile con *CentOS **7***~~


