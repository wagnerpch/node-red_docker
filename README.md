# node-red_docker

<h1>Node-RED com MySQL e Docker</h1>

###**Requisitos utilizados:**
- Docker
- WSL do Windows
- Compose

###**A docker compose desse projeto dois containers: Node-RED e MySQL**

###**Passo a passo para clonar o repositório:**

1) Criar pasta
> shell: ```mkdir <nome_da_pasta>```

2) Abrir Terminal (shell) ou VsCode
> shell: ```code .```

3) Clonar o projeto com credencial e senha de rede da Supera
> shell: ```git clone https://code.supera.com.br/wagner.cordeiro/node-red.git```

4) Iniciar container:
> shell: ```docker compose up -d --build```

5) Acessar a aplicação no navegador com http://localhost:1880/

**Importante:**
Para usar o nó MySQL, é necessário obter o número do ip do container para configurar o nó.

Digite o seguinte comando no terminal:

> docker inspect mysqlcompose

Procure a linha "Gateway": "NNN.NN.N.N"

<h3>Objetivo: rodar o Node-RED no container do Docker com MySQL</h3>

O conteúdo dos flows está separado por aulas, pois foi elaborado seguindo as aulas ministradas por CFBCursos, gratuitamente, no canal do Youtube.
Contudo, esse conteúdo não corresponde exatamente ao conteúdo das aulas, algumas mudanças foram feitas, para testar os nodes.

<ul>
    <li>Aula 1 - Utilizar o nó 'inject' e 'debug'</li>
    <li>Aula 2 - Alterando propriedades do nó 'inject'</li>
    <li>Aula 3 - Programar loop de repetição do nó 'inject' e utilização de 'function' com Javascript</li>
    <li>Aula 4 - Adição do nó 'random'</li>
    <li>Aula 5 - Utilizar 'function' para programar saídas diferentes</li>
    <li>Aula 6 e Aula 6 Global - Utilizar variáveis entre 'function' dentro do mesmo flow e com flow diferente</li>
    <li>Aula 7 - Selecionando elemento do array do payload</li>
    <li>Aula 8 - Usando o nó 'switch' para programar saídas diferentes</li>
    <li>Aula 9 - Usando o nó 'template' e handlebars</li>
    <li>Aula 10 - Usando o nó 'range' para mudar o número dentro de um determinado intervalo</li>
    <li>Aula 11 - Usando o nó 'delay' para atrasar o disparo do fluxo</li>
    <li>Aula 12 - Usando o nó 'trigger' para disparar automaticamente e utilizar o nó inject com valor (1) para iniciar o trigger e (-1) para desligar o mesmo</li>
    <li>Aula 13 - Usando o nó 'http in' com parâmetro 'get' para acessar o conteúdo via endpoint</li>
    <li>Aula 14 - Usando o nó 'http in' com parâmetro 'get' para acessar o conteúdo via endpoint e utilizar 'function' para trabalhar com query string (exemplo: msg.req.query.curso)</li>
    <li>Aula 15 - Utilizando handlebars no nó 'template' (exemplo: <i>Nome: {{req.params.nome}}</i>)</li>
    <li>Aula 16 - Usar o nó 'change' para guardar valor como variável do fluxo, para ser recuperado por outro processo dentro do mesmo fluxo com 'http in' via 'get' com o nó 'change'</li>
    <li>Aula 17 - Enviado conteúdo via requisição headers | headers.content-type | headers.access-control-allow-origin</li>
    <li>Aula 18 - Convertendo html em json com o nó 'json', passando pelo payload</li>
    <li>Aula 19 - Upload de arquivos com o nó 'write file'</li>
    <li>Aula 20 - Página com formulário utilizando endpoint 'post' no Node-RED</li>
    <li>Aula 21 - Alimentar a mesmo rota, ocorrendo a atualização da página</li>
    <li>Aula 22 - Capturar conteúdo de outro site por seletor</li>
    <li>Aula 23 - Capturar conteúdo de outro site por seletor</li>
    <li>Aula 24 - Uso do nó 'split' e 'join'</li>
    <li>Aula 25 - Adição do nó 'mysql', adicionando dado em banco (MySQL) e consultando os registros da tabela</li>
    <li>Aula 26 - Adição do nó 'dashboard', usando botões de ação no dashboard</li>
    <li>Aula 27 - Dashboard - adição de campo texto e botão de ação</li>
    <li>Aula 28 - Dashboard - gráficos</li>
    <li>Aula 29 - Dashboard - gráficos</li>
    <li>Aula 30 - Dashboard - gráficos</li>
    <li>Aula 31 a 36 e 39 - CRUD</li>
    <li>Aula 37 - Adicionar dado no banco</li>
    <li>Aula 38 - Consultar dado no banco</li>
</ul>
