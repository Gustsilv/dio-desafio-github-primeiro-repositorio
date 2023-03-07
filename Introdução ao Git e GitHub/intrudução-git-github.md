GitHub

O GitHub � uma plataforma de hospedagem de reposit�rios Git, que permite que voc� compartilhe e colabore em projetos com outras pessoas.

Git 

O Git � um sistema de controle de vers�o distribu�do que armazena informa��es em objetos internos. Existem tr�s tipos de objetos: BLOBS que armazenam conte�do de arquivos, TREES que armazenam refer�ncias a BLOBS e outros TREES, e COMMITS que armazenam informa��es de autor, mensagem e refer�ncias a uma TREE e a um COMMIT pai. Cada objeto � identificado por um hash SHA1, o que permite criar uma linha do tempo de modifica��es segura. Para criar esses objetos internos, � necess�rio fornecer seus metadados, como o tipo e tamanho do arquivo, e o conte�do do arquivo para BLOBS. Em seguida, o objeto TREE � criado com refer�ncias aos BLOBS e TREES que comp�em a estrutura do arquivo. Por fim, o objeto COMMIT � criado com refer�ncia a uma TREE e um COMMIT pai, e informa��es adicionais de autor e mensagem. O Git � projetado para ser seguro e distribu�do, permitindo que v�rias vers�es de c�digo sejam compartilhadas e confi�veis entre a comunidade.