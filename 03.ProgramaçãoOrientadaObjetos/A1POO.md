# POO - Programação Orientada a Objetos 
 Prof Alessandro Dias 

## Introdução 
* A programação orientada a Objetos é um **paradigma de programação**
    * Foco em **objetos** em vez de funções 
    * Objetos -> São uma estrutura mais complexas que funções 
* Não é uma linguagem de programação nem uma ferramenta ou framwork(conjunto de classes de uma linguagem) 
* **É um estilo e paradigma de programação**

    ### 1. Motivação 
    * Muitas linguagens atualmente **implementam ou dão suporte** a Orientação a objetos 
        * C++
        * C# 
        * Java
        * **JavaScript**
        * Python 
        * Ruby 
    * Conhecer paradigmas é **Essencial** para qualquer desenvolvedor de software 

## Contextualização 
* Programação estruturada 
    * Criada em 1940 
    * Por muito tempo só existia esse método 
    * Paradigma com foco em 
        * Sequência (como ensinar o computador a fazer o que queremos) - uma instrução é executada após a outra
        * Decisão (tomar caminhos diferentes dentro do mesmo programa) - uma instrução executada após um teste lógico 
        * Iteração (repetir) - um trecho de código pode repetir após algum teste lógico 

*Livro - Conceitos da linguagem de programação (Robert Sebesta)* 

* Programação procedural 
    * Pegou alguns conceitos da estruturada e tentou facilitar 
    *  Paradigma com foco no uso de procedimentos e funções para **facilitar o reuso**
    * Não deve ter mais que 10 linhas 
    * Estruturas da programação estruturadas e **quebrar trechos de códigos em funções**
    * O programa sabe o que a função faz e pode chamá-la quando precisar 
        * Começa a segmentar e simplificar o código 
    * dependendo de como separar pode até usar a mesma função em outros programas 

*Livro - Código Limpo (Robert Cecil)* - Boas práticas na programação 

* Programação estruturada e procedural 
    * Consegue separar os dados das funções 
    * Código mais enxuto e reutilizável 
    * Continuam com várias funções soltas e dados espalhados pelo código 
        * Várias funções se chamam e criam funções espalhadas em vários locais de forma confusa 
        * ![alt text](image.png) - Grafo das funções (função espagheti)
    * Muito copia e cola de funções 
    * Mudanças em uma função resultam em mudanças em outras funções (dificuldade em descobrir onde estava o problema)
    * Interdependência entre as funções (uma depende da outra e precisa saber completamente o que ela faz)
    * funcionava, mas era muito complexo para dar manutenção no código 

*Ler a documentação do JS, StackOverflow*

## Programação Orientada a Objeto 
* Paradigma com foco no uso de objetos, onde cada um contém suas variáveis e funções 
* Construída em cima da programação estruturada e procedural 
    * Objeto A ( função dele (Conjunto de dados dele))
    * Objeto B ( função dele (Conjunto de dados dele))
    * ![alt text](image-1.png)
    * **Tudo o que é Dado do Objeto chama de atributo ou propriedade**
    * **Tudo o que é função se chama método** - pode retornar ou não algo 
    * Um objeto pode ou não ter variáveis ou atributos
* Objetos possui um conjunto de componentes 

* Componentes 
    * Diagrama de objetos - UML 
        * Nome (Dispositivo) - Diferenciar os objetivos 
        * Atributos (Fabricante, modelo) - informações, dados do objetos - representam o estado do objeto (o que é e o que representa)
        * Métodos ( Comportamentos, ligar, diminuirVolume) - ação (o que o objeto pode fazer)

## Objeto 
* Tem atributos, método e nome 
* Coleção de dados e funcionalidades que tem alguma relação entre si 
    * Dados -> variáveis (Atributos ou propriedades) -> Na Orientação a objetos tudo isso é a mesma coisa
    * Funcionalidades -> Funções (métodos, comportamentos)
* No **Java Script** atributos e métodos são membros de um objeto, cada um com um nome e um valor 
* Em JS Até o objeto vazio possui algo dentro dele 
* Um objeto em Js é composto por membros que tem **nome e valores** 
* Em Js tudo eventualmente vira um objeto 
* Em JavaScript, atributos e métodos são membros de um objeto, cada um com um nome e um valor
    * var nomeDoObjeto = {
        nomeMembro1: valorMembro1,
        nomeMembro2: valorMembro2,
        nomeMembro3: valorMembro3,
    };
    * var pessoa = {
        nome: "Valentina", idade: 60, saudar: function() { console.log("Olá");
        };
    }

## Atributo ou Propriedades 
* Um ou mais dados **presentes em um objeto**
* Entender como é a dinâmica de objetos e fazer o código fornecer o resultado esperado 
* Os objetos em JS tem uma anotação diferente 
* Possuem um nome único 
* Armazenam um **valor ou referência** 
### Acesso ao atributo de um objeto 
* Atribuição - acessível de duas formas 
* objeto.propriedade - 
* objeto ["propriedade"] - em JavaScript 
* é possivel acessar e trocar os valores com esse mesmo comando 

**Atributos, propriedade e variável são sinônimos neste caso**

## Método 
* Representa uma ou mais funcionalidades presentes em um objeto 
	* Fazem várias coisas
* Possuem um nome único 
* Representam uma lógica pertinente ao objeto 
### Acesso 
* Como acessar um método - só existe uma maneira 
* objeto.metodo(); 
* objeto.metodo(parametro); - se tiver parâmetro tem que mandar os parâmetros 
* objeto.metodo(parametro1, parametro2, ...); - colocar a lista de parametros na ordem que eles  aparecem 
**Uma função tem o seu código dentro das chaves**

## Criando um Objeto 
### Primeira forma 
* A primeira forma corresponde as formas já criadas nas atividades 1 a 5 - de forma literal 
* Como é - Como está sendo lido 
* Var nomeDoObjeto = { 
	nomeMembro1: valorMembro1,
	nomeMembro2: valorMembro2,
	nomeMembro3: valorMembro3,
	}; 
* Ex: 
Var pessoa = {
	nome: ['Fulano','de Tal'], -> nome é um vetor 
	anoDeNascimento: 1990, ->numérico 
	profissão:'Estudante',
	calculaIdade: function(){
		return new Date().getFullYear()-this.anoDeNascimento;  -> pega uma data e chama o método da nova data (data atual) - subtrai isso do ano de nascimento 
	}
};

	* Não importa o ano que está sempre retornará a idade atuall 

## Comprando POO com PE 
* Ao criar uma calculadora tornando as variáveis atributos e criando a função para a ação de soma 
* Coloca tudo dentro de um objeto 
* Com o POO o código fica um pouco mais protegico 
	* Fica mais organizado 
	* Muda o jeito de organizar a informação 
* Há maneiras melhores e mais elegantes de criarmos objetos 
* Em JavaScript **quase tudo são objetos**

## Tipo de Dados em JavaScript 
*  Os valores definidos para uma variável podem assumir domínios diferentes ao longo do tempo de execução do programa 
	* Uma string pode se tornar outra coisa se necessário 
* Tipos de Valor 
	* Tipos primitivos, não consegue quebrar mais que aquilo
* Tipos de Referência 
	* Tipos complexos, definidos por usuário 
	
### Tipos de valor 
* Representam valores imutáveis - uma coisa sempre será essa coisa
	* Number
	* String 
	* Boolean 
	* Symbol 
	* Undefined 
	* Null 
	
### Tipos de referência 
* Representam valores mutáveis e complpexos quando comparados com o tipo de Valor 
	* Object 
	* Function
	* array 
* É muito simples criar um objeto em JS e associar a lógica 

## Conceitos principais da Orientação a Objetos 
* 4 pilares que fundamentam a Orientação a OBJ 
1. Encapsulamento 
	* Agrupamento de atributos e métodos para manupular os dados de um objeto de forma eficiente 
	* Proteger os dados e atributos (por segurança, por domínio) 
	* Os outros paradgmas não possuem proteção dos dados 
	* Só expoe para o mundo externo só o que o programador define 
	* O objeto define se pode ou nao ser acessado atravéz de uma interface bem definida 
	* Saber o que um objeto faz e não como ele faz 
	* Os dados de um objeto estão dentro dele mesmo e até as funções de como ele se comporta (ver exemplo 6)
2. Abstração 
	* Exercício que fazemos a todo o momento 
	* Abstração digital da vida real 
	* POO possui um alto grau de abstração - fazer sentido com o mundo real 
	* Colocamos o que queremos representar no nosso problema - somente o que nos interessa para o problema 
	* Deixamos de lado o que não importa e foca no que precisa ser feito 
	* Exercicio de abstração 
		* Os atributos podem ser mutaveis ou não 
			* Carro : 
				* fabricante 
				* modelo
				* potência 
				* velocidade atual
		* Métodos permitem a alteração do estado 
			* Carro: 
				* ligar()
				* acelerar()
				* frear () 
				* retornam uma informação ou criam uma mudança no estado atual 
3. Herança 
	* Mecanismo que permite atributos e métodos compartilhados entre objetos 
	* reaproveita o código e agrupa o que é comuum a objetos diferentes 
	* diminui a quantidade de código espalhado 
	* Ajuda a eliminar redudâncias 
	* generalizar (todos fazem) ou especializar (alguns fazem) comportamentos ou informações 
	* Conceitos de herança - classificar para simplificar 
	* Usuário 
		* Atributos 
			* Id 
			* e-mail
			* senha 
		* Ações 
			* login()
			* trocarEmail()
			* trocarSenha()
		* Todos os usuários possuem essas informações 
	* Administrador 
		* é um usuário também mas possuem outras informações 
		* setor 
		* autorizar()
		* revogar()
		* bloquear()
4. Polimorfismo 
	* Muitas formas 
	* Polimorfismo e herança são a grande sacada do POO
	* Atravéz da herança é possivel alterar um comportamento herdado de um objeto Pai 
	* Permite a separação de interesses - cada objeto operador tem os seus interesses - cada 
	um tem os seus proprios interesses e se por acaso precise ser diferente para quem herdou ele 
	pode modificar o código 
	* Ajuda a deixar o código mais limpo (ao invés de usar vários Ifs) 
	* duas formas de fazer o polimorfismo 
		* **Sobrescrita**
			* pegar o mesmo método, o mesmo nome e a mesma assinatura(o método tem uma assinatura com o nome e o que ele faz) 
			* cria na classe filha - quando chamar chama o de baixo 
		* **Sobrecarga**
			* metodos com o mesmo nome, mas com diferentes assinaturas
			* Os parâmetros que ele recebe são diferentes 
			* **O JavaScript não suporta a sobrecarga**

* Vantagens e Ganhos 
	*Encapsulamento - redução da complexidade/ proteção de dados 
	*Abstração - redução da complexidade/ Maior reuso
	*Herança - Eliminar redudância no código 
	*Polimorfismo - Eliminar lógica desnecessária no código (simplificar e reduzir os ifs) 

* Trabalhando com objetos 
	* Criar objetos é como criar pokemons 
		* Cada um tem o seu tipo, lista de poderes, numeros na pokedex, matrix de evolução, quantidade de vida 
		
* Criando Objetos 
	* Literais 
		* cria usando {} - respeitando a sintaxe 
	* Funções Fábricas 
		* funções que são responsáveis por criar objetos - sem precisar criar varios na mão 
		* funções que criam e retornam objetos 
		* ex: 
			function criarPessoa() {
				return {
					nome: ['Fulano','de Tal'],
					anoDeNascimento: 1990,
					profissao: 'Estudante',
					calculaIdade: function() {
						return new Date().getFullYear()-this.anoDeNascimento;
					}
				};
			};
			
			const pessoa = criarPessoa();
			console.log(pessoa); 
			
		* é possivel automatizar ainda mais pegando os parâmetros e colocando como parametros da função 
			* ex: 
			function criarPessoa(nome, anoDeNascimento, profissao) {
				return {
					nome,
					anoDeNascimento,
					profissao,
					calculaIdade: function() {
						return new Date().getFullYear()-this.anoDeNascimento;
					}
				};
			};
			
			const pessoa = criarPessoa("Fulano", 1990, "Estudante");
			console.log(pessoa); 
			
			const pessoa1 = criarPessoa("Julia", 1999, "Arquiteta");
			const pessoa2 = criarPessoa("Manu", 2005, "Estudante");
			
		**Sintaxe sugar - resumir os códigos**
		
		
			
	* Funções Construtoras
	* Protótipos 
	* Classes 