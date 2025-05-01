Utilizando Ansible para automatizar a VM na AWS com Docker, Iginx container NGINX na porta 80.

## Requesitos

- VM lab1 AWS Ubuntu 20.04+
- Chave ".pem" de acesso à instância.
- Ansible instalado na máquina local.
- Acesso à porta 80 liberado no Security Group da VM.

## Estrutura

- playbook_teste_porta_80.yml - verificar se o iginx esta rodando na porta 80.
- playbook_docker_nginx.yml - instala o Docker e sobe imagem iginx.
- host_aws - inventario com Ip da VM e chave de acesso SSH.

## Para Rodar

- Configura o host_aws com o IP que deseja a sua instância e alterar a chave .pem
- Rode o playbook.
