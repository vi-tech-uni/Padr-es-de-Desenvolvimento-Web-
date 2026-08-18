#definição da imagem
FROM maven:3.9-eclipse-temurin-21-noble

#desabilita a instalação interativa
ENV DEBIAN_FRONTEND=noninteractive

#instala as ferramentas que não existem nas imagens base
#Remove os arquivos temporários provenientes do processo de instalação
#apt-get update - Atualiza o repositório de software
#apt-get install - instala as ferramentas 
#gift-lfs - ferramenta para armazendo de arquivos binários
#curls - ferramenta para testar APIs
#apt-get clean e rm - limpam arquivos temporários 
RUN apt-get update && apt-get install -y \
    mysql-server-8.0 \
    git \
    git-lfs \
    curl \
    unzip \
    zip \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
