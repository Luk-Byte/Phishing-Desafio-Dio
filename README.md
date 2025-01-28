# Desafio de Criação de Phishing da DIO

Neste desafio de projeto, iremos criar um phishing para capturar senhas de login. Contudo, por motivos de segurança, a página indicada (http://www.facebook.com) não permite a coleta de e-mails e senhas. Para completar a tarefa, utilizei a página http://www.linkedin.com/login.

## Propósito Educacional: 

Este projeto é exclusivamente para fins de estudo e treinamento em segurança da informação. Não use estas ferramentas para atividades maliciosas.

## Ferramentas Utilizadas

- **Kali Linux**
- **Terminal Linux**
- **SeToolKit**

---

## Como Usar

### Pré-requisitos

Certifique-se de que as ferramentas estão instaladas no sistema operacional. Este tutorial utiliza o **Kali Linux virtualizado (WSL)** e as ferramentas funcionam via **linha de comando (CLI)**.

---

### Configuração do SetoolKit

1. Abra o terminal.
2. Torne-se superusuário:
   ```bash
   sudo su

1. Após se tornar superusuário no terminal, inicie o SetoolKit com o comando:  
   ```bash
   setoolkit

2. Selecione a primeira opção no menu:

       Social-Engineering Attacks

3. Escolha a segunda opção:

       Website Attack Vectors

4. Escolha a terceira opção:

       Credential Harvester Attack Method

4. Selecione a segunda opção:

       Site Cloner

Ao ser solicitado o endereço de IP, pressione Enter para que o SEToolkit detecte automaticamente o IP da sua máquina e o configure como padrão.

Digite o link do site que deseja clonar (por exemplo) e pressione Enter:

https://www.linkedin.com/login

Após isso, acesse o clone utilizando o IP detectado na etapa anterior.

Quando você realizar o login no site clonado, o terminal exibirá um log extenso. Embora o campo "USERNAME FIELD FOUND" possa não aparecer, o login será mostrado em PARAM: session_key=<usuário digitado>. 

A senha será mostrada em POSSIBLE PASSWORD FIELD FOUND: session_password= senha digitada

git add Phishing-Desafio-Dio/Captura de tela 2025-01-27 233846-1.png
git commit -m "Adicionando imagem ao repositório"
git push origin main



