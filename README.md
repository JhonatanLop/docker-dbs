# Conexão com Banco de Dados usando Docker-compose

Este repositório contém exemplos de como estabelecer conexões com bancos de dados utilizando o Docker-compose. O Docker-compose é uma ferramenta que permite definir e executar aplicativos multi-container Docker de forma fácil e rápida.

## SGDBs suportados

Os seguintes SGDBs são suportados neste repositório:

- Oracle XE (versão oracle-xe-11g)

## Vantagens de usar o Docker para conexão com banco de dados

- **Portabilidade**: Com o Docker, você pode empacotar seu aplicativo juntamente com todas as suas dependências, incluindo o banco de dados, em um contêiner. Isso torna o processo de implantação e execução do aplicativo consistente em diferentes ambientes.

- **Isolamento**: Cada contêiner Docker é isolado, o que significa que você pode executar várias instâncias do mesmo SGDB ou diferentes SGDBs em um único host sem conflitos.

- **Reprodutibilidade**: Com o Docker-compose, você pode definir a configuração do seu ambiente de desenvolvimento em um arquivo YAML. Isso permite que você compartilhe facilmente a configuração com outros desenvolvedores, garantindo que todos tenham o mesmo ambiente de desenvolvimento.

## Requisitos do sistema

Certifique-se de ter os seguintes requisitos instalados em seu sistema:

- Docker: [Instalação do Docker](https://docs.docker.com/get-docker/)
- Docker-compose: [Instalação do Docker-compose](https://docs.docker.com/compose/install/)

## Como executar?

Siga as etapas abaixo para executar um contêiner usando o Docker-compose:

1. Clone este repositório em sua máquina local:

    ```bash
    git clone https://github.com/JhonatanLop/docker-dbs.git
    ```

2. Navegue até o diretório do projeto:

    ```bash
    cd docker-dbs/oracle
    ```

3. Execute o comando abaixo para iniciar o contêiner:

    ```bash
    docker-compose up -d
    ```

Isso iniciará o contêiner em segundo plano. Você pode verificar o status do contêiner usando o comando `docker ps`.

Também é possivel iniciar uma conexão e trabalhar no banco de dados via terminal ou usando SQL Developer, Dbeaver ou qualquer outro sistema

4. Para parar o contêiner, execute o comando:

    ```bash
    docker-compose down
    ```

Isso encerrará o contêiner e removerá todos os recursos associados a ele.

## Contribuindo

Se você quiser contribuir para este projeto, sinta-se à vontade para abrir uma issue ou enviar um pull request.