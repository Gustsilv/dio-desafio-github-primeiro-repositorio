GitHub

O GitHub é uma plataforma de hospedagem de repositórios Git, que permite que você compartilhe e colabore em projetos com outras pessoas.

Git 

O Git é um sistema de controle de versão distribuído que armazena informações em objetos internos. Existem três tipos de objetos: BLOBS que armazenam conteúdo de arquivos, TREES que armazenam referências a BLOBS e outros TREES, e COMMITS que armazenam informações de autor, mensagem e referências a uma TREE e a um COMMIT pai. Cada objeto é identificado por um hash SHA1, o que permite criar uma linha do tempo de modificações segura. Para criar esses objetos internos, é necessário fornecer seus metadados, como o tipo e tamanho do arquivo, e o conteúdo do arquivo para BLOBS. Em seguida, o objeto TREE é criado com referências aos BLOBS e TREES que compõem a estrutura do arquivo. Por fim, o objeto COMMIT é criado com referência a uma TREE e um COMMIT pai, e informações adicionais de autor e mensagem. O Git é projetado para ser seguro e distribuído, permitindo que várias versões de código sejam compartilhadas e confiáveis entre a comunidade.