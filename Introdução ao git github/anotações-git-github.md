GIT 

COMANDOS BÁSICOS PARA UM BOM DESEMPENHO NO TERMINAL


dir = abrir mapa do sistema operacional Windows e abrir lista de diretórios
cd = mudar de diretório
mkdir = criar diretório
del / rmdir = excluir diretórios


Como o GIT o funciona abaixo dos panos.
- SHA1
- OBJETOS FUNDAMENTAIS
- SISTEMA DISTRIBUIDO
- SEGURANÇA

		SHA1
A sigla SHA significa Secure Hash Algorithm (Algoritmo de Hash Seguro), é um conjunto de funções hash criptográficas projetadas pela NSA (Agência de Segurança Nacional dos EUA).

A encriptação gera um conjunto de characteres identificador de 40 dígitos.
Se alterado o algoritmo, gera uma nova encriptação (segurança).

		OBJETOS INTERNOS DO GIT
BLOBS
TREES
COMMITS

	BLOBS (bolhas) - contem meta dados do GIT (tamanho/tipo/sha)
	TREES (arvores) - armazena BLOBS e conte além dos dados acima, também o nome dos arquivos.
Apontam tanto para as bolhas quanto para as arvores.
	COMMITS - englobam tudo, tanto arvores quanto bolhas e para outros commits, apresentam dados como data e hora de criação e também possuem criptação própria.
Qualquer alteração realizada no commit é sinalizada.

É hierarquia
COMMITS acima
TREES no meio
BLOBS abaixo de todos

		O GIT É UM SISTEMA DISTRIBUIDO SEGURO
Se acaso mais de uma pessoa começar a trabalhar no mesmo código, todas teram o seu shar e versão do código.

		CHAVES SSH E TOKENS
Chave SSH
Estabelece uma conexão segura com o GIT
Configurar minha maquina para ser segura

		CRIANDO UMA CHAVE SSH

Alien@Alien-PC MINGW64 ~
$ ssh-keygen -t ed25519 -C joao.angelodasilva01@gmail.com

Generating public/private ed25519 key pair.
Enter file in which to save the key (/c/Users/Alien/.ssh/id_ed25519):
Created directory '/c/Users/Alien/.ssh'.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/Alien/.ssh/id_ed25519
Your public key has been saved in /c/Users/Alien/.ssh/id_ed25519.pub
The key fingerprint is:
SHA256:HgEjMdcX9/FILMg4Q8hmOjiaILRVKHyCnzAh/InDTDo joao.angelodasilva01@gmail.com
The key's randomart image is:
+--[ED25519 256]--+
|*.  *+++.o.o..o  |
|=B + +=o= +..o.+ |
|*+Oo.+  .+   .o .|
|E*=oo    .       |
|o+.. .  S        |
|o      . .       |
|        .        |
|                 |
|                 |
+----[SHA256]-----+

Alien@Alien-PC MINGW64 ~
$ cd /c/users/Alien/.ssh/

Alien@Alien-PC MINGW64 /c/users/Alien/.ssh
$ ls
id_ed25519  id_ed25519.pub

Alien@Alien-PC MINGW64 /c/users/Alien/.ssh
$ ^C

Alien@Alien-PC MINGW64 /c/users/Alien/.ssh
$ cat id_ed25519.pub
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAICDVcJD+6uIjXldqyc26YLcgMDtB+RoLH58Kadmpwzxi joao.angelodasilva01@gmail.com

Alien@Alien-PC MINGW64 /c/users/Alien/.ssh
$ ls
id_ed25519  id_ed25519.pub

Alien@Alien-PC MINGW64 /c/users/Alien/.ssh
$ pwd
/c/users/Alien/.ssh

Alien@Alien-PC MINGW64 /c/users/Alien/.ssh
$ eval $(ssh-agent -s)
Agent pid 227

Alien@Alien-PC MINGW64 /c/users/Alien/.ssh
$ ssh-add id_ed25519
Enter passphrase for id_ed25519:
Identity added: id_ed25519 (joao.angelodasilva01@gmail.com)

Alien@Alien-PC MINGW64 /c/users/Alien/.ssh
$



		TOKEN DE ACESSO PESSOAL
Como se fosse um acesso via Token
O Token fica guardado no PC
(sem necessidade).











