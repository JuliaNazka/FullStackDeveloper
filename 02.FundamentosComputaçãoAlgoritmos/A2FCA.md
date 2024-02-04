# Aula 2 
## Continuação da aula 01, onde foram criados os primeiros 2 programas 

## 1. Trabalhando com banco de Dado
* Como ter um sistema para guardar dados de carros e pessoas - no excel 
        Pessoa
    * | Nome | CPF | 
    * | Mariana | 123456789 |
    * | Lucas | 123456781 |
        
        Carro
    * | Marca | Modelo | Placa 
    * | X | Cr30 | abc-3030 |
    * | Y | WvGol | abc-4030 |
    * | Z | Fs10 | abc-6030 |

        Pessoa_Carro - modelando o banco de dados 
    * | CPF | Placa |
    * | 123456789 | abc-3030 |
    * | 123456781 | abc-4030 |

* Sistema é uma formma de organizar e padronizar algo 
* Quando estamos trabalhando com banco de Dados sempre temos tabelas internas 

## 1. Inversão de Controle e Abstração 
* Ao invés de deixar a estrutura padrão da tabela definir como o sistema vai ser, pode falar que existe "coluna" e "valor"; 
        banco de dados cronológico
   * | coluna |  valor | id_registro | 
   * | nome | Mariana | 1 |
   * | cpf | 123456789 | 1 | 
   * | nome | Lucas | 2 | 
   * | cpf | 123456781 | 2 | 
   * | placa | asc-3030 | 1 | 

* quem tem o ID 1 é a mariana e quem tem o ID 2 é o lucas

* o que é a abstração - como converter um problema do mundo real para código 
    #### * O nome que se dá para a função que formata valor 
* Ex: Datomic - exemplo de banco de dados que vai modelando a sua estrutrua 
* A forma como você abstrai a solução depende do problema que te darem
* existem várias forma de se interpretar e resolver um problema e os dados 
* Banco de Dados relacional - lida melhor quando associa um valor mais simples como um ID 

        tabelas
    * | nome | id | 
    * | Carro | 1 | 
    * | Pessoa | 2 | 
    * | Pessoa_carro | 

        campos
    * | coluna | id_tabela | id_colunas | 
    * | nome | 2 | 1 | 

## 1. Wordpress 
* é uma ferramenta de blog que faz exatamente como o exemplificado 
* | posts | categora | páginas | 
* usa como uma ferramente que abstrai o banco de dados - ferramenta fácil de fazer prototipagem 
* nao funciona para um número muito grande de usuários 
* texto = string 
* valores numéricos = number 
* boolean = boo 

## 1. Navegadores e estruturas de Dados 
#### Como aprender base de programação com o navegador 
* Como simular um navegador e suas abas
* Hoje roda a o HTML5 e o CSS 
* O brawser lê o HTML, JavaScript e CSS(o que faz ficar bonito)
* Parcear e compilar as informações 
* Lida com requests (imagens, arquivos, vídeos,...) - precisa ter algumas informações para saber se foi carregado ou não 
* Histórico - guardar a hora, o site, o título que você acessou. - guarda um por um 
* Favoritos - guarda pasta, itens - um item pode ser uma pasta que guarda diversos itens 

### Trabalhar os recursos do browser 
* Juntar os desafios e tentar solucionar os problemas 
* discrever como representar uma aba aberta no navegador: 
    * https://github.com/omariosouto/pucpos-code/blob/main/a2b1/02-browser/index.html
    * Exercício de como criar uma página em html referênciando um site já existente 
    * O .css serve como arquivo de design do projeto 
    * Quando no código fizer a referência ao style.css ele já reconhece o arquivo e interpreta na mesma página 
* Ao usar o terminal para executar comandos 
    * ls -> mostra o que está na pasta (lista)
    * cd ./(nomePasta)-> entra na pasta digitada
    * ctrl ou clear ->limpa a tela 
    * cd ./03 + tab -> ele faz um auto complete 
    * cd ../ -> Volta a pasta 
    * cd ./"Area de Trabalho" -> Usar as aspas para reconhecer pasta com espaçamento 

* No Vs code vc pode abrir um código e pedir para ver o terminal direto no VS e facilita o dia a dia da programação 
* Aba do navegador é o conjunto do título, da url e dos códigos
    * criar uma variável e detro dela cria um objeto com {} e dentro dele coloca as sintaxes necessárias -> usa chaves 
    * Criar uma lista utiliza nomedalista = []; -> Usa colchetes 
  // Objeto: Representam coisas com multiplos atributos para representa-las {}
  //Arrays: Lista de coisas []
  * Em javascript vc pode acessar alguma propriedade através do "." 
  * Separando com <li></li> -> cria um bullet no texto 

* No vs code vc pode rodar toda a estrutura dando o comando "!" 
    * Template padrão 
        * Meta corrige os caracteres estranhos que nao aparecias 
        * Acrescentam a estrutura que toda página HTML deveria ter 
* Exemplo de entrada, processamento e output 
* como isso pode se aplicar no dia a dia 


## 1.Estruturas e Demanda 
* O profissional está sempre ciando uma estrutrua 
* O to-do list das abas - quando você renderiza as abas poderia ser diversas coisas de diversos locais 
* A nível de código das estruturas é diferente porque estamos criando coisas diferentes - ou seja, não necessáriamente toda vez que for criar uma lista será da mesma forma. 
* Controle das estruturas e das demandas 
* Começar a implementar as filas 

### Fila + Array + Objeto 
* Como simular uma fila 
* Qualquer tipo de dado em que a ordem importa e quem entra primeiro sai primeiro 
* Hacker Rank -> filtrar os candidatos de dev 
* A contagem começa a partir do 0 - 0 = posição 1, 1 = posição 2 ... - fila[0]
* A fila tem a ordem 
* fila.push('doguinho.jpg') -> você pode acrescentar algo na fila diretamente do terminal 
* fila.shift(); -> tira o primeiro item da fila 
* fila é uma variável que pegamos um espaço da memória (array) 
* fila.push('doguinho.png') -> adiciona alguem na fila 
* Diferença de array para estrutura de dado fila 
    #### Quando temos uma estrutura de dado temos uma representação para ficar mais fácil criar novas filas (como uma receita)
    * Receita para criar a fila 
        * Criar uma estrutura para trabalhar com o dado que ajuda a criar a fila 
        * enqueue - enfileira
        * dequeue - desenfileira 
* Para criar objetos é só chegar e criar { nome: 'Mário', idade: 24, andar() {} } -> dentro do navegado você consegue definir como é a receita de criar um objeto pela forma literal 
* Para criar um objeto a a partir de uma receita é uma classe 
* Daria para cirari uma fila com var push e shift -> mas seria muito mais complexa
* Quando você usa uma classe fica mais organizado e padronizado 

# Designs First e principior 
* Primeiro pensar em qual vai ser o design do código para ajustar a implementação para saber como criar 
* Pesquisar legal isso depois kkk
* Princípio do Open Closed - aberto para extensão e fechado para modificação
* Refactoring - Martin Fowler - aprendendo a aperfeçoar os designs de código 
* Uma fila é uma estrutura de dados que funciona para resolver todas as filas e dados que precise, não sobrecarregar o banco de dados, comprar ingressos. 

# Histórico do Navegador 
* Tudo que você navegou ele guarda, pode ir para uma expecífica, pode voltar para o futuro e quando você volta e vai para um site novo ele apaga todo o hitórico 
* LIFO - Last in, First Out 
* como simular o histórico 
* Stackoverflow - erro que acontece quando um programa tenta usar mais espaço do que o disponível na pilha das chamadas, falha do programa.
*  http://latentflip.com/ -> Loupe is a little visualisation to help you understand how JavaScript's call stack/event loop/callback queue interact with each other.
    * Simula como o JS esta rodando por baixo dos panos 
      * function bla() {
    console,log('Primeiro Log');
    console,log('Segundo Log');
    bla();
        }

    bla(); 
    -> exemplo de overflow e erro 

*history.push -> os sites que foram visitados 
* history.back/pop -> volta no anterior 
* Ao inves de usar a função do array com o histórico onde todo mundo pode entrar no console e modificar usa de outra forma para que ngm consiga 
* history.back(); -> tira algo da lista 
* A pilha trabalha no sistema last in first outr 
* no JS isso funciona no momento de empilhar as requisições e saber quando vao ocorrer as coisas
* No navegador trabalha como histórico 
     * o problema é mias complexo do que a estrutura padrão da pilha 

* history api - mdn -> documentação da web 
* https://developer.mozilla.org/en-US/docs/Web/API/History_API
* Saber como roda por baixo dos panos 

# Test Driven Development (TDD)
* Map - MDM - https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Map
    *Quokka,js - extensão 
    * ctrl+shift+P - New Quokka Java script FIle 
    * mostra o print do código ao lado dele 
    * como visualizar o problema de uma forma melhor 
    * escrever e testar ao longo para ver o que deu errado 

# Map e Set
* MAP - Uma estrutura de dados pronto. Basicamente é uma lista 
* Tem sempre uma chave e um valor 
* Exemplo 
    * Ao tentar acessar várias vezes o mesmo site, ao invès de poluir com vários acessos, ele mostra como se só tivesse acessado uma única vez; 
    * Cria uma chave para definir esse item em uma lista, atavez de um critério criado. 
    * nao importa quantos coloque no meio, ele sempre evitará duplicata, para evitar spam
    * Ele sempre sobresceve com os dados do ultimo 
    * Como não consumir tanta memória do usuário 
* Set - 
    * salvar tags e palavras chaves do usuário - para pesquisar depois 
    * remover tags repetidas 
    