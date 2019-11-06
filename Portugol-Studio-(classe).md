Aqui falaremos sobre a classe principal da IDE a PortugolStudio.java

# Descrição
Essa classe é um [Singleton](https://pt.wikipedia.org/wiki/Singleton) ela é a classe que permite acessar todas as outras classes da IDE. através dela, é possível acessar a Tela Principal, que dá acesso ao Painel Tabulado que então dá acesso as abas do Portugol Studio. Ela também é responsável por inicializar todas telas do Portugol Studio, carregar os arquivos de configuração e verificar os arquivos recuperados e recentes.

### Localização
ide/src/main/java/br/univali/ps/nucleo/PortugolStudio.java

# Dicas


# Funções

public static PortugolStudio getInstancia()

private PortugolStudio()

public void iniciarNovaInstancia(String[] parametros)

public void finalizar(int codigo)

private void exibirTelaPrincipal()

public TelaPrincipal getTelaPrincipal()

public JDialog getTelaSobre()

public JDialog getTelaRelatarBug()

public JDialog getTelaAtalhosTeclado()

public JDialog getTelaDicas()

public JDialog getTelaPluginsInstalados()

public TelaCustomBorder getTelaInformacoesPlugin()

public JDialog getTelaLicencas()

public JDialog getTelaEditarTemas()

public JDialog getTelaPesquisarSubstituir()

public PSFindReplace getTelaProcurarSubstituirPanel()

public JDialog getTelaRenomearSimbolo()

public TelaRenomearSimbolo getTelaRenomearSimboloPanel()

