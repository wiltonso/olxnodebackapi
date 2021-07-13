/*
// instalaçoes iniciais
// express-fileupload  para upload de arquivos 
// jimp tratamento de imagens
// cors para receber requisiçoes de todos lugares
npm init -y
npm install express mongose cors dotenv bcrypt express-fileupload jimp uuid
npm install nodemon --dev

No arquivo pakage.json incluir em scripts
"start": "node server.js"
"start-der": "nodemon server.js"


Configura servidor (server.js) e configuracao de ambiente .env


// Planejamento do banco de dados (estrutura)
user (_id, nome, email, state, passwordhash, token)
states (_id, name)

categories ()_id, name, slug)

ads (_id, imagens {url, default}), _iduser, datecreated, state, title, categoria
price, priceNegocitlhe, descriptino, views, status)

Criar a pasta src e subpasta models
Na pasta models, criar os arquivos  das estrutura do db

Criar controlles para controlar os usuarios (processo autenticacao usuario)
UserController.js e AdController.js

Alterar o arquivo route.js (para incluir o require dos contoller criado),
e criar os router necessarios para cada AdController

Criar pasta middlewares e inclui middlewares nas rotas que precisem

Criar validators (processo de validacao de dados para enviar antes do controller)

Existem uma lib para ser utilizada para esta funcao
npm install express-validators

Criar a pasta validators... compativel com controller
AuthValidator



*?