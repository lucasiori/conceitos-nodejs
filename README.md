<p align="center">
  <img src="https://github.com/lucasiori/conceitos-nodejs/blob/master/.github/gostack.png" alt="GoStack" width="250" />
</p>

<h1 align="center">Desafio: Conceitos do Node.js</h1>
<p align="center">
  <a href="#sobre-desafio">Sobre</a> &nbsp;&nbsp;|&nbsp;&nbsp;
  <a href="#executando-aplicacao">Executando a aplicação</a> &nbsp;&nbsp;|&nbsp;&nbsp;
  <a href="#rotas-aplicacao">Rotas</a> &nbsp;&nbsp;
  
</p>

<h2 id="sobre-desafio">ℹ Sobre o desafio</h2>

<p>
  Nesse desafio, você deve criar uma aplicação para treinar o que você aprendeu até agora no Node.js!
</p>
<p>
  Essa será uma aplicação para armazenar repositórios do seu portfólio, que irá permitir a criação, listagem, atualização e remoção dos repositórios, 
  e além disso permitir que os repositórios possam receber "likes".
</p>

<br />

<h2 id="executando-aplicacao">✅ Executando a aplicação</h2>

<strong>Requisitos:</strong>
<ul>
  <li>Node.js</li>
  <li>Gerenciador de pacotes: NPM ou Yarn</li>
</ul>

<p>
  Primeiramente, clone o repositório na sua máquina local: <br />
  <code>git clone https://github.com/lucasiori/conceitos-nodejs</code>
</p>

<p>
  Acesse a pasta do projeto, e no terminal execute o comando para instalar as dependências: <br />
  <ul>
    <li>
      <strong>se estiver utilizando NPM: </strong>
      <code>npm install</code>
    </li>
    <li>
      <strong>se estiver utilizando Yarn: </strong>
      <code>yarn</code>
    </li>
  </ul>
</p>

<p>
  Após instaladas as dependências, certifique-se de que a porta <strong>3333</strong> está disponível pois é a porta onde a aplicação será executada. <br />
  Para iniciar o serviço, execute o comando: <br />
  <ul>
    <li>
      <strong>se estiver utilizando NPM: </strong>
      <code>npm dev</code>
    </li>
    <li>
      <strong>se estiver utilizando Yarn: </strong>
      <code>yarn dev</code>
    </li>
  </ul>
</p>

<br />

<h2 id="rotas-aplicacao">🔀 Rotas da aplicação</h2>

<h3>🔵 GET</h3>

<p>
  <strong>Rota:</strong> /repositories <br />
  <strong>Descrição:</strong> Retorna a lista de repositórios cadastrados. <br />
</p>

<br />

<h3>🟢 POST</h3>

<p>
  <strong>Rota:</strong> /repositories <br />
  <strong>Descrição:</strong> Cadastra um novo repositório. <br />
  <strong>Corpo da Requisição: </strong> Objeto JSON contendo título, url e tecnologias do repositório.
  <pre>
    {
      title: "Repositório 1",
      url: "https://github.com/lucasiori/repositorio1",
      techs: ["Node.js", "Typescript"]
    }
  </pre>
</p>
<br />
<p>
  <strong>Rota:</strong> /repositories/:id_repositorio/like <br />
  <strong>Descrição:</strong> Adiciona um like ao repositório. <br />
</p>

<br />

<h3>🟡 PUT</h3>

<p>
  <strong>Rota:</strong> /repositories/:id_repositorio <br />
  <strong>Descrição:</strong> Edita os dados do repositório. <br />
  <strong>Corpo da Requisição: </strong> Objeto JSON contendo título, url e tecnologias do repositório.
  <pre>
    {
      title: "Repositório 1",
      url: "https://github.com/lucasiori/repositorio1",
      techs: ["Node.js", "Typescript"]
    }
  </pre>
</p>

<br />

<h3>🔴 DELETE</h3>

<p>
  <strong>Rota:</strong> /repositories/:id_repositorio <br />
  <strong>Descrição:</strong> Delete o registro do repositório.
</p>
