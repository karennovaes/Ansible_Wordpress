# Ansible: Automatizando a Instalação do WordPress

Este repositório contém o código-fonte desenvolvido durante o curso "Ansible: Infraestrutura como código" da Alura. O objetivo do projeto é demonstrar como automatizar completamente o processo de provisionamento e configuração de um ambiente web para hospedar um site WordPress, utilizando Ansible para orquestrar todas as tarefas em servidores na AWS.

## 🎯 Objetivo do Projeto

O objetivo é criar um playbook Ansible que, ao ser executado, configure um servidor  Ubuntu dozero, instalando e configurando todos os componentes necessários para instalar o WordPress.

Isso elimina a necessidade de configuração manual, garantindo um ambiente consistente, repetível e escalável.


## 📋 Pré-requisitos

Antes de executar este playbook, você precisará de:

- Ansible Instalado: O Ansible deve estar instalado na sua máquina de controle.

- Servidor de Destino: Um ou mais servidores Ubuntu 22.04 já provisionados.

- Acesso SSH: Sua máquina de controle deve ter acesso SSH ao servidor de destino através de um par de chaves.

- Inventário Configurado: Um arquivo de inventário (ex: hosts) que lista os endereços IP dos seus servidores e as variáveis de conexão.

## 🚀 Como Executar

#### Clone o Repositório:

```bash
#!/bin/bash
git clone https://github.com/alura-cursos/Ansible_Wordpress.git
cd Ansible_Wordpress
Configure seu Inventário:
Edite o arquivo inventory/hosts.ini e substitua SEU_IP_AQUI pelo endereço IP do seu servidor e o caminho para sua chave SSH.
``` 

#### Execute o Playbook: 

Use o comando ansible-playbook, especificando o arquivo de inventário e o playbook principal.

```bash
#!/bin/bash
ansible-playbook -i inventory/hosts.ini playbook.yml
``` 

#### Acesse seu Site:

Após a execução bem-sucedida, abra seu navegador e acesse o endereço IP do seu servidor. Você será recebido pela famosa tela de instalação de 5 minutos do WordPress para finalizar a configuração.


