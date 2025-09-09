#carlos.ribeiro.8-periodo

<h1 align="center">  ATIVIDADE AVALIAÇÃO PROCESSUAL </h1>  
#Computação movel // Edgard da Cunha

#
Carlos Ribeiro Greggio;  
Eduardo Miranda;
#

# Sobre o trabalho
Esta aplicação foi criada uma atividade avaliativa para o curso de sistemas de informação, com o objetivo demonstrar as habilidades no em linguagem Dart e em Flutter do alunos do turma.

Trabalho esse que foi realizado em 3 partes e se trata de uma aplicação que funciona como uma forma de filtro para certos itens no sistema.
Ne caso foi feito um sistema de munitoria de alunos de encino superior de de difentes idades e varios cursos, mas da mesma instituição ictícia.

## Part1;
Nesta etapa foi criado a estrutura básica do Dart sem o auxílio a interface visual do Flutter, desta forma podendo apenas ser usado no console. O programa oferece duas opções 1 para utilizar o sistema e opção 2 para desligar o sistema, E na opção existem duas linhas de ação que podem ser toma das por curas filtrando por 'idade' ou 'média', que no caso são 'ide' e 'med' repequitivamente. Atraves das operações '>', '<', '=>' e '<=' para encontrar os estudantes que se enquadrão.

  https://github.com/CRGlg/carlos.ribeiro.8-periodo/commit/b1b5609345f202c85be0992c80646bbb943d18dd
  

![excutando no consolo, sem interface visual](https://github.com/CRGlg/carlos.ribeiro.8-periodo/blob/main/MATERILvisual/Captura%20de%20tela%202025-09-08%20183050.png)

Neste ponto foi feito uso de elemendos de controle de entrada "switch" para poder inciar o programa de separar os alunos e também fechar a programa, desta forma as funções "encontrarEstudantesPorValor()" e "consultarEstudantes()" fazem o trabalho de consultar a lista da aplicação separando os separando pela operações ">=" e "<=", e no final o método "apresentar()" chama e exibe o reusltado segundo o conteudo contido em "List<Estudantes>".


## Part2;
já na parte 2 o código teve de ser autorizado para incluir os elementos fort-end, ou seja o a implementação de flutter de forma que agora tem uma interface com o usuário. A interface tem recurso visuais que são usados nas visulização dos alunos que estão no sistema e para a implementar as caixas do caracteres númericos.

As quatro areias que são para selecionar os alunos que se emcaixão no o usuáoria determinar, as buscas poden ser feitas estabelecendo um teto e/ou chão para os critérios de 'médio' e/ou 'idade' e demais informações dos alunos sendo apresentadas nos perfis dos mesmos.

  https://github.com/CRGlg/carlos.ribeiro.8-periodo/blob/7dcd5cbf7fc3e6687ac6aabf64fa4a1430a5687f/part-2

![interface da tela do android mostrando como ficou](https://github.com/CRGlg/carlos.ribeiro.8-periodo/blob/main/MATERILvisual/Captura%20de%20tela%202025-09-08%20184554.png)
![interface sendo usada para seleção de estudantes](https://github.com/CRGlg/carlos.ribeiro.8-periodo/blob/main/MATERILvisual/Captura%20de%20tela%202025-09-08%20194230.png)
![interface sendo usada para seleção de estudantes](https://github.com/CRGlg/carlos.ribeiro.8-periodo/blob/main/MATERILvisual/Captura%20de%20tela%202025-09-08%20195759.png)
![interface sendo usada para seleção de estudantes](https://github.com/CRGlg/carlos.ribeiro.8-periodo/blob/main/MATERILvisual/Captura%20de%20tela%202025-09-08%20220125.png)

No código que foi atualiza do para a parte 2 a principal coisa que vale resaltar, forra os novos elementos visuais, são os "TextEditingController" que atraves dos quadros vão separar os menbras da classee Estudante de acordo com valores macimos e/ou minimos de 'Idade' e/ou 'Média', podendo ser usados os dois alvos de busca simultaneamente. "initState()" é executado uma única vez ao iniciar o widget e por meioda das listeners que detecta uma ou mais alterações e chama a função aplicarFiltros automaticamente, mas tambem possui uma widget 'StatelessWidget' para criação e fiquiçação de um cabeçalho.



## Part3; 
Agora vem novas funões e elementos dinamicos que tendem a melorar a experiencia de deichar os recurso estaticos em segundo plano. As 3 grandes novidades são 3 botões um que vão alternar entre o modo de tela clara e tela escura, outro que vai zerar as caixas de texto e mais um que vai ordenar por ordem alfabética ou ordem por idade decrescente (do mais velho ao mais novo), assim organizando o processo de busca de forma mais clara e com recusos visuais que ajudam na atenção.


https://github.com/CRGlg/carlos.ribeiro.8-periodo/blob/main/part-3



  
![tela de verção anterior em execução](https://github.com/CRGlg/carlos.ribeiro.8-periodo/blob/main/MATERILvisual/Captura%20de%20tela%202025-09-09%20154654.png)


![tela de verção anterior em execução22](https://github.com/CRGlg/carlos.ribeiro.8-periodo/blob/main/MATERILvisual/Captura%20de%20tela%202025-09-09%20154716.png)  
![tela da app rodando](https://github.com/CRGlg/carlos.ribeiro.8-periodo/blob/main/MATERILvisual/Captura%20de%20tela%202025-09-09%20154802.png)
![tela da app rodando](https://github.com/CRGlg/carlos.ribeiro.8-periodo/blob/main/MATERILvisual/Imagem%20do%20WhatsApp%20de%202025-09-09%20%C3%A0(s)%2016.14.55_4d7e0edd.jpg)
  


O componente principal do código "StudentListPage"  que é um StatefulWidget. Essa widget mutavel é essencial para o funcionamento do aplicativo, pois ele precisa gerenciar um estado mutável, ou seja, dados que mudam ao longo do tempo e afetam a interface do usuário, justamente na "StudentListPageState" é onde a essência de todas as coisas acontecem todas as filtragens, todas as ordenações e mudanças que são refletidas na interface visual do flutter. Para que a mudansas que os novos botões fazem o método "setState()" por meio dele o framework flutter sabe o estado interno do widget, quando alterado movimenta para a interface ser reconstruída para refletir as novas informações, o botão "Ordenar" quando acionado atualiza o widget com o novo modo de ordenação que vai estar de acrodo com os requisitos de logicos da função.  










