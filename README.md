## Do que você vai precisar
Ferramentas necessárias:  
* Do Node instalado na sua máquina  
* Instalar o typescript usando o npm (npm install -g typescript)
    * É interessante que ele seja instalado de forma global, para que o usuário possa usar a biblioteca a qualquer momento e em qualquer projeto para fazer testes rápidos com o TS.
* De uma IDE como o visual studio code  

## Estrutura do repositório 
* *src* 
    * Contém arquivos com exemplos de uso de TS e JS comentados para facilitar o entendimento da ferramenta
* *desafios*
    * Contém vários arquivos JS que podem ser refatorados para solidificar o conhecimento adquirido na aula
* *index.html*
    * É onde está a chamada para o arquivo app.js e pode ser manipulado a vontade para testarem seus scripts
* *tsconfig.json*
    * O coração do TS que configura suas funcionalidades.  
* *package.json*
    * Nesse arquivo foram colocados alguns scripts com o propósito de facilitar a vida de quem usar esse repositório
        * start
            * Inicia o *lite-server*, que vai escutar modificações no index.html e em seus arquivos importados. É útil caso queira fazer testes no browser. A porta disposta normalmente é a *localhost:3000*
        * watch  
            * Roda o *tsc --watch* com o propósito de compilar constantemente qualquer coisa que for editada nos arquivos TS para sua contraparte em JS. Esse comando evita que *tsc* tenha que ser digitado constantemente para fazer a compilação.  

## Sobre como testar 
* Teste mão livre
    * Faça suas alterações em src/app.ts
    * Rode *tsc* ou *npm watch* para compilar elas para o arquivo dist/app.js
    * Caso queira fazer um teste interagindo com o DOM, altere o index.html
    * Rode o npm start e acesse o localhost:3000
* Testar algum dos arquivos da pasta de exemplos ou desafios
    * Copie e cole o conteúdo para o arquivo src/app.ts ou altere o caminho do atributo src da tag script no index.html  
        * ex : *src=dist/app.js* -> *src=dist/exemplos/any.js*
    * Rode *tsc* ou *npm watch* para compilar elas para o arquivo dist/app.js
    * Caso queira fazer um teste interagindo com o DOM, altere o index.html
    * Rode o npm start e acesse o localhost:3000 
Caso queira fazer testes usando html é só alterar o index.html.
 