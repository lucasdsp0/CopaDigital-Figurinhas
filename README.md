<!-- README preenchido para o projeto FigurinhasCopa Digital -->

<a href="https://classroom.github.com/online_ide?assignment_repo_id=99999999&assignment_repo_type=AssignmentRepo"><img src="https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg" width="200"/></a> <a href="https://classroom.github.com/open-in-codespaces?assignment_repo_id=99999999"><img src="https://classroom.github.com/assets/launch-codespace-2972f46106e565e64193e422d61a12cf1da4916b45550586e14ef0a7c637dd04.svg" width="250"/></a>

---

# ⚽ CopaDigital - Figurinhas 🃏

> [!NOTE]
> Plataforma B2C de colecionamento e troca de figurinhas digitais da Copa do Mundo. Compre pacotes, descubra figurinhas raras e lendárias, complete seu álbum virtual e negocie repetidas com outros colecionadores em um marketplace integrado.

<table>
  <tr>
    <td width="800px">
      <div align="justify">
        O <b>CopaDigital - Figurinhas</b> reimagina a tradição centenária de colecionar figurinhas da Copa do Mundo em formato 100% digital. A plataforma permite que fãs de todo o Brasil comprem pacotes de figurinhas digitais, descubram cartas com diferentes raridades — Comum, Rara, Lendária e Brilhante — colem no álbum virtual e participem de um <i>marketplace</i> onde podem trocar ou vender figurinhas repetidas para outros colecionadores. Com sistema de <b>ranking</b>, <b>conquistas desbloqueáveis</b> e <b>notificações em tempo real</b> via WebSocket, o CopaDigital - Figurinhas oferece uma experiência social e competitiva que vai muito além do simples colecionamento. O projeto foi desenvolvido como trabalho acadêmico na disciplina de <b>Projeto de Software</b> da PUC Minas, modelando uma aplicação B2C completa com arquitetura de microsserviços sobre infraestrutura AWS.
      </div>
    </td>
    <td>
      <div align="center">
        ⚽🃏
        <br/>
        <b>CopaDigital</b>
        <br/>
        <i>Digital</i>
      </div>
    </td>
  </tr>
</table>

---

## 🚧 Status do Projeto

[![Versão](https://img.shields.io/badge/Versão-v1.0.0-blue?style=for-the-badge)](https://github.com/)
[![Licença](https://img.shields.io/badge/Licença-MIT-007ec6?style=for-the-badge&logo=opensourceinitiative)](./LICENSE)
![Node.js](https://img.shields.io/badge/Node.js-20.x-007ec6?style=for-the-badge&logo=node.js&logoColor=white)
![React](https://img.shields.io/badge/React-18.x-007ec6?style=for-the-badge&logo=react&logoColor=white)
![React Native](https://img.shields.io/badge/React_Native-0.74-007ec6?style=for-the-badge&logo=react&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-15-007ec6?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-7.x-007ec6?style=for-the-badge&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-24.x-007ec6?style=for-the-badge&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-ECS%20%7C%20RDS%20%7C%20S3-007ec6?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-5.x-007ec6?style=for-the-badge&logo=prisma&logoColor=white)

---

## 📚 Índice
- [Links Úteis](#-links-úteis)
- [Sobre o Projeto](#-sobre-o-projeto)
- [Funcionalidades Principais](#-funcionalidades-principais)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Arquitetura](#-arquitetura)
  - [Exemplos de diagramas](#exemplos-de-diagramas)
- [Instalação e Execução](#-instalação-e-execução)
  - [Pré-requisitos](#pré-requisitos)
  - [Variáveis de Ambiente](#-variáveis-de-ambiente)
     - [1 Back-end (Node.js)](#1-back-end-nodejs)
     - [2 Front-end (React, Vite)](#2-front-end-react-vite)
     - [3 Exemplos de Variáveis de Ambiente na Vercel](#3-exemplos-de-variáveis-de-ambiente-na-vercel)
  - [Instalação de Dependências](#-instalação-de-dependências)
    - [Front-end (React)](#front-end-react)
    - [Back-end (Node.js)](#back-end-nodejs)
  - [Inicialização do Banco de Dados (PostgreSQL)](#-inicialização-do-banco-de-dados-postgresql)
  - [Como Executar a Aplicação](#-como-executar-a-aplicação)
    - [Terminal 1: Back-end (Node.js)](#terminal-1-back-end-nodejs)
    - [Terminal 2: Front-end (React, Vite)](#terminal-2-front-end-react-vite)
    - [Execução Local Completa com Docker Compose](#-execução-local-completa-com-docker-compose-incluindo-banco-de-dados)
    - [Passos para build, inicialização e execução](#-passos-para-build-inicialização-e-execução)
- [Deploy](#-deploy)
- [Estrutura de Pastas](#-estrutura-de-pastas)
- [Demonstração](#-demonstração)
  - [Aplicativo Mobile](#-aplicativo-mobile)
  - [Aplicação Web](#-aplicação-web)
  - [Exemplo de saída no Terminal (para Back-end, API, CLI)](#-exemplo-de-saída-no-terminal-para-back-end-api-cli)
- [Testes](#-testes)
- [Documentações utilizadas](#-documentações-utilizadas)
- [Autores](#-autores)
- [Contribuição](#-contribuição)
- [Agradecimentos](#-agradecimentos)
- [Licença](#-licença)

---

## 🔗 Links Úteis
* 🌐 **Demo Online:** [Acesse a Aplicação Web](https://figurinhascopa.vercel.app)
  > 💻 **Descrição:** Aplicação hospedada na Vercel (Front-end React) com API no AWS ECS.
* 📱 **Download Mobile:** [App Store](#) | [Google Play](#) | [APK Direto](#)
  > 📱 **Descrição:** Aplicativo React Native disponível para iOS e Android. APK direto disponível para testes no Android.
* 📖 **Documentação:** [Swagger / OpenAPI](https://api.figurinhascopa.com/docs)
  > 📚 **Descrição:** Documentação interativa de todos os endpoints REST da API. Também disponível localmente em `http://localhost:3000/api/docs` após subir o back-end.

---

## 📝 Sobre o Projeto

A paixão por figurinhas da Copa do Mundo une gerações de brasileiros, mas o formato físico apresenta limitações sérias: disponibilidade geográfica restrita, deterioração das cartas ao longo do tempo e grande dificuldade de encontrar figurinhas específicas para completar o álbum.

**Por que ele existe:** O projeto nasceu da vontade de digitalizar essa experiência cultural, eliminando as barreiras físicas e criando um ecossistema onde qualquer fã, em qualquer lugar do Brasil, possa colecionar, trocar e vender figurinhas de forma segura e divertida.

**Qual problema ele resolve:** Centraliza em uma única plataforma a compra de pacotes com sorteio justo por raridade, o gerenciamento do álbum digital com progresso visual, e um marketplace de trocas e vendas entre usuários com transferência atômica garantida.

**Contexto:** Projeto acadêmico desenvolvido na disciplina de **Projeto de Software** — PUC Minas 2026, modelando uma aplicação B2C completa com foco em arquitetura de microsserviços, diagramação UML e boas práticas de engenharia de software.

**Onde pode ser utilizado:** Qualquer evento esportivo de grande escala que envolva colecionamento de figurinhas — Copa do Mundo, Olimpíadas, campeonatos nacionais — pode se beneficiar da arquitetura e dos padrões aqui definidos.

> [!NOTE]
> Este projeto cobre a fase de **arquitetura e diagramação** (não inclui código-fonte implementado). Todos os diagramas foram gerados com PlantUML e estão disponíveis na pasta `/diagramas`.

---

## ✨ Funcionalidades Principais

- 🔐 **Autenticação Segura:** Cadastro com confirmação por e-mail, Login com JWT (access + refresh token) e Recuperação de Senha com link temporário.
- 📗 **Álbum Digital Interativo:** Visualização do álbum com progresso percentual, filtros por status (faltando / repetidas / coladas) e animação ao colar figurinha.
- 🎁 **Pacotes com Sistema de Raridade:** Sorteio com pesos por raridade — Comum 60%, Rara 25%, Lendária 10%, Brilhante 5% — garantindo experiência justa e emocionante.
- 🔄 **Marketplace de Trocas:** Publicação de ofertas, envio de propostas entre usuários e transferência atômica (ACID) das figurinhas ao aceitar uma troca.
- 💰 **Venda de Figurinhas Avulsas:** Precificação com sugestão de preço baseada no histórico de mercado, anúncio público e compra com pagamento integrado.
- 🏆 **Ranking e Conquistas:** Placar global e entre amigos, badges desbloqueáveis por marcos (25%, 50%, 100% do álbum, primeira lendária, etc.).
- 📲 **Compartilhamento Social:** Geração automática de imagem da conquista para compartilhar no Instagram e X (Twitter).
- 🔔 **Notificações em Tempo Real:** WebSocket (Socket.io) para notificações instantâneas + Push Notifications via Firebase FCM + E-mails transacionais via SendGrid.
- 🛠️ **Painel Administrativo:** Gerenciamento do catálogo de figurinhas, moderação de usuários com registro de auditoria e relatórios de vendas exportáveis em PDF.

---

## 🛠 Tecnologias Utilizadas

As seguintes ferramentas, frameworks e bibliotecas foram utilizadas na construção deste projeto.

### 💻 Front-end

* **Framework/Biblioteca:** [React 18.x](https://react.dev/)
* **Linguagem:** TypeScript / JavaScript ES6+
* **Estilização:** [Tailwind CSS 3.x](https://tailwindcss.com/)
* **Gerenciamento de Estado:** Context API + React Query
* **Build Tool:** [Vite 5.x](https://vitejs.dev/)
* **WebSocket Client:** [Socket.io Client 4.x](https://socket.io/)
* **HTTP Client:** [Axios 1.x](https://axios-http.com/)

### 🖥️ Back-end

* **Linguagem/Runtime:** [Node.js 20.x](https://nodejs.org/)
* **Framework:** [Express.js 4.x](https://expressjs.com/)
* **WebSocket Servidor:** [Socket.io 4.x](https://socket.io/)
* **ORM:** [Prisma 5.x](https://www.prisma.io/)
* **Banco de Dados:** [PostgreSQL 15](https://www.postgresql.org/) (AWS RDS Multi-AZ)
* **Cache:** [Redis 7.x](https://redis.io/) (AWS ElastiCache)
* **Autenticação:** JWT (jsonwebtoken 9.x) + bcrypt 5.x
* **Validação:** [Zod 3.x](https://zod.dev/)

### 📱 Mobile

* **Framework:** [React Native 0.74](https://reactnative.dev/)
* **Ferramentas:** Expo, Metro Bundler
* **Plataformas:** iOS e Android

### ⚙️ Infraestrutura & DevOps

* **Containerização:** Docker 24.x + Docker Compose 2.x
* **Cloud:** AWS (ECS — orquestração de containers com Auto Scaling, RDS — banco PostgreSQL, S3 — imagens e arquivos, SQS — filas de mensagens, ElastiCache — Redis, CloudFront — CDN, API Gateway — roteamento e rate limiting)
* **CI/CD:** GitHub Actions
* **Integrações externas:** Stripe / PagSeguro (pagamentos), Firebase FCM (push notifications), SendGrid (e-mails), Instagram API / X API (compartilhamento)

---

## 🏗 Arquitetura

O **FigurinhasCopa Digital** adota uma arquitetura de **microsserviços** organizados por domínio de negócio, com comunicação REST síncrona entre o front-end e a API, e comunicação assíncrona via filas SQS entre os serviços internos para operações não críticas (notificações, e-mails, relatórios).

**Visão geral das camadas:**
- **Clientes** (Web React + Mobile React Native) → acessam via HTTPS passando por CDN CloudFront
- **API Gateway** (AWS) → centraliza autenticação JWT, rate limiting e roteamento
- **8 Microsserviços** (Node.js/Express em containers Docker no AWS ECS) → Auth, Album, Loja, Marketplace, Troca, Ranking, Notificação, Admin
- **Camada de dados** → PostgreSQL (RDS), Redis (ElastiCache), S3 (arquivos), SQS (filas)
- **Sistemas externos** → Gateway de Pagamento, Firebase FCM, SendGrid, Redes Sociais

**Padrões de design adotados:**
- **Repository Pattern** — abstração do acesso ao banco via Prisma ORM
- **Service Layer** — regras de negócio isoladas dos controllers
- **DTO (Data Transfer Objects)** — validação e tipagem de entrada/saída com Zod
- **Observer (assíncrono)** — eventos publicados em filas SQS consumidos por workers
- **Cache-Aside** — Redis populado sob demanda com TTL configurado por recurso

**Decisões arquiteturais importantes:**
- Transferências de figurinhas entre usuários são executadas em **transações ACID** no PostgreSQL para garantir consistência
- Notificações em tempo real via **WebSocket persistente** (Socket.io) com fallback para push FCM e e-mail
- Auto Scaling no ECS entre 2 e 10 instâncias baseado em CPU e volume de requisições

### Exemplos de diagramas

Para melhor visualização e entendimento da estrutura do sistema, os diagramas principais estão organizados abaixo.

| Diagrama de Arquitetura | Diagrama de Componentes e Implantação |
| :---: | :---: |
| **C4 — Nível Container** | **Infraestrutura AWS** |
| <img src="diagramas/componentes/ARQ-C4-container.png" alt="Diagrama C4 Container" width="420px"> | <img src="diagramas/componentes/COMP01-componentes-implantacao.png" alt="Diagrama de Componentes AWS" width="420px"> |

| Modelo de Dados | Diagrama de Classes |
| :---: | :---: |
| **Entidade-Relacionamento (ER)** | **Modelo de Domínio** |
| <img src="diagramas/dados/DAT01-modelo-dados.png" alt="Diagrama ER" width="420px"> | <img src="diagramas/classes/CLS01-diagrama-classes.png" alt="Diagrama de Classes" width="420px"> |

| Casos de Uso | Diagrama de Estados |
| :---: | :---: |
| **22 Casos de Uso com include/extend** | **Ciclo de Vida da Figurinha** |
| <img src="diagramas/casos-de-uso/UC-casos-de-uso.png" alt="Diagrama de Casos de Uso" width="420px"> | <img src="diagramas/estados/EST01-ciclo-vida-figurinha.png" alt="Diagrama de Estados" width="420px"> |

---

## 🔧 Instalação e Execução

### Pré-requisitos

* **Node.js:** Versão **20.x** ou superior (necessário para o back-end e front-end)
* **npm** ou **yarn** — gerenciador de pacotes
* **Docker** e **Docker Compose** — altamente recomendados para rodar PostgreSQL e Redis localmente
* **Git**

---

### 🔑 Variáveis de Ambiente

Crie arquivos `.env` específicos para cada parte da aplicação.

#### 1 Back-end (Node.js)

Crie um arquivo **`.env`** na raiz da pasta `/backend`:

| Variável | Descrição | Exemplo |
| :--- | :--- | :--- |
| `PORT` | Porta onde o back-end será executado | `3000` |
| `DATABASE_URL` | URL de conexão com o PostgreSQL (Prisma) | `postgresql://user:password@localhost:5432/figurinhas_copa` |
| `REDIS_URL` | URL de conexão com o Redis | `redis://localhost:6379` |
| `JWT_SECRET` | Chave secreta para assinatura dos tokens JWT | `chave_super_segura_base64` |
| `JWT_EXPIRES_IN` | Tempo de expiração do access token | `7d` |
| `JWT_REFRESH_EXPIRES_IN` | Tempo de expiração do refresh token | `30d` |
| `STRIPE_SECRET_KEY` | Chave secreta do gateway Stripe | `sk_test_...` |
| `SENDGRID_API_KEY` | Chave da API SendGrid para e-mails | `SG....` |
| `EMAIL_FROM` | Remetente padrão dos e-mails transacionais | `noreply@figurinhascopa.com` |
| `FIREBASE_SERVER_KEY` | Chave do servidor Firebase FCM (push) | `AAAA...` |
| `AWS_REGION` | Região AWS dos serviços | `us-east-1` |
| `AWS_S3_BUCKET` | Nome do bucket S3 para imagens | `figurinhas-copa-assets` |
| `AWS_SQS_QUEUE_URL` | URL da fila SQS de notificações | `https://sqs.us-east-1.amazonaws.com/...` |
| `NODE_ENV` | Ambiente de execução | `development` |

#### 2 Front-end (React, Vite)

Crie um arquivo **`.env`** na raiz da pasta `/frontend`:

| Variável | Descrição | Exemplo |
| :--- | :--- | :--- |
| `VITE_API_URL` | URL base da API back-end | `http://localhost:3000/api` |
| `VITE_WS_URL` | URL do servidor WebSocket | `ws://localhost:3001` |
| `VITE_FIREBASE_API_KEY` | Chave de API Firebase (FCM client-side) | `AIzaSy...` |
| `VITE_STRIPE_PUBLIC_KEY` | Chave pública Stripe para checkout | `pk_test_...` |

---

#### 3. Exemplos de Variáveis de Ambiente na Vercel

A Vercel permite configurar variáveis no painel (Project Settings > Environment Variables).

---

##### **Exemplo 1 – Front-end React com API na AWS**

```
VITE_API_URL=https://api.figurinhascopa.com/api
VITE_WS_URL=wss://ws.figurinhascopa.com
```

---

##### **Exemplo 2 – Aplicação Full-stack com banco gerenciado**

```
DATABASE_URL=postgresql://admin:senha@ep-figurinhas.aws.neon.tech:5432/figurinhasdb
JWT_SECRET=uma_chave_muito_longa_e_segura_gerada_com_openssl
REDIS_URL=rediss://default:senha@redis-figurinhas.cache.amazonaws.com:6380
```

---

##### **Exemplo 3 – Integração com APIs externas**

```
STRIPE_SECRET_KEY=sk_live_seu_stripe_key_aqui
SENDGRID_API_KEY=SG.sua_sendgrid_key_aqui
FIREBASE_SERVER_KEY=AAAA_sua_firebase_server_key_aqui
```

---

##### **Exemplo 4 – Front-end Vite com Firebase**

```
VITE_FIREBASE_API_KEY=AIzaSy_sua_key_aqui
VITE_FIREBASE_AUTH_DOMAIN=figurinhascopa.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=figurinhascopa
VITE_STRIPE_PUBLIC_KEY=pk_live_sua_key_aqui
```

> **Obs:** As variáveis em projetos **Vite** precisam começar com `VITE_` para serem incluídas no bundle do front-end. Variáveis sem esse prefixo ficam acessíveis apenas no servidor.

---

Para adicionar essas variáveis na Vercel:
1. Acesse `https://vercel.com/<seu-usuario>/figurinhascopa/settings/environment-variables`
2. Clique em **"Add"** para adicionar cada variável com nome e valor correspondente.

Localmente, crie um arquivo **`.env.local`** dentro da pasta **`frontend`** com o conteúdo acima.

---

### 📦 Instalação de Dependências

Clone o repositório e instale as dependências.

1. **Clone o Repositório:**

```bash
git clone https://github.com/seu-usuario/figurinhas-copa.git
cd figurinhas-copa
```

2. **Instale as Dependências:**

#### Front-end (React)

```bash
cd frontend
npm install
# ou
yarn install
cd ..
```

#### Back-end (Node.js)

```bash
cd backend
npm install
# ou
yarn install
cd ..
```

---

### 💾 Inicialização do Banco de Dados (PostgreSQL)

O projeto utiliza **PostgreSQL 15** gerenciado pelo **Prisma ORM**.

1. **Rode os containers de PostgreSQL e Redis via Docker:**

```bash
docker compose up -d postgres redis
```

2. **Execute as migrations do Prisma:**

```bash
cd backend
npx prisma migrate dev
```

3. **Popular o banco com dados iniciais (catálogo da Copa 2026):**

```bash
npm run seed
```

---

### ⚡ Como Executar a Aplicação

Execute a aplicação em modo de desenvolvimento em **dois terminais separados**.

#### Terminal 1: Back-end (Node.js)

```bash
cd backend
npm run dev
```
🚀 *O Back-end estará disponível em **http://localhost:3000**.*
📖 *Swagger disponível em **http://localhost:3000/api/docs**.*

---

#### Terminal 2: Front-end (React, Vite)

```bash
cd frontend
npm run dev
```
🎨 *O Front-end estará disponível em **http://localhost:5173**.*

---

#### 🐳 Execução Local Completa com Docker Compose (Incluindo Banco de Dados)

Para uma execução local que inclui back-end (Node.js), front-end (React), PostgreSQL e Redis, use o **`docker-compose`**.

Antes de tudo, certifique-se de que o **Docker Desktop** (Mac/Windows) ou o **serviço Docker** (Linux) está em execução.

- **No Linux**: rode o comando abaixo para iniciar o serviço:

```bash
sudo systemctl start docker
```

---

#### 📦 Passos para build, inicialização e execução

1. Acesse a pasta raiz do projeto:

```bash
cd figurinhas-copa
```

2. Suba todos os serviços (back-end, front-end, PostgreSQL e Redis):

```bash
docker compose up --build -d
```

> [!NOTE]
> 💡 O parâmetro `--build` garante que as imagens mais recentes do projeto sejam geradas, e `-d` executa em segundo plano.

3. Verifique se os containers estão rodando:

```bash
docker ps
```

4. Execute as migrations e seed dentro do container do back-end:

```bash
docker exec -it figurinhas-backend npx prisma migrate deploy
docker exec -it figurinhas-backend npm run seed
```

5. Abra no navegador:
   - Front-end: **http://localhost:5173**
   - API: **http://localhost:3000**
   - Swagger: **http://localhost:3000/api/docs**

6. Para parar e remover todos os containers:

```bash
docker compose down
```

✅ **Em resumo:** Usar **`docker compose`** simplifica a execução do ambiente completo, garantindo que PostgreSQL e Redis estejam disponíveis sem instalação manual.

---

## 🚀 Deploy

Instruções para deploy em produção.

1. **Build dos artefatos:**

```bash
# Build do Front-end (React/Vite) — gera a pasta /dist
cd frontend
npm run build

# Build do Back-end (gera imagem Docker)
cd ../backend
docker build -t figurinhas-backend:latest .
```

2. **Configuração do Ambiente de Produção:**

Configure as variáveis de ambiente no seu provedor:
- **Front-end:** Vercel (Project Settings > Environment Variables)
- **Back-end:** AWS ECS Task Definition (environment variables)

> 🔑 **Variáveis Cruciais:** `DATABASE_URL` apontando para o RDS, `REDIS_URL` para o ElastiCache, `JWT_SECRET` com chave segura gerada via `openssl rand -base64 64`, e `VITE_API_URL` com a URL pública da API.

3. **Execução em Produção (AWS ECS):**

```bash
# Push da imagem para o ECR (Elastic Container Registry)
aws ecr get-login-password --region us-east-1 | docker login --username AWS --password-stdin <account>.dkr.ecr.us-east-1.amazonaws.com
docker tag figurinhas-backend:latest <account>.dkr.ecr.us-east-1.amazonaws.com/figurinhas-backend:latest
docker push <account>.dkr.ecr.us-east-1.amazonaws.com/figurinhas-backend:latest

# Atualizar o serviço ECS (força novo deploy)
aws ecs update-service --cluster figurinhas-cluster --service figurinhas-backend --force-new-deployment
```

---

## 📂 Estrutura de Pastas

```
figurinhas-copa/
├── .editorconfig                  # ✍️ Padronização de estilo de código
├── .env.example                   # 🧩 Exemplo de todas as variáveis necessárias (sem valores sensíveis)
├── .gitignore                     # 🧹 Ignora arquivos não versionados (.env, node_modules, etc.)
├── .github/                       # 🤖 CI/CD (GitHub Actions), templates de Issues e PRs
├── README.md                      # 📘 Documentação principal do projeto
├── CONTRIBUTING.md                # 🤝 Guia de contribuição
├── LICENSE                        # ⚖️ Licença MIT do projeto
├── docker-compose.yml             # 🐳 Orquestração dos containers (front/back/postgres/redis)
├── docker-compose.override.yml    # 🐳 Configurações extras apenas para desenvolvimento
│
├── /frontend                      # 📁 Aplicação React (Web)
│   ├── .env.example               # 🧩 Variáveis de ambiente do front-end
│   ├── Dockerfile                 # 🐳 Docker build do front-end
│   ├── vite.config.ts             # ⚙️ Configuração do Vite
│   ├── tailwind.config.ts         # 🎨 Configuração do Tailwind CSS
│   ├── /public                    # 📂 Arquivos estáticos e index.html
│   └── /src                       # 📂 Código-fonte React
│       ├── /components            # 🧱 Componentes reutilizáveis (UI)
│       │   ├── /album             # 📗 Componentes do álbum digital
│       │   ├── /marketplace       # 🛒 Componentes do marketplace
│       │   ├── /figurinha         # 🃏 Cards de figurinhas (raridade, animação)
│       │   └── /shared            # 🔗 Botões, modais, inputs, etc.
│       ├── /pages                 # 📄 Páginas/rotas da aplicação
│       │   ├── Home.tsx
│       │   ├── Album.tsx
│       │   ├── Marketplace.tsx
│       │   ├── Ranking.tsx
│       │   └── Admin/
│       ├── /services              # 🔌 Chamadas HTTP (Axios)
│       ├── /hooks                 # 🎣 Hooks personalizados
│       ├── /store                 # 🗃️ Gerenciamento de estado (Context API)
│       ├── /styles                # 🎨 Estilos globais
│       └── /utils                 # 🛠️ Funções utilitárias
│
├── /backend                       # 📁 Aplicação Node.js (API)
│   ├── .env.example               # 🧩 Variáveis de ambiente do back-end
│   ├── Dockerfile                 # 🐳 Docker build do back-end
│   ├── /src
│   │   ├── /controllers           # 🎮 Endpoints REST (AuthController, AlbumController, etc.)
│   │   ├── /services              # ⚙️ Regras de negócio (AuthService, TrocaService, etc.)
│   │   ├── /repositories          # 🗄️ Acesso ao banco via Prisma ORM
│   │   ├── /models                # 🧬 Tipos e interfaces de domínio
│   │   ├── /dto                   # ✉️ Data Transfer Objects (validação Zod)
│   │   ├── /middleware            # 🛡️ AuthMiddleware (JWT), rate limiting, erros
│   │   ├── /config                # 🔧 Configurações (DB, Redis, S3, SQS)
│   │   ├── /workers               # ⚡ Consumidores das filas SQS
│   │   └── /websocket             # 🔔 Servidor Socket.io
│   ├── /prisma
│   │   ├── schema.prisma          # 🧬 Schema do banco de dados
│   │   ├── seed.ts                # 🌱 Dados iniciais (catálogo da Copa)
│   │   └── /migrations            # 📜 Histórico de migrations
│   ├── /src/tests                 # 🧪 Testes unitários e de integração (Jest)
│   └── package.json               # 📦 Dependências e scripts
│
├── /mobile                        # 📁 Aplicação React Native (iOS/Android)
│   ├── /src
│   │   ├── /screens               # 📱 Telas do aplicativo
│   │   ├── /components            # 🧱 Componentes reutilizáveis
│   │   └── /services              # 🔌 Chamadas HTTP e WebSocket
│   └── package.json
│
├── /diagramas                     # 📊 Código-fonte PlantUML (.puml)
│   ├── /casos-de-uso              # UC-casos-de-uso.puml
│   ├── /sequencia                 # UC01 a UC22 + DSS UC06, UC13, UC14
│   ├── /comunicacao               # COM01, COM02
│   ├── /estados                   # EST01, EST02
│   ├── /componentes               # COMP01, ARQ-C4-container
│   ├── /classes                   # CLS01
│   └── /dados                     # DAT01
│
├── /imagens                       # 🖼️ PNGs gerados dos diagramas PlantUML
│
├── /docs                          # 📚 Documentação de Projeto (Word .docx)
│   └── documentacao-figurinhas-copa.docx
│
└── /tests                         # 🧪 Testes End-to-End (Playwright)
```

---

## 🎥 Demonstração

> [!WARNING]
> Como este é um projeto de diagramação/arquitetura, as telas abaixo são representações conceituais das principais interfaces do sistema. Hospede suas imagens em um CDN ou GitHub Pages para garantir carregamento rápido.

### 📱 Aplicativo Mobile

| Tela | Captura de Tela |
| :---: | :---: |
| **Álbum Digital** | **Abertura de Pacote** |
| <img src="https://joaopauloaramuni.github.io/image/fundo_mobile_engsoft.jpeg" alt="Álbum Digital Mobile" height="300"> | <img src="https://joaopauloaramuni.github.io/image/fundo_mobile_engsoft.jpeg" alt="Abertura de Pacote Mobile" height="300"> |
| _Tela do álbum com progresso visual_ | _Animação de abertura de pacote_ |

### 🌐 Aplicação Web

| Tela | Captura de Tela |
| :---: | :---: |
| **Página Inicial (Home)** | **Marketplace** |
| <img src="https://joaopauloaramuni.github.io/image/aramunilogo.png" alt="Home FigurinhasCopa" width="320px"> | <img src="https://joaopauloaramuni.github.io/image/aramunilogo.png" alt="Marketplace" width="320px"> |
| **Álbum Digital** | **Ranking de Colecionadores** |
| <img src="https://joaopauloaramuni.github.io/image/aramunilogo.png" alt="Álbum Digital" width="320px"> | <img src="https://joaopauloaramuni.github.io/image/aramunilogo.png" alt="Ranking" width="320px"> |
| **Painel Administrativo** | **Abertura de Pacote** |
| <img src="https://joaopauloaramuni.github.io/image/aramunilogo.png" alt="Admin" width="320px"> | <img src="https://joaopauloaramuni.github.io/image/aramunilogo.png" alt="Abertura de Pacote Web" width="320px"> |

### 💻 Exemplo de Saída no Terminal (para Back-end, API, CLI)

#### 1. Demonstração da API (Exemplo com cURL)

```bash
# Abre um pacote de figurinhas do usuário autenticado
curl -X POST 'http://localhost:3000/api/pacotes/abrir' \
     -H 'Authorization: Bearer <seu-jwt-token>' \
     -H 'Content-Type: application/json' \
     -d '{"pacoteId": "a1b2c3d4-e5f6-7890-abcd-ef1234567890"}'
```

**Saída Esperada:**
```json
{
  "sucesso": true,
  "pacoteId": "a1b2c3d4-e5f6-7890-abcd-ef1234567890",
  "figurinhas": [
    { "id": "fig-001", "nome": "Vinicius Jr.", "selecao": "Brasil", "raridade": "LENDARIA", "numero": 11 },
    { "id": "fig-042", "nome": "Rodrigo", "selecao": "Brasil", "raridade": "RARA", "numero": 42 },
    { "id": "fig-078", "nome": "Marquinhos", "selecao": "Brasil", "raridade": "COMUM", "numero": 78 },
    { "id": "fig-113", "nome": "Estádio Maracanã", "selecao": null, "raridade": "COMUM", "numero": 113 },
    { "id": "fig-200", "nome": "Mascote Fuleco", "selecao": null, "raridade": "BRILHANTE", "numero": 200 }
  ]
}
```

---

#### 2. Demonstração de Execução de CLI/Script

```bash
# Executa seed do catálogo completo da Copa 2026
npm run seed
```

**Saída Esperada:**
```text
[INFO]  Conectando ao banco de dados...
[OK]    Conexão estabelecida com PostgreSQL 15.
[INFO]  Limpando dados existentes do catálogo...
[OK]    Catálogo limpo.
[INFO]  Inserindo 32 seleções...
[OK]    32 seleções inseridas.
[INFO]  Inserindo 736 jogadores...
[OK]    736 jogadores inseridos.
[INFO]  Inserindo 640 figurinhas (jogadores + estádios + especiais)...
[OK]    640 figurinhas inseridas.
[SUCCESS] Seed concluído! Total: 32 seleções, 736 jogadores, 640 figurinhas.
Tempo de execução: 3.41s
```

---

## 🧪 Testes

### Testes Unitários e de Integração

Para rodar os testes de unidade e integração:

```bash
cd backend
npm run test
```
*Ferramenta utilizada: Jest + Supertest*

### Cobertura de Testes

```bash
npm run test:coverage
```

**Saída esperada:**
```text
PASS src/services/PacoteService.test.ts
  ✓ deve sortear exatamente 5 figurinhas por pacote (12ms)
  ✓ deve respeitar pesos de raridade na distribuição (8ms)
  ✓ deve marcar pacote como aberto após abertura (5ms)

PASS src/services/TrocaService.test.ts
  ✓ deve criar proposta quando usuário possui a figurinha (9ms)
  ✓ deve transferir figurinhas atomicamente ao aceitar troca (18ms)
  ✓ deve liberar reserva ao recusar proposta (6ms)
  ✓ não deve permitir proposta com figurinha já reservada (4ms)

PASS src/services/AlbumService.test.ts
  ✓ deve calcular progresso correto do álbum (7ms)
  ✓ deve marcar figurinha como colada corretamente (5ms)
  ✓ deve listar somente figurinhas repetidas (6ms)

Test Suites: 12 passed, 12 total
Tests:       67 passed, 67 total
Coverage:    82.4%
Tempo de execução: 8.72s
```

### Testes End-to-End (E2E)

Para rodar os testes de ponta a ponta:

```bash
npm run test:e2e
```
*Ferramenta utilizada: Playwright*

---

## 🔗 Documentações utilizadas

* 📖 **Diagramação UML:** [PlantUML — Documentação Oficial](https://plantuml.com/guide)
* 📖 **Framework (Front-end):** [Documentação Oficial do **React**](https://react.dev/reference/react)
* 📖 **Build Tool (Front-end):** [Guia de Configuração do **Vite**](https://vitejs.dev/config/)
* 📖 **Mobile:** [Documentação Oficial do **React Native**](https://reactnative.dev/docs/getting-started)
* 📖 **Framework (Back-end):** [Documentação Oficial do **Express.js**](https://expressjs.com/en/4x/api.html)
* 📖 **ORM:** [Documentação Oficial do **Prisma**](https://www.prisma.io/docs)
* 📖 **WebSocket:** [Documentação Oficial do **Socket.io**](https://socket.io/docs/v4/)
* 📖 **Containerização:** [Documentação de Referência do **Docker**](https://docs.docker.com/)
* 📖 **Cloud AWS ECS:** [Guia do Desenvolvedor AWS ECS](https://docs.aws.amazon.com/ecs/)
* 📖 **Pagamento:** [Referência de API do **Stripe**](https://stripe.com/docs/api)
* 📖 **Push Notifications:** [Guia do **Firebase FCM**](https://firebase.google.com/docs/cloud-messaging)
* 📖 **Guia de Estilo:** [**Conventional Commits** — Padrão de Mensagens](https://www.conventionalcommits.org/en/v1.0.0/)
* 📖 **Especificação UML 2.5:** [OMG UML Standard](https://www.omg.org/spec/UML/2.5.1/)

---

## 👥 Autores

| 👤 Nome | 🖼️ Foto | :octocat: GitHub | 💼 LinkedIn | 📤 Gmail |
|---------|----------|-----------------|-------------|-----------|
| Seu Nome  | <div align="center"><img src="https://joaopauloaramuni.github.io/image/aramunilogo.png" width="70px" height="70px"></div> | <div align="center"><a href="https://github.com/seu-usuario"><img src="https://joaopauloaramuni.github.io/image/github6.png" width="50px" height="50px"></a></div> | <div align="center"><a href="https://www.linkedin.com/in/seu-usuario"><img src="https://joaopauloaramuni.github.io/image/linkedin2.png" width="50px" height="50px"></a></div> | <div align="center"><a href="mailto:seu-email@gmail.com"><img src="https://joaopauloaramuni.github.io/image/gmail3.png" width="50px" height="50px"></a></div> |

> [!TIP]
> 💡 **Dica:** Substitua os links acima pelo seu GitHub, LinkedIn e Gmail reais. Escolha uma foto profissional de rosto para o perfil.

---

## 🤝 Contribuição

Guia para contribuições ao projeto.

1. Faça um `fork` do projeto.
2. Crie uma branch para sua feature (`git checkout -b feature/minha-feature`).
3. Commit suas mudanças (`git commit -m 'feat: Adiciona nova funcionalidade X'`). **(Utilize [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/))**
4. Faça o `push` para a branch (`git push origin feature/minha-feature`).
5. Abra um **Pull Request (PR)**.

> [!IMPORTANT]
> 📝 **Regras:** Por favor, verifique o arquivo [`CONTRIBUTING.md`](./CONTRIBUTING.md) para detalhes sobre nosso guia de estilo de código e o processo de submissão de PRs.

---

## 🙏 Agradecimentos

Gostaria de agradecer aos seguintes canais e pessoas que foram fundamentais para o desenvolvimento deste projeto:

* [**Engenharia de Software PUC Minas**](https://www.instagram.com/engsoftwarepucminas/) — Pelo apoio institucional, estrutura acadêmica e fomento à inovação e boas práticas de engenharia.
* [**Prof. Dr. João Paulo Aramuni**](https://github.com/joaopauloaramuni) — Pelos valiosos ensinamentos sobre **Arquitetura de Software**, **Padrões de Projeto** e pelo template de documentação que norteou este trabalho.
* [**Fernanda Kipper**](https://www.instagram.com/kipper.dev/) — Pelos ensinamentos em **Desenvolvimento Web**, **DevOps** e melhores práticas em **Front-end**.
* [**Rodrigo Branas**](https://branas.io/) — Pela didática excepcional em **Clean Architecture** e **Clean Code**.
* [**Código Fonte TV**](https://codigofonte.tv/) — Pelo vasto conteúdo e cobertura de tutoriais e apoio à comunidade de **Desenvolvimento Web**.

---

## 📄 Licença

Este projeto é distribuído sob a **[Licença MIT](./LICENSE)**.

---

> Projeto acadêmico — Disciplina: Projeto de Software — PUC Minas — 2026
