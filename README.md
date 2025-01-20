# Phishing para captura de senhas do Facebook

### Objetivos

- Com intuito didático, temos como objetivo obter as senhas de usuário da rede social Facebook através da tecnica de phishing. Para isso, será utilizado a ferramenta ```settoolkit ```disponivel na distribuição ```Kali Linux ```. Iremos clonar a página de login oficial do Facebook, que estára disponível localmente e que irá coletar as credenciais inseridas pelo usuário e poderão ser visualizadas pelo log.

### Ferramentas

- Kali Linux
- setoolkit

### Configurando o Phishing no Kali Linux

1 - Garantir o acesso como root: ``` sudo su ```
2 - Iniciando o setoolkit: ``` setoolkit ```
3 - Selecionar o tipo de ataque (opção 1): ``` Social-Engineering Attacks ```
4 - Selecionar o vetor de ataque (opção 2): ``` Web Site Attack Vectors ```
5 - Selecionar o método de ataque (opção 3): ```Credential Harvester Attack Method ```
6 - Selecionar o método de ataque (opção 2): ``` Site Cloner ```
  6.1 - Definir o IP do host que receberá as solicitações dos usuários.
  Nota: Utilize o seguinte comando para obter o endereço da máquina: ``` ifconfig ```
  6.2 - Definir qual site será clonado. Nesse caso será a URL: ```http://www.facebook.com ```
7 -  Executar no computador do usuário usando o IP definido no passo 6.1
8 - Verificar os logs no Kali Linix (setoolkit)

### Resutados

![Alt text](./passwd.png "Optional title")
