#Anotações **Git/GitHub**
 - Link útil para arquivos Markdown
 	[Acesse aqui](https://www.markdownguide.org/cheat-sheet/)
	
 - _Notas_
 
 ## **GIT e GITHUB**

 São aplicações diferentes. Git livre Github da Microsoft.

 _UNIX_        **Windows**
  - _cd_          **cd**   - navega nas pastas - Cd.. - volta um nível. cd + pasta entra na pasta. Cd/ volta ao nível principal.
  
 - **_clear_** - limpa a tela comando+l
  - ***Is***  lista os arquivos dentro da pasta ou repositório
  - *ls -a* -lista os arquivos e pastas ocultos.
  -                  - **dir**
  - _mkdir_     -**mkdir** - cria pastas
  - "echo > . Nome do arquivo. Extensão" - cria um arquivo na pasta. Ex. echo Olá mundo > teste.txt
 
  - **rm -rf** rm(remover Repositório) r(recursivo para deletar tudo dentro da pastas, inclusive as pastas dentro das pastas) f(forçar esse evento sem pedir permissão)   - del/ rmdir(windows)
  - **mv** "arquivo".extensão  /'nova pasta'/


 SHA1 - Secur Hash Algorithm - encriptado com identificador de caracteres de 40 dígitos.

  - Blob - Bloco básico de composição - 'blob 9/0conteúdo
  - Trees -  armazena blobs. 
        Tree aponta para blobs ou para outras trees.
        Se mudarmos uma "," nos arquivos mudamos toda a estrutura de metadados (sha1) dos Blobs e das trees.

  - Commit - une todos os arquivos, aponta para eles.
       commit aponta para um parente (outro commit) tree, autor, mensagem timestamp\
 commit único para cada autor, também tem um sha1 dele. Caso seja alterado algo no arquivo, alteração reage em cadeia alterando o sha1 do commit também. 

 no terminal o nome do programa vem na frente e o comando após.
  - git init - inicializa um repositório do git na pasta selecionada.
      - Untracked - arquivo criado fora do git com o comando git add
      - unmodified - arquivos sem modificação. via Sha1
      - modified - Quando há modificação no Sha1
      - staged - na sala de espera para algo esperando ser um commit
      - retorna para unmodified.
      - Isso é um ciclo.

  - git add - Arquivo não traçado para unmodified

  - git commit - move os arquivos da área de stage para o local repository. E daqui podemos colocar ele no repositório remoto.

 - git status.

  - git config --global --sunset user.name - desativa o user name do git.
  - git config --global --user.name "......"
  -  git config --global --user.emails "......"
  - git pull origin master - para resolver conflitos de merge. quando o código do GitHub esta diferente do da sua máquina, mas com uma data mais atual.( outra pessoa editou)
  - git clone "endereço"
  - git remote -v: mostra para onde o repositório está apontado
