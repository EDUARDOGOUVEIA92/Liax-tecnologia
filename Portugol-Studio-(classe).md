Aqui falaremos sobre a classe principal da IDE a PortugolStudio.java

# Descrição
Essa classe é um [Singleton](https://pt.wikipedia.org/wiki/Singleton) ela é a classe que permite acessar todas as outras classes da IDE. através dela, é possível acessar a Tela Principal, que dá acesso ao Painel Tabulado que então dá acesso as abas do Portugol Studio. Ela também é responsável por inicializar todas telas do Portugol Studio, carregar os arquivos de configuração e verificar os arquivos recuperados e recentes.

### Localização
`ide\src\main\java\br\univali\ps\nucleo\PortugolStudio.java`

# Dicas


# Funções
A seguir serão apresentadas as funções da classe Portugol Studio mais úteis para trabalhar no desenvolvimento do projeto. 

------
### public static PortugolStudio getInstancia()

Essa função sempre deve ser chamada antes de chamar qualquer função da classe. Ela faz pare do padrão Singleton assim não sendo necessário instanciar-la para chamar uma de suas funções. Por exemplo: chamando a função getTelaDicas().

```JAVA
JDialog telaDicas = PortugolStudio.getInstancia().getTelaDicas();
```

Retorna: Instância da classe PortugolStudio

------
### public void iniciarNovaInstancia(String[] parametros)

Função que inicializa todas as outras classes do Portugol Studio. Ela é quem passa o splash (tela inicial de carregamento) na tela, atualizando ela de acordo com as classes que são carregadas.

Sem retorno.

------
### public void finalizar(int codigo)
Função que finaliza o Portugol corretamente. Ela remove os arquivos temporário do Portugol e salva as configurações que foram modificadas. Após isso ela finaliza a execução do Portugol.

Sem retorno.

------
### public TelaPrincipal getTelaPrincipal()
Função que possui a classe TelaPrincipal. A TelaPrincipal é a classe que possui os componentes entre o título e as bordas do Portugol. É a partir dela que você terá acesso as abas existentes no Portugol e consequentemente à Aba Inicial e Aba de Código Fonte. Mais detalhes em ......

Retorna: Instância da classe TelaPrincipal.

------
### public JDialog getTelaSobre()
Função que possui a tela Sobre do Portugol Studio. No PortugolStudio essa tela é acessível na Aba Inicial, pelos menus inferiores, é possível localizar a opção "Sobre", que te apresentará a tela. Essa tela possui as informações de todos os atuais e antigos principais colaboradores do Portugol Studio.

Retorna: Instância de JDialog da TelaSobre.

A tela é um JDialog e para acessar o painel Sobre contendo os componentes é necessário chamar a função getPanel fazendo um cast de TelaCustomBorder e Sobre. Ex:

```JAVA
Sobre sobre = (Sobre)((TelaCustomBorder)PortugolStudio.getInstancia().getTelaSobre()).getPanel();
```
Alternativamente você pode alterar a tela acessando ela na seguinte localização: `ide\src\main\java\br\univali\ps\ui\telas\Sobre.java`

------
### public JDialog getTelaRelatarBug()
Função que possui a tela de Relatar Bug do Portugol Studio. No PortugolStudio essa tela é acessível na Aba Inicial, pelos menus inferiores, é possível localizar a opção "Relatar Bug", que te apresentará a tela. Essa tela possui as informações de como relatar um bug ou contatar a equipe do Portugol Studio.

Retorna: Instância de JDialog da TelaRelatarBug.

A tela é um JDialog e para acessar o painel RelatarBug contendo os componentes é necessário chamar a função getPanel fazendo um cast de TelaCustomBorder e TelaRelatarBug. Ex:

```JAVA
TelaRelatarBug relatarBug = (TelaRelatarBug)((TelaCustomBorder)PortugolStudio.getInstancia().getTelaRelatarBug()).getPanel();
```
Alternativamente você pode alterar a tela acessando ela na seguinte localização: `ide\src\main\java\br\univali\ps\ui\telas\TelaRelatarBug.java`

------
### public JDialog getTelaAtalhosTeclado()
Função que possui a tela de Atalhos de Teclado do Portugol Studio. No PortugolStudio essa tela é acessível na Aba Inicial, pelos menus inferiores, é possível localizar a opção "Atalhos de Teclado", que te apresentará a tela. Essa tela possui as informações sobre os atalhos de teclado que podem ser usados no Portugol Studio.

Retorna: Instância de JDialog da TelaAtalhos.

A tela é um JDialog e para acessar o painel TelaAtalhos contendo os componentes é necessário chamar a função getPanel fazendo um cast de TelaCustomBorder e TelaAtalhos. Ex:

```JAVA
TelaAtalhos atalhos= (TelaAtalhos)((TelaCustomBorder)PortugolStudio.getInstancia().getTelaAtalhosTeclado()).getPanel();
```
Alternativamente você pode alterar a tela acessando ela na seguinte localização: `ide\src\main\java\br\univali\ps\ui\telas\TelaAtalhos.java`

------
### public JDialog getTelaDicas()
Função que possui a tela de Dicas do Portugol Studio. No PortugolStudio essa tela é acessível na Aba Inicial, pelos menus inferiores, é possível localizar a opção "Dicas de Interface", que te apresentará a tela. Essa tela possui as dicas de como usar as funções básicas do Portugol Studio.

Retorna: Instância de JDialog da TelaDicas.

A tela é um JDialog e para acessar o painel TelaDicas contendo os componentes é necessário chamar a função getPanel fazendo um cast de TelaCustomBorder e TelaDicas. Ex:

```JAVA
TelaDicas dicas= (TelaDicas)((TelaCustomBorder)PortugolStudio.getInstancia().getTelaDicas()).getPanel();
```
Alternativamente você pode alterar a tela acessando ela na seguinte localização: `ide\src\main\java\br\univali\ps\ui\telas\TelaDicas.java`

------
### public JDialog getTelaPluginsInstalados()
Função que possui a tela de Plugins Instalados do Portugol Studio. No PortugolStudio essa tela é acessível na Aba Inicial, pelos menus superiores, é possível localizar a opção "Plugins", que te apresentará a tela. Essa tela possui uma lista dos plugins instalados e opções de instalação de novos plugins no Portugol Studio.

Retorna: Instância de JDialog da PainelPluginsInstalados.

A tela é um JDialog e para acessar o painel PainelPluginsInstalados contendo os componentes é necessário chamar a função getPanel fazendo um cast de TelaCustomBorder e PainelPluginsInstalados. Ex:

```JAVA
PainelPluginsInstalados plugins= (PainelPluginsInstalados)((TelaCustomBorder)PortugolStudio.getInstancia().getTelaPluginsInstalados()).getPanel();
```
Alternativamente você pode alterar a tela acessando ela na seguinte localização: `ide\src\main\java\br\univali\ps\ui\telas\PainelPluginsInstalados.java`

------
### public JDialog getTelaLicencas()
Função que possui a tela de Licenças de uso dos componentes do Portugol Studio. No PortugolStudio essa tela é acessível na Aba Inicial, pelos menus inferiores, é possível localizar a opção "Sobre", que te apresentará a tela de informações do Portugol. No canto inferior direito desta tela, no ícone de um papel, ao clicar nele a tela aparecerá. Essa tela possui abas com todas as licenças de uso de componentes do Portugol Studio.

Retorna: Instância de JDialog da TelaLicencas.

A tela é um JDialog e para acessar o painel TelaLicencas contendo os componentes é necessário chamar a função getPanel fazendo um cast de TelaCustomBorder e TelaLicencas. Ex:

```JAVA
TelaLicencas licencas= (TelaLicencas)((TelaCustomBorder)PortugolStudio.getInstancia().getTelaLicencas()).getPanel();
```
Alternativamente você pode alterar a tela acessando ela na seguinte localização: `ide\src\main\java\br\univali\ps\ui\telas\TelaLicencas.java`

------
### public JDialog getTelaEditarTemas()
Função que possui a tela de edição de temas do Portugol Studio. No PortugolStudio essa tela é acessível na Aba Inicial, pelos menus inferiores, é possível localizar a opção "dicas interface", que te apresentará a com dicas da interface do  Portugol. No canto inferior direito desta tela, no ícone colorido "Trocar tema", ao clicar nele a tela aparecerá. Alternativamente em uma aba de código fonte, é possível acessa-la por clicar na engrenagem no canto direito superior da tela e clicar em "Editar Temas". Essa tela possui uma lista de cores editáveis de diversas partes do Portugol Studio.

Retorna: Instância de JDialog da TelaEditarTemas.

A tela é um JDialog e para acessar o painel TelaEditarTemas contendo os componentes é necessário chamar a função getPanel fazendo um cast de TelaCustomBorder e TelaEditarTemas. Ex:

```JAVA
TelaEditarTemas temas= (TelaEditarTemas)((TelaCustomBorder)PortugolStudio.getInstancia().getTelaEditarTemas()).getPanel();
```
Alternativamente você pode alterar a tela acessando ela na seguinte localização: `ide\src\main\java\br\univali\ps\ui\telas\TelaEditarTemas.java`

------
### public PSFindReplace getTelaProcurarSubstituirPanel()
Função que possui a tela de procurar e substituir texto do Portugol Studio. No PortugolStudio essa tela é acessível na Aba Código Fonte, ao apertar "Ctrl+F" no editor de texto. Alternativamente na aba de código fonte, é possível acessa-la por clicar na engrenagem no canto direito superior da tela e clicar em "Pesquisar e Substituir". Essa tela permite buscar por palavras pelo texto do editor do Portugol Studio e substitui-las por outro texto .

Retorna: Instância de PSFindReplace da TelaProcurarSubstituir.

A função chama diretamente o painel com a tela, portanto pode se instancias ela diretamente. Ex:

```JAVA
PSFindReplace psfr= PortugolStudio.getInstancia().getTelaProcurarSubstituirPanel();
```
Alternativamente você pode alterar a tela acessando ela na seguinte localização: `ide\src\main\java\br\univali\ps\ui\editor\PSFindReplace.java`

------
### public TelaRenomearSimbolo getTelaRenomearSimboloPanel()
Função que possui a tela de renomear símbolos do Portugol Studio. No PortugolStudio essa tela é acessível na Aba Código Fonte, ao apertar "Ctrl+R" no editor de texto. Essa tela permite buscar nomes de variáveis, matrizes ou vetores pelo texto do editor do Portugol Studio e substituir por outro nome.

Retorna: Instância de TelaRenomearSimbolo da TelaRenomearSimboloPanel.

A função chama diretamente o painel com a tela, portanto pode se instancias ela diretamente. Ex:

```JAVA
TelaRenomearSimbolo psfr= PortugolStudio.getInstancia().getTelaRenomearSimboloPanel();
```
Alternativamente você pode alterar a tela acessando ela na seguinte localização: `ide\src\main\java\br\univali\ps\ui\telas\TelaRenomearSimbolo.java`