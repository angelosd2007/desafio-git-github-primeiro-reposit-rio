GIT

		INICIANDO O GIT
		INICIANDO O VERSIONAMENTO
		CRIAR UM COMMIT

	- Iniciando o GIT

* git init
* git add
* git commit

sempre o nome do programa na frente

	CRIANDO UM REPOSITÓRIO


Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE
$ ls
livro-receitas/

Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE
$ cd livro-receitas/

Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE/livro-receitas
$ git init
Initialized empty Git repository in C:/Users/Alien/Estudos/WORKSPACE/livro-receitas/.git/

Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE/livro-receitas (master)
$ ls

Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE/livro-receitas (master)
$ ls -a
./  ../  .git/

Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE/livro-receitas (master)
$

Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE/livro-receitas (master)
$ cd .git/

Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE/livro-receitas/.git (GIT_DIR!)
$ ls
HEAD  config  description  hooks/  info/  objects/  refs/

Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE/livro-receitas/.git (GIT_DIR!)
$ cd ..

Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE/livro-receitas (master)
$

Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE/livro-receitas (master)
$ git config --global user.email "joao.angelodasilva01@gmail.com"

Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE/livro-receitas (master)
$ git config --global user.name angelosd2007

Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE/livro-receitas (master)
$

Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE/livro-receitas (master)
$ git add*
git: 'add*' is not a git command. See 'git --help'.

The most similar command is
        add

Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE/livro-receitas (master)
$ git add *

Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE/livro-receitas (master)
$ git commit -m "commit inicial"
[master (root-commit) bb0155b] commit inicial
 1 file changed, 18 insertions(+)
 create mode 100644 Strogonoff_de_frando.txt

Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE/livro-receitas (master)
$ ^C

Alien@Alien-PC MINGW64 ~/Estudos/WORKSPACE/livro-receitas (master)
$
