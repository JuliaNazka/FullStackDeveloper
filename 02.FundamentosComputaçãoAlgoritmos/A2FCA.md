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

