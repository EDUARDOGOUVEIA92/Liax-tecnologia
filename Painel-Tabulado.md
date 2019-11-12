Aqui veremos as configurações do painel tabulado do Portugol Studio.

# Descrição
Essa classe é responsável por gerenciar todas as abas do Portugol Studio. É possível adicionar e remover abas, mudar a aba selecionada e obter as abas ajuda e inicial. Essa classe é filha da classe PSPainelTabulado.
### Localização
`ide\src\main\java\br\univali\ps\paineis\PainelTabuladoPrincipal.java`

# Funções
A seguir serão apresentadas as funções da classe PainelTabuladoPrincipal mais úteis para trabalhar no desenvolvimento do projeto. 

------
### public AbaInicial getAbaInicial()
Essa função retornará a classe PainelTabuladoPrincipal que contém todas as abas abertas do Portugol Studio.
Mais detalhes dela aqui.
Ex:
```JAVA
PainelTabuladoPrincipal painelTab = PortugolStudio.getInstancia().getTelaPrincipal().getPainelTabulado();
```

Retorna: Instância da classe PainelTabuladoPrincipal.

------
### public AbaAjuda getAbaAjuda() 

------
### public Aba mudarParaAba(Aba aba)

------

