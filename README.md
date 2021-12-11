
## SENAI-SP 
### Encontro Remoto 1



#### Elaboração de teste de navegabilidade automática no site SENAI ao realizar uma pesquisa por cursos num campo de busca.
<br><br>

<h2 align="center">R E L A T Ó R I O </h2>

**Descrição**

Nesta atividade, foram testadas as funcionalidades através da execução de um teste automático de navegabilidade no site do SENAI. 

**Ferramentas**

Foi feito o download e instalação do **Eclipse IDE for Enterprise Java and Web Developers, versão 2021-09 ,  do JDK 1.8 e do Apache Maven**.  Uma vez que o procedimento foi feito com o navegador Google Chrome ,  foi preciso também efetuar o download do executável **ChromeDriver (WebDriver)** compatível com a versão do browser. Todas as variáveis ambientes do Java e Maven foram devidamente configuradas na máquina Windows 10. Foram utilizadas as dependências do projeto **Selenium e JUnit** dentro do Eclipse após a pesquisa no  repositório do Maven. <br/><br/>

O Selenium consiste num framework que possui um recurso chamado WebDriver, o qual permite a automatização do browser, podendo ser utilizada em várias linguagens de programação. Nesta atividade foi utilizada a linguagem Java. O JUnit é um framework que facilita o desenvolvimento e execução de testes em código Java. Fornece uma completa API (conjunto de classes) para construir os testes.


**Métodos**

Dentro da pasta src/test/java foi criado um pacote chamado webdriver que contém uma classe chamada _HomePage_. 

Nessa classe foram elaborados procedimentos para configuração **antes** do teste ser feito. Estas rotinas foram responsáveis por abrir o navegador Chrome, ficar em dormência por 2 segundos para dar tempo de carregar a página e maximizar o navegador.

Na fase  de **teste** propriamente dita, foi elaborado um código para ter acesso ao site SENAI de forma automatizada, e a busca por id de um elemento input (campo de pesquisa da página) , onde foi possível por a palavra chave “gestão” neste campo selecionado. Com isso, foi feita uma simulação de um usuário pressionando a tecla ENTER ao fazer a pesquisa por cursos. 
Alternativamente, também foi possível selecionar por id o botão de pesquisar para em seguida simular o seu clique. 


**Resultados e considerações**

O navegador foi aberto com sucesso , onde foi acessado o site do SENAI, permitindo a seleção de um campo de busca e o envio da palavra “gestão” para realizar a pesquisa. Contudo, apesar de aparecerem resultados para a pesquisa, foi informado que foram encontrados  0 resultados para “gestão”, o que caracteriza um bug no site, vindo de uma possível falha interna no código.


---

**Execução do teste**

![teste](https://user-images.githubusercontent.com/88597534/145659993-079d747f-28eb-436f-a4bb-3a28cc20787d.gif)
