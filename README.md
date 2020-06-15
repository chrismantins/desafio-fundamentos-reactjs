<img alt="GoStack" src="https://storage.googleapis.com/golden-wind/bootcamp-gostack/header-desafios.png" />

<h3 align="center">
  Desafio 07: GoFinances Web
</h3>

<blockquote align="center">“Não espere resultados brilhantes se suas metas não forem claras”!</blockquote>

<p align="center">
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/chrismantinsdev/desafio-fundamentos-reactjs?color=%2304D361">

  <img alt="License" src="https://img.shields.io/badge/license-MIT-%2304D361">
</p>

<p align="center">
  <a href="#rocket-sobre-o-desafio">Sobre o desafio</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-licença">Licença</a>
</p>

## :rocket: Sobre o desafio

Nesse desafio, foi desenvolvido a aplicação de gestão de transações, a GoFinances. Sendo praticado o que foi aprendido até agora no React.js junto com TypeScript, utilizando rotas e envio de arquivos por formulário.

Essa será uma aplicação dependo do backend desenvolvido no [Desafio 06 - Fundamentos de NodeJs com TypeORM e Multer](https://github.com/chrismantinsdev/desafio-fundamentos-nodejs-typeorm-multer), para exibir as transações criadas e permitir a importação de um arquivo CSV para gerar novos registros no banco de dados.

### Preparando o backend

Antes de tudo é nescessário a instalação e configuração do backend.

- Primeiro de `git clone https://github.com/chrismantinsdev/desafio-fundamentos-nodejs-typeorm-multer.git` para clonar o repositório do backend.

- Depois encontre o arquivo `ormconfig.json` na raíz do projeto e adicione as suas configurações do banco de dados, no caso o que está sendo utilizado é o banco **`PostgreSQL`**.

- Utilize o comando `yarn` ou `npm install` na raiz do projeto para baixar todas as depêndencias.

- Utilize o comando `yarn typeorm migration:run` que fará toda criação das tabelas nessesárias no banco de dados.

- **`PRONTO`**, seu banco já está configurado e e a API já está pronta para ser utilizada.

### Layout da aplicação

O layout pode ser acessado através da página do Figma, no [seguinte link](https://www.figma.com/file/EgOhyj1Inz14dhWGVhRlhr/GoFinances?node-id=1%3A863).

Você precisará uma conta (gratuita) no Figma pra inspecionar o layout e obter detalhes de cores, tamanhos, etc.

### Funcionalidades da aplicação

- **`Listar as transações da sua API`**: Sua página `Dashboard` deve ser capaz de exibir uma listagem através de uma tabela, com o campo `title`, `value`, `type` e `category` de todas as transações que estão cadastradas na sua API.

- **`Exibir o balance da sua API`**: Sua página `Dashboard`, você deve exibir o balance que é retornado do seu backend, contendo o total geral, junto ao total de entradas e saídas.

- **`Importar arquivos CSV`**: Na sua página `Import`, você deve permitir o envio de um arquivo no formato `csv` para o seu backend, que irá fazer a importação das transações para o seu banco de dados. O arquivo csv deve seguir o seguinte [modelo](https://github.com/chrismantinsdev/desafio-fundamentos-reactjs/assets/file.csv).

### Específicação dos testes

Em cada teste, tem uma breve descrição no que sua aplicação deve cumprir para que o teste passe.

Para esse desafio, temos os seguintes testes:

- **`should be able to list the total balance inside the cards`**: Para que esse teste passe, sua aplicação deve permitir que seja exibido na sua Dashboard, cards contendo o total de `income`, `outcome` e o total da subtração de `income - outcome` que são retornados pelo balance do seu backend.

* **`should be able to list the transactions`**: Para que esse teste passe, sua aplicação deve permitir que sejam listados dentro de uma tabela, toda as transações que são retornadas do seu backend.

- **`should be able to navigate to the import page`**: Para que esse teste passe, você deve permitir a troca de página através do Header, pelo botão que contém o nome `Importar`.

- **`should be able to upload a file`**: Para que esse teste passe, você deve permitir que um arquivo seja enviado através do componente de drag-n-drop na página de `import`, e que seja possível exibir o nome do arquivo enviado para o input.

## :memo: Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

Feito com :purple_heart: by Christian | Rocketseat :wave: [Entre na nossa comunidade!](https://discordapp.com/invite/gCRAFhc)
