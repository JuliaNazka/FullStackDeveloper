##FCA

#O que é base na programação 

#As empresas que melhor pagam em programação 
F - Facebook (meta) 
A- Amazon
A- Apple 
N - Netflix 
G - Google 
	* Cada uma delas tem o seu próprio modelo de negócio 
	* A maior parte de renda da amazon vem do uso e armazenamento de dados (AWS) 
		* Para aguentar a estrutura tão grande que precisavam criaram o AWS e foi to bom que resolveram comercializar como um novo meio. 

#A história 
ENIAC - um dos primeiros computadores, do tamanho de um andar que possuía a função de basicamente uma calculadora
A tecnologia está em constante evolução e otimização 
Ter uma base bem fundamentada para saber escolher e opinar sobre as peças de cada software. 
* Números sozinhos não dizem nada 
*Qual problema você quer resolver ?
	- Saber qual o problema para saber o que podemos resolver 

#Como a internet funciona
	* pede um requeste para o banco de dados através de um servidor e volta o response  
	*O servidor pode controlar o acesso, gerenciar  as informações - criar uma camada de segurança 

Cliente -> Servidor -> Base de dados 
Entrada -> Processo -> Saída 

#Conexão Client-Server 
Coisas que são síncronas e coisas que são assíncronas 
Acessar um site é uma operação síncrona - quando ele finaliza a operação ele fecha a ação (como se fosse uma ligação telefônica) 
Erro 500 - Erro interno do servidor (quando ele não consegue mais processar as informações) 
Existem códigos padrões que existem para mostrar os erros 

#Como resolver o problema de muitas pessoas tentando acessar um sistema 
Aumentar os sistemas pode ser uma solução - mas começa a aumentar a complexidade  (como garantir que os usuários vão entrar nele) - Load balancer - distribui os sistemas 

12FACTORS - metodologia de como fazer uma aplicação funcionar 

*Colocar mais pessoas aumenta a complexidade da comunicação 
“No silver  Bullet” - Frederick P. Brooks 

Escalonamento 

#Replicam a estrutura ao invés de colocar todos os clientes na mesma estrutura - Ex: Servidores de Games 
•	Escalonamento Vertical - Aumenta o tamanho do servidor - precisa de mais dinheiro 
•	Escalonamento Horizontal - Cria mais servidores pequenos - precisa de mais tempo e atenção 
•	Cada sistema vai desempenhar de uma forma baseado no histórico dele 
* Verificar os pontos de queda do aplicativo e ter atenção com o numero de usuários 

#Servidor 
•	Conteúdo estático -  texto, imagens - Claudflare - servidor para resolver esse problema - conteúdo que não muda
	* Faz o Cash do conteúdo e da o acesso para o usuário - Rede de distribuição de conteúdo 
•	Server Side Rendered - AWS - Contrata uma máquina de servidores (consegue calcular o quanto precisa de máquina) 
	* Monitorar constantemente os casos de erro - desligar os servidores 

#Fila e Performance
•	Alinhar os clientes que querem entrar no servidor por meio da fila e senha. 
	* Para não bater todas as pessoas de uma vez no sistema 
	* Não precisa gastar com o sistema para um numero maior de pessoas que pode receber 
		* Trade-off - pesar o que é mais importante 

#Porque determinado site trava somente no meu celular - Se a sua internet não tiver boa qualquer coisa mais pesada que você tenta usar não consegue 
	* O WhatsApp só entrega o texto da mensagem com baixo acesso a internet - ao invés de tudo 
Cada vez mais é necessário utilizar mais dados e informações 
Como otimizar a experiência 
	* Se demorar mais de 3 segundos para abrir a pessoa vai fechar o conteúdo 
	* Fazer um render otimizado  progressivo 

#Espera Passiva e Ativa  
Performace é UX 
•	Se o seu sistema for ruim o usuário final não vai querer mais utilizar o sistema 
•	O usuário precisa ter a sensação que o sistema é rápido 
•	A espera passiva é massante 
•	A espera ativa - pode ser um joguinho, algo para o usuário fazer 
	* Muitas empresas fazem isso e nem percebemos 
•	Utilizar um placeholder - parece que está progredindo o resultado - rodar uma animação 

“Além dos MILISSEGUNDOS - João Cunha”
“Perceived Perfformance - Fernanda Bernardo”

Como mostrar por meio de código e otimizar as performances - 26 dicas para otimização de sites 

Otimizar os códigos e sites , otimizar as imagens, diminuir a latência (a distância do servidor). 

#Performace de Computador 
•	Não precisa da ferramenta mais top antes de ganhar dinheiro com isso 
•	HDD x SSD x M2NVME - limites de velocidade, de compatibilidade 
•	Placas de Vídeo - emulador do pc consume mt ram e placa de. Vídeo - emular direto no celular 
•	A placa mãe possui as limitações dela 

#Princípios de Programação 
•	Dev Soutinhho - página do youtube do professor 
#Exercício 
• Dev 
	- Pedir uma informação 
	- Mostrar o resultado da idade 

• Usuário 
	- Digitar a informação 
	- Ver o resultado 

• Código 
	alert(2022-prompt('Quando você nasceu?'));
	
• Exemplo 2 da aula 
	- utilizar a variável 
	- Saber os valores que precisa para definir 
	- Para executar algo deve usar ()
	- Operações de soma e multiplicação no código 
	- function (hdhdhdh) { }
	- id="" - resgata em script um campo html
	- trabalhar com dinheiro é complexo no mundo da tecnologia - deve mostrar 2 casas para o usuário
	- == - compara um valor 
	- return; - não esquecer de para a função, se não ela executará infinitamente 
	- Usando api do google MAPs - https://github.com/googlemaps/google-maps-services-js

	Visto no exemplo - tópicos básicos para qualquer linguagem de programação que for trabalhar
	- 3 campos e um botão 
	- criação de variaveçl 
	- formatação de função 
	- parametro de função 
	- retorno de função 


resultado.toFixed(2); - traz para duas casas decimais o resultado 
resultado.toFixed(2).replace('.',','); - muda o . para , para chegar mais proximo da moeda brasileira 

NÃO TENHA MEDO DE ERRA AO TENTAR FAZER ALGO
