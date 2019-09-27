Existem diversas maneiras de se utilizar o git, com diversas ferramentas. Neste Tutorial apresentaremos o Git normal, utilizado pelo console e o GitKraken que possui uma interface para a visualização e gestão dos projetos em git. Ele é um sistema de controle de versões que te ajuda a manter projetos versionados na nuvem, ou seja, terá um registro de todas as modificações que você fizer no projeto.

# 1 Download

## 1.1 Instalação
Faça o download do GitBash neste [link](https://git-scm.com/downloads) ou do GitKraken neste [link](https://www.gitkraken.com/).
Instale o de sua preferencia.
<div align="center">
    <a href="https://git-scm.com/downloads"><img src="https://cdn.discordapp.com/attachments/571157550956019741/622108484913201162/unknown.png" width="350"></a>
    <a href="https://www.gitkraken.com/"><img src="https://cdn.discordapp.com/attachments/571157550956019741/622109305491161102/unknown.png" width="350"></a>
</div>

# 2 Configurando ambiente
Aqui configuraremos o Git e o GitKraken para funcionarem com a sua conta do GitHub. Isso será necessário apenas uma vez.

## 2.1 Git
Abra o GitBash

Digite nele os seguintes comandos, substituindo seu nome e e-mail nos lugares pedidos respectivamente:

`git config --global user.name "Seu nome aqui"`

`git config --global user.email "seu_email@exemplo.com"`

## Passo 2.2 GitKraken
Abra o GitKraken

Quando ele terminar de abrir a seguinte tela aparecerá:

<div align="center">
    <a><img src="https://cdn.discordapp.com/attachments/571157550956019741/624037306273235016/unknown.png" width="250"></a>
</div>

Entre com sua conta do Github clicando em *Sign in with Github*. O seu Browser irá abrir pedindo para entrar no seu Github (se você não estiver logado ainda). Entre na sua conta e na próxima tela clique em *Authorize* e sua conta Github se ligará ao GitKraken.

# 3 Clonando o projeto
Nesta parte faremos o download do Portugol Studio como um projeto versionado git.

Primeiro entre na sua conta do Github em um browser e entre no seu repositório Fork que você deve ter feito nos tutoriais anteriores. No seu repositório clique no botão verde chamado *Clone or Download* e em seguida no botão marcado pela seguinte imagem.

<div align="center">
    <a><img src="https://cdn.discordapp.com/attachments/571157550956019741/624043968103055370/unknown.png"></a>
</div>

O link para o seu repositório git foi copiado para sua área de transferência. Agora é necessário baixar o repositório através do GitBash ou do GitKraken, isso é visto no próximo tópico. Para isso é sugerido ter uma pasta no seu computador que terá repositórios que serão baixados do git.

## 3.1 GitBash

Abra o GitBash <img src="https://gitforwindows.org/img/gwindows_logo.png" width="25">

Ele iniciará na sua pasta de usuário do sistema. Você pode ver quais pastas estão dentro dela digitando `ls` no console.

<img src="https://cdn.discordapp.com/attachments/571157550956019741/627151341810089994/unknown.png" width="400">

Você pode entrar em uma das pastas mostradas pelo comando `ls` utilizando o comando `cd + *espaço* + *nome da pasta*` (você pode digitar o começo do nome da pasta e aperta `tab` no teclado para autocompletar).

Exemplo: Entrando na pasta Documentos

<img src="https://cdn.discordapp.com/attachments/571157550956019741/627152453598445571/unknown.png" width="400">

Para voltar uma pasta acima, utilize `cd ..`

<img src="https://cdn.discordapp.com/attachments/571157550956019741/627153403243659278/unknown.png" width="400">

Agora com os comandos de navegação conhecidos, utilize eles para navegar até a pasta que quer colocar o Portugol Studio. No meu caso criei uma pasta no Documentos chamada Git, em que coloco todos os repositórios baixados do Github.

<img src="https://cdn.discordapp.com/attachments/571157550956019741/627154618664615966/unknown.png" width="400">

Agora com o link do Git que copiamos no passo 3, utilize o comando `git clone `+`*link copiado*` (para colar o link utilize `Shift+Insert`no teclado ou clique com o botão direito e selecione `paste`)

<img src="https://cdn.discordapp.com/attachments/571157550956019741/627156252417327123/unknown.png" width="400">

Ele começará a baixar os arquivos para a pasta atual. Pode demorar um pouco dependendo da velocidade da sua internet. Assim que ele terminar você poderá navegar até a pasta com o navegador padrão do seu sistema e encontrar o Portugol Studio baixado.

## 3.2 GitKraren

Abra o GitKraken <img src="https://dl2.macupdate.com/images/icons256/56930.png" width="25">

Sua tela inicial será semelhante a esta:

<img src="https://cdn.discordapp.com/attachments/571157550956019741/627197712277831690/unknown.png" width="400">

Entre na opção *Clone a Repo*

A primeira opção clone with URL te permitira utilizar o link que copiamos no passo 3 para baixar o repositório.

Na caixa *Where to clone to*, clique em Browse e selecione a pasta que deseja baixar o repositório.

Na caixa URL, cole o link copiado e clique em *Clone the repo!*

<img src="https://cdn.discordapp.com/attachments/571157550956019741/627216817932468224/unknown.png" width="400">

Ele começará a baixar o repositório na pasta correta. Quando baixado a seguinte opção aparecerá no GitKraken.

<img src="https://cdn.discordapp.com/attachments/571157550956019741/627216374976217118/unknown.png" width="400">

Clique em *Open Now*. A arvore de commits do Portugol aparecerá. Pronto o repositório está baixado e você poderá acessar ele na pasta que selecionou.

# 4 Baixando atualizações
Nesta seção olharemos como baixar as atualizações do Portugol Studio caso o seu repositório local fique desatualizado tanto por ter feito modificações em outro computador como por querer as modificações feitas na versão oficial do Portugol Studio.

## 4.1 Baixando as próprias modificações

### 4.1.1 No GitBash
Entre na pasta em que está Portugol Studio e digite `git pull`

<img src="https://cdn.discordapp.com/attachments/571157550956019741/627223005734633483/unknown.png" width="400">

### 4.1.2 No GitKraken
Abra o repositório pelo GitKraken pelo *Open Repo* se não estiver aberto.

Na barra superior você pode aperta o botão *pull* para baixar as atualizações

<img src="https://cdn.discordapp.com/attachments/571157550956019741/627223328985186345/unknown.png" width="800">

## 4.2 Baixando as modificações do Portugol Studio Oficial

### 4.2.1 No GitBash
Entre na pasta em que está Portugol Studio e digite os seguintes comandos.

`git remote add upstream https://github.com/UNIVALI-LITE/Portugol-Studio.git`

`git fetch upstream`

`git checkout master`

`git rebase upstream/master`

`git push -f origin master`

As atualizações estarão baixadas e salvas no seu repositório.

### 4.2.2 No GitKraken
Vá na barra lateral do repositório no GitKraken onde está escrito *Remote*. Clique no botão **+* que aparecer.

Vá na opção Pull URL e cole a URL do Portugol Studio oficial: `https://github.com/UNIVALI-LITE/Portugol-Studio.git`. Dê um nome a ela e clique em *Add Remote*.

<img src="https://cdn.discordapp.com/attachments/571157550956019741/627237502662737930/unknown.png" width="400">

Na árvore de commits, procure o commit master do Portugol Studio (haverá um icone com essa <img src="https://avatars1.githubusercontent.com/u/1704041?s=200&v=4" width="25"> imagem). Arraste ele até o seu próprio master e clique em `merge [nomequevocedeu/master] into master`

# 5 Fazendo um commit e enviando

Nesta seção veremos como enviar suas modificações locais para o seu repositório do Portugol-Studio no Github.

## 5.1 No GitBash

Entre na pasta do repositório do seu Portugol Studio e digite `git status`.

Uma lista de arquivos em vermelho aparecerá, eles são os arquivos que foram modificados desde o último commit. Eles deverão primeiro serem adicionados em um commit que salvará eles. Para fazer isso primeiro digite. `git add --all`.

<img src="https://cdn.discordapp.com/attachments/571157550956019741/627242331002634241/unknown.png" width="400">

Em seguida digite `git commit -m "[mensagem indicando o que foi feito no commit]"`.

Por fim digite:

`git push --set-upstream-to origin master"` se é seu primeiro push

ou

`git push"`se já fez um push anteriormente com o comando anterior

<img src="https://cdn.discordapp.com/attachments/571157550956019741/627242518832087051/unknown.png" width="400">

## 5.2 No GitKraken

Abra o GitKraken no seu repositório. Se você fez alguma modificação perceberá que agora há uma linha de commit extra acima do último commit com um `//WIP` escrito. Clique nela e a tela ficará semelhante a essa

<img src="https://cdn.discordapp.com/attachments/571157550956019741/627243597132988456/unknown.png" width="400">

Na coluna à direita na caixa `Unstaged Files`, você verá os arquivos seus que foram modificados.
Clique nos arquivos que quer adicionar ao commit ou clique em `Stage all files` para adicionar todos.
Na última caixa `Commit Message`, adicione a mensagem indicando o que foi modificado.

<img src="https://cdn.discordapp.com/attachments/571157550956019741/627244965793234974/unknown.png" width="400">

Clique em `Commit changes do N files`. Você terá feito um commit, mas apenas localmente. Para enviar para o repositório no Github, clique em `Push`. Caso apareça mais alguma mensagem, dê apenas um ok.

<img src="https://cdn.discordapp.com/attachments/571157550956019741/627245683644170291/unknown.png" width="400">

## 5.3 Final
Uma vez feito o push por qualquer um dos dois métodos, você já poderá ver no repositório no github seu commit com as modificações:
<img src="https://cdn.discordapp.com/attachments/571157550956019741/627246171991179295/unknown.png" width="800">

<div align="right">
   <a href="#">
      <img src="https://i.imgur.com/OG7k1pu.png" align="right">
   </a>
   <a href="https://github.com/UNIVALI-LITE/Portugol-Studio/wiki/Criando-uma-conta-no-GitHub">
      <img src="https://i.imgur.com/cCsIdh6.png" align="right">
   </a>
</div>