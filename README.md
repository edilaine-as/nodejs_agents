# 🧠 AI-Powered Classroom API

[Leia em Português](#português) | [Read in English](#english)

## English
This is an API developed with Fastify + TypeScript that allows the creation of virtual rooms where users can record class content. The content is transcribed using Google's Gemini 2.5 Flash API and stored as vectors (embeddings) in the database, enabling semantic queries based on user questions.

### 📝 Features
* Create virtual room
* Record and process class
* Ask questions related to the class

### 🧠 How the AI Works
* The class is transcribed using gemini.generativeModel.generateContent(audio).
* After transcription, the text is converted into an embedding.
* When a question is asked, its embedding is compared to those stored in the database (pgvector).
* The most relevant excerpt is sent to Gemini to generate a final response based on the context.

### 🚀 Technologies Used
#### 🧱 Back-end
* Node: Back-End Framework
* Fastify: Web framework
* TypeScript: Static typing for greater robustness
* Zod: Schema validation library with native TypeScript integration
* PostgreSQL: Relational database
* drizzle-orm: ORM for database integration
* pgvector: PostgreSQL extension to store and query embeddings (vectors)
  
#### 🤖 AI & Language Processing
* Gemini API (Google AI)

#### 📦 Package Management & DevTools
* Drizzle Kit: CLI for managing migrations with Drizzle ORM
* Biome: Code linter and formatter
* Ultracite: Defines pre-configurations for Biome

#### 🧪 Other Utilities
* @fastify/multipart: File upload support via multipart/form-data (audio)
* @fastify/cors: Middleware to enable CORS
*fastify-type-provider-zod: Native integration between Fastify and Zod
  
### 📦 Installation
1. Clone the repository:
   ```
   gh repo clone edilaine-as/nodejs_agents
   ```
2. Navigate to the project:
   ```
   cd nodejs_agents
   ```
3. Install dependencies:
   ```
   npm i
   ```
4. Configure the .env file based on .env.example
5. Start the server:
   ```
   npm run dev
   ```
### 🤝 Contribution
Feel free to contribute! Open an issue or submit a pull request
### 📄 License
This project is licensed under the MIT License. See the LICENSE file for more details

## Português
Esta é uma API desenvolvida com Fastify + TypeScript que permite a criação de salas virtuais onde os usuários podem gravar o conteúdo das aulas. O conteúdo é transcrito utilizando a API Gemini 2.5 Flash do Google e armazenado como vetores (embeddings) no banco de dados, permitindo consultas semânticas com base nas perguntas dos usuários.

### 📝 Funcionalidades
* Criar sala virtual
* Gravar e processar uula
* Criar perguntas relacionadas a aula

### 🧠 Como Funciona a IA
- A transcrição da aula é feita com gemini.generativeModel.generateContent(audio).
- Após a transcrição, o texto é convertido para embedding.
- Ao receber uma pergunta, o embedding da pergunta é comparado com os do banco (pgvector)
- O trecho mais relevante é enviado para o Gemini gerar uma resposta final com base no contexto.

### 🚀 Tecnologias Utilizadas
#### 🧱 Back-end
* Node: Framework Back-End
* Fastify: Framework web
* TypeScript: Tipagem estática para maior robustez
* Zod: Biblioteca de validação de esquemas com integração nativa com TypeScript
* PostgreSQL: Banco de dados relacional
* drizzle-orm: ORM para integração com o banco de dados
* pgvector: Extensão do PostgreSQL para armazenar e consultar embeddings (vetores)
  
#### 🤖 IA & Processamento de Linguagem
* Gemini API (Google AI)

#### 📦 Gerenciamento de Pacotes & DevTools
* Drizzle Kit: CLI para gerenciamento de migrações com Drizzle ORM
* Biome: Linter e formatador de código
* Ultracite: Define pré configurações para Biome

#### 🧪 Outros Utilitários
* @fastify/multipart: Suporte a envio de arquivos via multipart/form-data (áudio)
* @fastify/cors: Middleware para habilitar CORS
*fastify-type-provider-zod: Integração nativa entre Fastify e Zod
  
### 📦 Instalação
1. Clone o repositório:
   ```
   gh repo clone edilaine-as/nodejs_agents
   ```
2. Navegue até o projeto
   ```
   cd nodejs_agents
   ```
3. Instale as dependências
   ```
   npm i
   ```
4. Configure o arquivo .env, baseado no arquivo .env.example
5. Inicie o servidor
   ```
   npm run dev
   ```
### 🤝 Contribuição
Sinta-se à vontade para contribuir! Abra uma issue ou envie um pull request.
### 📄 Licença
Este projeto está licenciado sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.
