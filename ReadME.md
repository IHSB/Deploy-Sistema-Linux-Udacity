# Deploy-Sistema-Linux-Udacity

### IP de Acesso
* Endereço IP: 3.89.10.235


### Resumo de instalações e mudanças nas configurações
Configuração do servidor:
* (Amazon Lightsail)[https://lightsail.aws.amazon.com];
* Linux/UNIX;
* SO: Ubunto 16.04 LTS

Configuração Check-list:
* Adicione o usuário 'grader' - 'adduser example_user';
* Adicione privilégios 'sudo' - 'adduser example_user sudo';
* Para (SSH Key)[https://www.linode.com/docs/security/securing-your-server/#create-an-authentication-key-pair];
* Configure o Firewall:
'''
$ sudo ufw default deny incoming
$ sudo ufw default allow outgoing
$ sudo ufw allow 2200/tcp
$ sudo ufw allow www
$ sudo ufw allow ntp
$ sudo ufw enable
'''
* Verifique se não há nenhum update: '$sudo apt-get update', aguarde e após concluir '$sudo apt-get upgrade', para atualizar os packages existentes.
