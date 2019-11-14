Aqui veremos as configurações do painel tabulado do Portugol Studio.

# Descrição
Essa classe é responsável por gerenciar todas as abas do Portugol Studio. É possível adicionar e remover abas, mudar a aba selecionada e obter as abas ajuda e inicial. Essa classe é filha da classe PSPainelTabulado.
### Localização
`ide\src\main\java\br\univali\ps\paineis\PainelTabuladoPrincipal.java`

# Funções
A seguir serão apresentadas as funções da classe PainelTabuladoPrincipal mais úteis para trabalhar no desenvolvimento do projeto. 

------
### public AbaInicial getAbaInicial()
Essa função retornará a classe AbaInicial que contém a primeira Aba do Portugol, com os exemplos e os arquivos recentes.

Ex:
```JAVA
AbaInicial painelTab = PortugolStudio.getInstancia().getTelaPrincipal().getPainelTabulado().getAbaInicial();
```

Retorna: Instância da classe AbaInicial.

------
### public AbaAjuda getAbaAjuda() 
Essa função retornará a classe AbaAjuda que contém a Aba de ajuda do Portugol, com a documentação da Sintaxe e da Bibliotecas do Portugol Studio.
Ex:
```JAVA
AbaAjuda ajuda = PortugolStudio.getInstancia().getTelaPrincipal().getPainelTabulado().getAbaAjuda();
```

Retorna: Instância da classe AbaAjuda.

------
### public Aba mudarParaAba(Aba aba)

------

