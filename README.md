## 🌐 [English Version of README](README_EN.md)

# Docker para Desenvolvedores (com Docker Swarm e Kubernetes)

Este projeto é um curso completo de Docker, abrangendo desde os conceitos básicos até o uso avançado, incluindo Docker Swarm e Kubernetes. O conteúdo inclui a criação de containers, imagens e o uso de Docker Compose, além de orquestração de containers com Docker Swarm e Kubernetes.

## 🔨 Funcionalidades do Projeto

### Exemplo Visual do Projeto  

Este projeto permite criar e orquestrar containers com Docker, utilizando diferentes métodos de orquestração, como Docker Swarm e Kubernetes. Ele também inclui a criação de redes e volumes, além de um exemplo de integração com o Docker Compose.

## ✔️ Técnicas e Tecnologias Utilizadas

- **Docker**: Containers, Imagens, Volumes, Networks, Bind Mounts.
- **Docker Compose**: Orquestração de múltiplos containers.
- **Docker Swarm**: Orquestração de containers em cluster.
- **Kubernetes**: Orquestração de containers com clusters Kubernetes.
- **YAML**: Definição de configurações para containers e serviços.
- **Flask**: Framework web para exemplos de containers de aplicação.

## 📁 Estrutura do Projeto

- **1_imagens_e_containers/**
  - **Dockerfile**: Arquivo para construção da imagem Docker.
  - **app.js**: Aplicação simples em Node.js.
  - **copia/**: Diretório com uma cópia do arquivo app.js.
  - **package.json**: Dependências do Node.js.
  
- **2_volumes/**
  - **Dockerfile**: Arquivo para construção de imagem com volumes.
  - **index.php**: Exemplo simples de aplicação PHP.
  - **messages/**: Diretório com arquivos de mensagens.
  - **process.php**: Arquivo PHP para processamento de dados.

- **3_networks/**
  - **1_externa/**: Contém exemplo de rede externa no Docker.
  - **2_host/**: Exemplo de rede host.
  - **3_conn_containers/**: Exemplo de containers conectados em rede.

- **4_yaml/**
  - **app.py**: Exemplo de uso de YAML com Flask.
  - **test.yaml**: Arquivo YAML de configuração.

- **5_compose/**
  - **docker-compose.yaml**: Configuração para orquestração com Docker Compose.

- **6_kubernetes/**
  - **Dockerfile**: Arquivo Docker para construção de imagem Kubernetes.
  - **app.py**: Aplicação Flask para execução no Kubernetes.
  - **templates/**: Diretório com arquivos de template HTML para o Kubernetes.

- **7_docker_yt/**
  - **Dockerfile**: Arquivo Docker para aplicação YouTube.
  - **index.js**: Código da aplicação Node.js.
  - **package.json**: Dependências para o projeto Node.js.

- **LICENSE**: Licença do projeto.
- **README.md**: Documentação principal do projeto.
- **README_EN.md**: Documentação em inglês.
- **Slides do curso de Docker.pdf**: Apresentações do curso.

## 🛠️ Abrir e rodar o projeto

Para iniciar o projeto localmente, siga os passos abaixo:

1. **Certifique-se de que o Node.js está instalado**:
   - O [Node.js](https://nodejs.org/) é necessário para rodar o projeto. Você pode verificar se já o tem instalado com:

   ```bash
   node -v
   ```

- Se não estiver instalado, baixe e instale a versão recomendada.

2. **Clone o Repositório**:
    - Copie a URL do repositório e execute o comando abaixo no terminal:

   ```bash
   git clone <URL_DO_REPOSITORIO>
   ```

## 🌐 Deploy

Para fazer o deploy do projeto, você pode utilizar o Docker, Docker Compose ou Kubernetes, conforme descrito nos arquivos de configuração.

### Deploy com Docker

1. Navegue até o diretório do projeto.
2. Construa a imagem Docker:

   ```bash
   docker build -t nome-da-imagem .
   ```

3. Rode o container:

   ```bash
   docker run -p 3000:3000 nome-da-imagem
   ```

### Deploy com Docker Compose

1. Navegue até o diretório `5_compose/`.
2. Crie e inicie os containers com Docker Compose:

   ```bash
   docker-compose up --build
   ```

### Deploy com Kubernetes

1. Navegue até o diretório `6_kubernetes/`.
2. Inicie o serviço Kubernetes:

   ```bash
   kubectl apply -f flask-service.yaml
   ```

3. Acesse o serviço no navegador para visualizar o projeto em execução.
