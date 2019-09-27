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

## GitKraren

Abra o GitKraken <img src="https://dl2.macupdate.com/images/icons256/56930.png" width="25">


# Baixando atualizações

# Fazendo um commit e enviando

# Criando Branchs

<div align="right">
   <a href="#">
      <img src="https://i.imgur.com/OG7k1pu.png" align="right">
   </a>
   <a href="https://github.com/UNIVALI-LITE/Portugol-Studio/wiki/Criando-uma-conta-no-GitHub">
      <img src="https://i.imgur.com/cCsIdh6.png" align="right">
   </a>
</div>