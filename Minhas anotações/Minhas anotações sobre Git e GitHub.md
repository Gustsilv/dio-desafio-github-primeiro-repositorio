# Minhas anotações

### Fundamentos do GIt:

- SHA1
- É um algoritmo de Hash Seguro, é um conjunto de funções hash criptográficas projetas pela Agência de Segurança Nacional dos EUA.
- A encriptação gera conjunto de chacacteres identificados de 40 dígitos.

> É uma forma de representar um arquivo. ex: openssl sha1 Estudos.txt SHA1(Estudos.txt)= 4f3ada89f71ff524b3f3d92b94d71f5232b430d0

- Objetos fundamentais
- Sistema distribuído
- Segurança

### Objetos fundamentais - Objetos internos

São Meta-dados

- BLOBS (Bolhas)
- TIpo do objeto
- Tamanho da String/arquivo
- o Zero "0"
- O conteúdo do arquivo
- Possui meta-dados
- TREES - é uma crescente
- Armazenam BLOBS "Bloco básico de composição"
- Aponta para tipos de blobs diferentes
- Aponta para COMMITS
- Também armazena meta-dados
- Armazena o tamanho do arquivo
- São responsáveis por montar toda estrutura dos arquivos
- COMMITS
- Objeto que vai dar sentido e responsável por juntar tudo
- Aponta para Tree
- Aponta para um parente (último COMMIT antes dele)

> Com isso é possível criar um linha do tempo de modificações o que trás mais segurança.

- Aponta aponta para o autor (o responsável pelo COMMIT)
- Aponta para uma mensagem (sentido)

> O SHA1 desse COMMIT é o hash de toda essa informação

Sistema distribuido e Seguro

> foi projetado para trazer mais segurança por meio da distribuição de versões de código que são compartilhadas entre a comunidade, então mesmo que ocorra a perda total do código original ainda terão as outras versões que também são confiáveis.



### Chaves SSH

As chaves SSH são uma forma segura de autenticação que permite acessar repositórios remotos no Git sem precisar digitar sua senha toda vez que fizer uma operação remota. Para autenticar sua chave SSH no Git, siga os seguintes passos:

1. Abra o terminal e digite o comando `ssh-keygen`.
2. Pressione Enter para aceitar o local padrão do arquivo da chave e escolha uma senha forte.
3. Copie o conteúdo da chave pública gerada, normalmente localizada em `~/.ssh/id_rsa.pub`.
4. Acesse as configurações de sua conta no Github ou no servidor remoto que deseja autenticar e adicione a chave SSH copiada.

Lembre-se de manter suas chaves SSH em segurança, pois elas permitem acesso a recursos importantes em sua conta do Github ou servidor remoto.

Aqui está um passo a passo sobre como criar e configurar sua chave SSH no terminal Git Bash:

1. Abra o Git Bash e digite o comando `ssh-keygen -t rsa -b 4096 -C "seu-email@example.com"`.
2. Pressione Enter para aceitar o local padrão do arquivo da chave e escolha uma senha forte.
3. Adicione a chave SSH ao agente SSH usando o comando `eval "$(ssh-agent -s)"` e depois `ssh-add ~/.ssh/id_rsa`.
4. Copie o conteúdo da chave pública gerada, normalmente localizada em `~/.ssh/id_rsa.pub`, usando o comando `cat ~/.ssh/id_rsa.pub`.
5. Acesse as configurações de sua conta no Github ou no servidor remoto que deseja autenticar e adicione a chave SSH copiada.

Lembre-se de manter suas chaves SSH em segurança, pois elas permitem acesso a recursos importantes em sua conta do Github ou servidor remoto.

## Tokens de Acesso

Os Tokens de Acesso são chaves de autenticação que podem ser utilizadas para acessar recursos específicos em uma conta do Github sem precisar digitar a senha do usuário. Para autenticar um Token de Acesso no Git, siga os seguintes passos:

1. Acesse as configurações de sua conta no Github e gere um novo Token de Acesso.
2. Copie o Token gerado.
3. No terminal, digite o comando `git config --global credential.helper store`.
4. Em seguida, digite `git push` e forneça suas credenciais de acesso.
5. O Git irá armazenar suas credenciais de acesso em um arquivo de texto.

Lembre-se de manter suas chaves SSH e Tokens de Acesso em segurança, pois elas permitem acesso a recursos importantes em sua conta do Github ou servidor remoto.

Com essas informações, você já pode autenticar suas chaves SSH e Tokens de Acesso no Git e Github de forma segura e eficiente.



### Iniciando o Git e criando um commit

O Git é uma ferramenta de controle de versão muito utilizada por desenvolvedores de software. Para começar a utilizar o Git em um projeto, é necessário seguir alguns passos iniciais.

## Comando git init

O primeiro passo é criar um repositório Git. Para isso, basta executar o comando `git init` no diretório do projeto. Esse comando irá criar um diretório oculto chamado ".git", que irá armazenar todas as informações do repositório.

## Comando git add

Após criar o repositório, é necessário adicionar os arquivos que serão versionados. Para isso, utiliza-se o comando `git add`. Esse comando adiciona os arquivos ao "index", que é uma área temporária do Git onde os arquivos são preparados para serem commitados.

## Comando git commit

O último passo é criar um commit. O commit é uma snapshot do estado atual dos arquivos adicionados ao index. Para criar um commit, utiliza-se o comando `git commit`. É importante informar uma mensagem descritiva para o commit, que deve resumir as alterações realizadas.

Esses são os primeiros comandos básicos do Git. Com eles, é possível iniciar um projeto e começar a versionar os arquivos. Há muitos outros comandos disponíveis no Git para controle de versão, mas esses são os mais utilizados no início de um projeto.

Segue uma lista de comandos básicos para navegação e criação de pastas no Git:

- `cd`: navega para o diretório especificado
- `ls`: lista os arquivos e pastas no diretório atual
- `mkdir`: cria uma nova pasta no diretório atual
- `touch`: cria um novo arquivo no diretório atual
- `pwd`: mostra o caminho completo do diretório atual

Esses comandos são executados no terminal do Git, assim como os comandos `git init`, `git add` e `git commit`, que são utilizados para controle de versão.