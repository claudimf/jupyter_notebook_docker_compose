# Jupyter Notebook + Docker Compose

👋 Olá, Seja Bem-vindo(a) ao 'Jupyter Notebook + Docker Compose'.

## Sobre o projeto:

Esse projeto tem como objetivo mostrar como subir o Jupyter Notebook em um contêiner Docker.

### Permissões de arquivos:

Ao se criar arquivos dentro do contâiner Docker o proprietário para edição se torna o contêiner, sendo assim você precisará rodar o comando abaixo para alterar essas permissões e você poder editar:

```sh
sudo chown -R $USER:$USER .
```

# Exigências

**:warning: Atenção:** É necessário que os desenvolvedores usem o Docker no seu ambiente de desenvolvimento.

- **🛠 Modo Desenvolvimento Docker**
    - :computer: [Linux Ubuntu LTS](https://ubuntu.com/download/desktop)
    - 🐳 [Docker](https://docs.docker.com/engine/installation/) Deve estar instalado.
    - 🐳 [Docker Compose](https://docs.docker.com/compose/) Deve estar instalado.
    - **💡 Dica:** [Documentação do Docker](https://docs.docker.com/)

# Instalando

## 🐳 Modo Desenvolvimento com Docker

Após instalar o docker e docker-compose, estando na pasta raiz do projeto, execute:

```sh
docker-compose up
```

Para se certificar que os seus containers subiram corretamente, todos os containers deve estar com o status `UP`, execute:

```sh
docker-compose ps -a
```

Para acessar o container da aplicação, execute:

```sh
docker-compose run --rm jupyter bash
```

Para derrubar e subir a instância do docker novamente, execute:

```sh
docker-compose down && docker-compose up
```

🚀 :clap: Para visualizar o sistema basta acessar no navegador no endereço:   
[localhost:8888](localhost:8888)

# Referências utilizadas

[1° How and why to put your Jupyter notebooks in Docker containers](https://github.com/austinbrian/jupydocker)

[2° How to Put Jupyter Notebooks in a Dockerfile](https://u.group/thinking/how-to-put-jupyter-notebooks-in-a-dockerfile/)

[3° Jupyter Docker Stacks](https://github.com/jupyter/docker-stacks)