Roteiro da Prática 01

** A maioria dos erros acontecem por não estar na pasta certa no terminal. Verifique sempre a pasta com o comando pwd e se não estiver na parte correta, navegue até ela. Os comandos e roteiro realizado na aula do dia 25/08/2021 estão disponíveis na pasta do Drive com o nome de “Prática 00”.

Parte 1 – Github (https://github.com)

1.	Criar conta e usuário no github
2.	Criar um repositório chamado AulaGit01 (Não esqueça de marcar a opção Inicializar com o Readme (para o repositório já ser inicializado))
3.	Copiar o link do repositório

Parte 2 – Arquivos para prática

1.	Fazer o download das pastas Códigos e PDF na pasta do Drive.

Parte 3 - Credencial 

1.	Abrir o terminal do sistema operacional
2.	Inserir os comandos abaixo (Para quem não tiver configurado):
         git config --global user.email "you@example.com"
         git config --global user.name "Nome do Usuario"

Parte 4 – Atualizando o repositório local. 

1.	Abra o terminal e insira o comando git clone “LINK DO REPOSITÓRIO CRIADO NO GIT HUB" (Pesquisar sobre o Git Clone)
2.	Copie os arquivos / diretórios obtidos na Parte 2 para dentro da pasta AulaGit01.

Parte 5 – Atualizando o repositório WEB. 

1.	Abra o terminal e navegue até o diretório AulaGit01 (local do clone) obtido na Parte 4.

2.	Adicione os arquivos novos ou atualizados
       git add Codigos/*      (Adiciona os arquivos em uma pasta chamada Codigo presente na raiz)
       git add PDF/*           (Adiciona os arquivos em uma pasta chamada PDF presente na raiz)


3.	Commit das alterações realizadas
       git commit -m “Adicionando pastas e arquivos”

4.	Atualize o repositório oficial
       git push -u origin main


Observações:
Não esqueça de conferir sempre o status (git status) e também de olhar os logs dos commits seja no GitHub ou via terminal (git log). Você também pode adicionar outro arquivo ou código no repositório que achar interessante e realizar mais commits. Não esqueça de fazer um bom comentário no seu commit. A parte 6 abaixo inclui a utilização de Branchs (Ramos) que veremos na próxima aula. 

Parte 6 – Criando Branch. 

1.	Abra o terminal e navegue até o diretório AulaGit01 (local do clone) obtido na Parte 4.

2.	Crie o branch developer
git branch developer

3.	 Altere para o branch developer 
git checkout developer

4.	Crie o arquivo cart.html em Código e adicione algum comentário nele

5.	Adicione os arquivos novos ou atualizados
       git add cart.html

6.	 Commit das alterações realizadas
       git commit -m “Adicionando carrinho”

7.	 Altere para o branch main
git checkout main

8.	Faça um merge com o branch developer
git merge developer

9.	Atualize o repositório oficial
       git push
