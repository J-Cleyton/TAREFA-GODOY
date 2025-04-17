# TAREFA-GODOY
Lição de casa Godoy
---

## Descrição
API para upload de imagens, com funções GET, INPUT e DELETE. Destinado a estudo e aprendizado.

## Instalação
1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/tarefa-godoy.git
   ```
2. Para acessar a API navegue até o diretório do projeto:
   ```bash
   cd tarefa-godoy
   ```
3. Instale as dependências:
   ```bash
   npm install
   ```

## Configuração
Criado um arquivo `.env` na raiz do projeto com as seguintes variáveis:
```
DB_USER=johnneycleyton
DB_PASS=####
PORT=4000
```

## Como Usar
### Iniciar o servidor
```bash
npm start
```
### Endpoints
- **GET /pictures**: Retorna todas as imagens.
- **POST /pictures**: Faz o upload de uma nova imagem.
- **GET /pictures/:id/image**: Retorna uma imagem específica pelo ID.
- **DELETE /pictures/:id**: Deleta uma imagem pelo ID.
- **PUT /pictures/:id**: Atualiza uma imagem pelo ID.

### Interface Web
A interface web permite visualizar e gerenciar as imagens. Para acessá-la, abra o arquivo `index.html`, se através do compilador VSCODE, use a extensão LIVE SERVER e abra-o em um navegador. A interface inclui:
- Um botão para adicionar novas fotos.
- Um botão para deletar imagens existentes.
- Um modal para fazer o upload de fotos.
- Uma grade para exibir as fotos carregadas.

Backend

O backend do projeto é construído com Node.js e Express, e utiliza MongoDB para armazenamento de dados. Aqui estão alguns detalhes adicionais:

    Node.js: Plataforma de desenvolvimento que permite a execução de código JavaScript no lado do servidor.
    Express: Framework web para Node.js que facilita a criação de APIs e servidores web.
    Mongoose: Biblioteca de modelagem de dados para MongoDB, que fornece uma interface para interagir com o banco de dados.
    Multer: Middleware para manipulação de multipart/form-data, usado para upload de arquivos.
    dotenv: Carrega variáveis de ambiente de um arquivo .env para a aplicação.

Estrutura de Pastas

    config: Contém a configuração do Multer para upload de arquivos.
    controllers: Contém os controladores que definem a lógica das rotas.
    models: Contém os modelos Mongoose para o MongoDB.
    routes: Contém as definições de rotas da API.
    db.js: Configuração e conexão com o banco de dados MongoDB.
    app.js: Arquivo principal que configura o servidor Express e as rotas.

Frontend

O frontend do projeto é uma interface web simples que permite visualizar e gerenciar as imagens. Aqui estão alguns detalhes adicionais:

    HTML: Estrutura básica da interface web.
    CSS: Estilos para a interface web, incluindo responsividade.
    JavaScript: Lógica para interagir com a API e atualizar a interface web.

### Funcionalidades do Script
O arquivo `script.js` contém a lógica para interagir com a API e atualizar a interface web. As principais funcionalidades incluem:
- **fetchPhotos**: Busca as fotos da API e as exibe na grade.
- **uploadNewPhoto**: Envia uma nova foto para a API.
- **deletePhoto**: Deleta uma foto da API.
- **showNotification**: Mostra notificações temporárias para o usuário.
- **openUploadModal** e **closeUploadModal**: Abrem e fecham o modal de upload.
- **handleFormSubmit**: Processa o envio do formulário de upload.

### Estilos
O arquivo `style.css` define os estilos para a interface web, incluindo:
- **Reset e Estilos Globais**: Define margens, preenchimentos e fontes padrão.
- **Layout e Containers**: Estiliza o contêiner principal.
- **Cabeçalho**: Estiliza o cabeçalho da página.
- **Botões**: Define estilos para botões primários e de exclusão.
- **Galeria de Fotos**: Estiliza a grade de fotos e os cartões de fotos.
- **Modal de Upload**: Define estilos para o modal de upload.
- **Formulários**: Estiliza os elementos do formulário.
- **Notificações (Toast)**: Define estilos para notificações de sucesso e erro.
- **Responsividade**: Ajusta o layout para dispositivos móveis.

## Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir o issues e enviar um pull requests.

## Licença
Este projeto está licenciado sob os termos da licença MIT. Veja o arquivo LICENÇA nas raiz do projeto para mais detalhes.

---

```
MIT Licença

Copyright (c) 2025 johnney Cleyton

Concede-se, por meio deste, permissão, gratuita, a qualquer pessoa que obtenha uma cópia
deste software e dos arquivos de documentação associados (o "Software"), para lidar
com o Software sem restrições, incluindo, entre outros, os direitos
de usar, copiar, modificar, mesclar, publicar, distribuir, sublicenciar e/ou vender
cópias do Software, e para permitir que as pessoas a quem o Software for
fornecido o façam, sujeito às seguintes condições:

O aviso de direitos autorais acima e este aviso de permissão deverão ser incluídos em todas as
cópias ou partes substanciais do Software.

O SOFTWARE É FORNECIDO "NO ESTADO EM QUE SE ENCONTRA", SEM GARANTIA DE QUALQUER TIPO, EXPRESSA OU
IMPLÍCITA, INCLUINDO, MAS NÃO SE LIMITANDO ÀS GARANTIAS DE COMERCIALIZAÇÃO,
ADEQUAÇÃO A UM DETERMINADO FIM E NÃO VIOLAÇÃO. EM NENHUMA HIPÓTESE OS
AUTORES OU TITULARES DOS DIREITOS AUTORAIS SERÃO RESPONSÁVEIS POR QUALQUER REIVINDICAÇÃO, DANOS OU OUTRA
RESPONSABILIDADE, SEJA EM UMA AÇÃO CONTRATUAL, ATO ILÍCITO OU DE OUTRA FORMA, DECORRENTE DE,
DE OU EM CONEXÃO COM O SOFTWARE OU O USO OU OUTRAS NEGOCIAÇÕES NO
SOFTWARE.
```
