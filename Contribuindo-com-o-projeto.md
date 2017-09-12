Se você está interessado em ajudar no desenvolvimento do  **Portugol Studio**, ou testar a versão mais atual do sistema, é necessário seguir alguns passos.

* **Baixe e instale o** [JDK versão 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html): certifique-se de escolher a versão correspondente ao seu sistema operacional. **Para usuários do Ubuntu**, recomendamos instalar esta versão [aqui](http://www.diolinux.com.br/2014/03/como-instalar-java-8-no-ubuntu.html)

* **Crie uma conta no GitHub**: acesse o endereço https://github.com/join e faça o registro seguindo os passos na tela

* **Baixe e instale o** [Git](https://git-scm.com/book/pt-br/v1/Primeiros-passos-Instalando-Git): certifique-se de escolher a versão correspondente ao seu Sistema Operacional

* **Baixe e instale o** [GitKraken](https://www.gitkraken.com/): este software é opcional, mas é mais fácil de trabalhar do que com o Git na versão de linha de comando

* **Clone este repositório**: com o [Git](https://git-scm.com/book/pt-br/v1/Primeiros-passos-Instalando-Git) instalado, abra o **terminal do git (não do Sistema Operacional)** e digite o comando: ```git clone https://github.com/UNIVALI-LITE/Portugol-Studio.git```. Se estiver usando o [GitKraken](https://www.gitkraken.com/), siga este tutorial: [TODO: Tutorial do GitKraken]()


* **Execute o Portugol Studio**: abra um terminal do sistema operacional e navegue até a pasta onde o Portugol Studio foi clonado. Em seguida digite o comando ```./gradlew run``` para executar. **Se estiver no Windows pode ser necessário rodar um comando um pouco diferente:** ```./gradlew.bat run```. Você também pode trocar a instrução ```run``` por ```build``` (para gerar os binários) e ```dist-gui``` (para gerar os instaladores)

* **Baixe e instale uma ferramenta para trabalhar**: se preferir, você pode utilizar um ambiente de programação para trabalhar. Isto permite compilar e executar o Portugol Studio sem digitar comandos no terminal do Sistema Operacional. Recomendamos o [NetBeans](https://netbeans.org/) ou o [Eclipse](http://www.eclipse.org/downloads/eclipse-packages/). Após baixar a ferramenta desejada, siga um destes tutoriais para abrir os projetos: [TODO: Tutorial do NetBeans com Gradle]() ou [TODO: Tutorial do Eclipse com Gradle]()

**Sentiu dificuldade?** Não se preocupe, novas instruções serão acrescentadas a esta página conforme o projeto for avançando. Sinta-se a vontade para tirar dúvidas em nosso [fórum online](https://discord.gg/fRW7Vq2)