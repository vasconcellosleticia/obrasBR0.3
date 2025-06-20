🏗️ Obras em Andamento - Backend
API desenvolvida com Node.js para gerenciamento de obras, incluindo cadastro de obras, geolocalização, fotos, usuários e relatórios de fiscalização.

⚙️ Tecnologias Utilizadas
Node.js – Ambiente de execução JavaScript.

Express – Framework web minimalista e flexível.

MongoDB – Banco de dados NoSQL para armazenamento dos dados.

Mongoose – ODM para modelagem de dados no MongoDB.

dotenv – Gerenciamento de variáveis de ambiente.

bcryptjs – Criptografia de senhas.

jsonwebtoken (JWT) – Autenticação baseada em tokens.

Multer – Upload de arquivos (ex: fotos da obra).

PDFKit – Geração de relatórios em PDF.

Cloudinary – Armazenamento de imagens na nuvem.

Cors – Middleware para controle de acesso entre domínios.

📁 Estrutura do Projeto

obras-backend/
├── controllers/         # Lógica dos endpoints
├── db/                  # Conexão com MongoDB
├── models/              # Modelos Mongoose (Obra, Usuario, Fiscalizacao, etc.)
├── middlewares/         # Autenticação, upload, etc.
├── routes/              # Definição de rotas
├── utils/               # Funções utilitárias (ex: assinatura digital, Cloudinary)
├── .env.example         # Exemplo de variáveis de ambiente
├── server.js            # Ponto de entrada da aplicação
├── package.json         # Dependências e scripts

🚀 Como Executar
1. Clone o repositório
git clone (https://github.com/vasconcellosleticia/ObrasBR.git)
cd obras-backend

2. Instale as dependências
npm install

3. Configure as variáveis de ambiente
Crie um arquivo .env com base no .env.example:


PORT=3000
MONGO_URI=mongodb+srv:mongodb+srv://vasconcellosleticia:<db_password>@cluster0.vxqhjd4.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0
JWT_SECRET=M5gcC!7Asvu8b.M
JWT_EXPIRES_IN=1d
CLOUDINARY_URL=cloudinary://652561436585195:ku4i19EjubnZQEe_eY8QqcE9JYo@dntqljhrr

4. Inicie o servidor
npm run dev

A API estará disponível localmente em: http://localhost:3000

✨ Funcionalidades
✅ Cadastro e login de usuários

✅ Autenticação com JWT

✅ Cadastro de obras com geolocalização

✅ Upload de fotos da obra

✅ Cadastro e consulta de fiscalizações

✅ Geração de relatórios em PDF

✅ Controle de acesso por perfil (Admin, Engenheiro, Fiscal, etc.)

