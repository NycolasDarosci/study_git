____________________Começando no git________________________________________________________________

CONTROLE DE VERSÃO 
VCS – VERSION CONTROL SYSTEM

- Registro de alterações em um ou mais arquivos
- Lembrar versões específicas mais tarde
- Reverter para estado anterior determinados arquivos ou um projeto
- Compare as mudanças ao longo do tempo
- Veja quem modificou pala última vez algo que pode estar causando um problema
- Quem introduziu um problema ou quando
- Se você estragar tudo ou perder arquivos, você pode recuperar


	O QUE É GIT?

- Sistema de controle de versão distribuído
- Open-Source
- Pontos na história: commit (viagem no tempo)
- Histórico de alterações no código
- Voltar para qualquer ponto da história
- Controlar o fluxo de novas funcionalidades
- Ramificações: branch (universos paralelos)
- Vários devs no mesmo projeto
- Análise e resolução de conflitos
____________________________________________________________________________________________________

- Pwd - 
	Local do usuário
		

- mkdir “nome do arquivo” - 
criar um arquivo. “todo programador quando inicia um repositorio, começa com um arquivo README.md”

- git status -
status do git, mostra os arquivos que estão no stage area, working directory etc.

- git branch -
você cria um novo histórico; tive uma nova ideia e quero testá-lo sem comprometer o histórico principal, então cria-se um novo histórico.

- git chekout “nome do branch” -
mudar para o branch desejado

- cd Documents/git-test -
	entrar na pasta para iniciar um repositório

- ls -
	listar o que tenho na pasta

- git init -
	inicializar um repositório

- ls -a -
observar se eu tenho um diretório .git, pois quer dizer que o repositório deu certo. Consigo ver outros arquivos que criei

- ls -al .git -
	listar tudo que há dentro do diretório .git

- git log -
pontos da história quando o commit foi feito, por quem

- git log -n 5 -
	trazer o log dos últimos 5 commits



- vim file.txt -
	adicionar um arquivo
  		dentro do vim, aperte a tecla ‘i’ para escrever um texto, depois aperte ‘esc’ e aperte as teclas ’:wq’ que significa write and quit


- git add . -
	Depois disso, o git já identificou que tem uma modificação no projeto, agora eu preciso adicionar ‘add’. O ‘.’ Significa que estou me referindo a todos os arquivos do meu diretório local git

- git commit -m “inicial commit” -
	Adiciona um ponto na história do meu processo

- Touch qualquer coisa -
	Criar arquivo, depois que você dá git init

- git reset –soft –mixed --hard -
voltar algum commit que você deseja; soft não exclui nenhum commit, hard exclui todos os commits, àqueles depois do selecionado

- git rm –cached file2.txt -
	Quando você não quer commitar um arquivo, ele volta para o working directory
	
- git diff -
	Ver o que eu modifiquei no working directory durante o processo

- git diff --staged - 
	Ver o que eu modifiquei e já mandei para o stage area, pois quando dou um git add, git diff não localiza mais este que foi para o stage area (add)

- git mv file1.txt _file1.txtt -
	renomear arquivos com git mv e o nome

- cat file1.txt -
	ver o que está escrito dentro do arquivo

- git commit –-amend -m “change to file1.txt” -
	renomear o texto

- git checkout 148c6f53 – file1.txt -


- git clean -f -
remover arquivos

- git clean -n -
vai mostrar quais arquivos irão ser excluidos

- git revert HEAD~4 -
	trazer um arquivo do passado e fazer um novo commit

- git show 65b0bb063 -
	mostra todas as alterações que fizemos. É parecido com o git diff, mas esse funciona para quando já tem um commit

- git show 65b0bb063 -- src/views/* -
	posso entrar também nas pastas para ver o que eu mudei

	
