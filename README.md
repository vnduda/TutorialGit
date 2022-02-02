## Bem vindos ao nosso primeiro tutorial!

Se você caiu aqui de paraquedas, esse tutorial escrito é material de apoio do vídeo: [Tutorial Git e Github](https://www.youtube.com/watch?v=6arOMdYC9Oc)

Para esse tutorial vamos precisar de: uma conta aqui no github, e um editor ou IDE de sua preferência (nesse caso eu utilizarei o VS Code)

#### Primeiro passo: Instalação do git
Para começar tudo, precisamos começar a nossa instalação do git, e ele pode ser feito através do link: [Git](https://git-scm.com/downloads)

##### O que é o git? 
Git é nossa ferramenta de controle de versionamento, ou seja, através dela, vamos conseguir ter todo um histórico de mudanças do nosso código, além de outras ferramentas muito úteis, principalmente se estamos falando de código em empresas com muitos funcionários!

#### Configurações iniciais do git
Nosso primeiro passo é configurar nosso git para conectar com nossa conta aqui do github! 

Para isso vamos digitar no nosso Git Bash (ou terminal de sua preferência):

<pre><code> git config --global user.name 'seunomedeusuariodogithub' </code></pre>
e 
<pre><code> git config --global user.email 'seuemaildogithub' </code></pre>

#### Começando um repositório vazio no github
Para nosso projeto estamos considerando que começaremos esse projeto do zero, ou seja, não possuimos nenhum código em nossa máquina, e que ele ainda será desenvolvido.

Para criar nosso repositório precisamos ir ao nosso perfil do github, clicar em **Repositories** e no botão verde escrito **New**

![Captura de tela de 2022-02-01 21-48-44](https://user-images.githubusercontent.com/49242526/152079887-1f55ffd0-8728-4fc3-913a-5bc86d8b6d06.png)

Assim que preencher o nome do repositório, basta clicar em **Create repository**

![Captura de tela de 2022-02-01 21-48-47](https://user-images.githubusercontent.com/49242526/152079893-2a88e4e0-6c5d-480d-b52d-7ca6fe5ee204.png)

#### Clonando um repositório 
Agora precisamos trazer esse repositório que estava apenas no nosso github, para a nossa máquina também!

Para isso faremos no terminal:
<pre><code>git clone 'link do repositório' </code></pre>

Após isso vamos perceber que aparecerá uma pasta no nosso computador com o mesmo nome do Github, e dentro dela vamos ter uma pasta `.git`

Essa pasta `.git` ficará na nossa pasta principal e não vamos mexer nela! 

#### Criando um arquivo que vamos mandar para o Github!

Agora chegou a hora de botar a mão na massa e mandar um arquivo para nosso github! Para isso vamos abrir nosso VS Code, e abrir nele nossa pasta que clonamos do Github!

Depois de abrir essa pasta, vamos criar um arquivo `Readme.md`

Com isso já conseguimos ter um arquivo para mandar para o github

Para isso vamos seguir três passos principais:

<pre><code> git add . </code></pre> ou <pre><code> git add nomedoarquivo </code></pre>

Com esses comandos você pode tanto adicionar todos os arquivos que existir (com git add .), ou adicionar um arquivo apenas, usando o segundo comando. Isso faz com que as mudanças fiquem na área de stagging 

Depois isso faremos o nosso commit <pre><code> git commit -m 'mensagem que descreve brevemente o que você fez'</code></pre>

O commit serve basicamente para mandar nossa mudança com uma mensagem, que descreve de forma breve as alterações que aconteceram naquele codigo que você está mandando!

O último passo é dar o empurrão final para o nosso código subir para o github, para isso vamos usar o comando <pre><code> git push -u origin main </code></pre>

E tchanan! Se atualizarmos nosso navegador, vamos ver as mudanças refletidas no repositório aqui no Github!
