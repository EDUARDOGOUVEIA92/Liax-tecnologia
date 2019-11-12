Aqui veremos como funciona a Tela Principal do Portugol Studio

# Descrição
Essa classe, mantém o painel tabulado do Portugol Studio. A partir desse painel tabulado é possivel acessar as abas abertas e criar novas abas. Ela também é responsável por adicionar as abas iniciais do Portugol Studio e verificar as atualizações.
### Localização
`ide\src\main\java\br\univali\ps\telas\TelaPrincipal.java`

# Funções
A seguir serão apresentadas as funções da classe Tela Princiapl mais úteis para trabalhar no desenvolvimento do projeto. 

------
### public PainelTabuladoPrincipal getPainelTabulado()
Essa função retornará a classe PainelTabuladoPrincipal que contém todas as abas abertas do Portugol Studio.
Mais detalhes dela aqui.
Ex:
```JAVA
PainelTabuladoPrincipal painelTab = PortugolStudio.getInstancia().getTelaPrincipal().getPainelTabulado();
```

Retorna: Instância da classe PainelTabuladoPrincipal.

------
### public void criarNovoCodigoFonte()
Essa função cria uma nova aba no Portugol Studio com o código padrão.

Sem retorno.

------
### public void abrirArquivosCodigoFonte(final List<File> arquivos)
Essa função abre uma lista de arquivos .por no Portugol Studio.

Sem Retorno

------
### public AbaCodigoFonte obterAbaArquivo(File arquivo)
Essa função retorna a Aba que está com o arquivo enviado por parâmetro aberto.

Retorna: Instância da classe AbaCodigoFonte.

------