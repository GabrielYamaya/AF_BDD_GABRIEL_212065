# Branch de testes

Imagine que você está planejando alugar um carro para uma viagem. Para facilitar esse processo, uma empresa de locação de carros desenvolveu um sistema com diferentes comportamentos, dependendo das circunstâncias da locação e do cliente.

Inicialmente, considere um cliente que deseja alugar um carro de luxo. Se esse cliente realizar a reserva com antecedência de pelo menos uma semana, o sistema deve oferecer um desconto especial no valor total da locação. Por outro lado, suponha um cliente que necessita alugar um carro utilitário de última hora, sem qualquer reserva prévia. Nesse caso, o sistema deve ainda conseguir encontrar um veículo disponível e processar a locação rapidamente, mesmo que isso implique em um custo um pouco mais elevado devido à demanda urgente.

## Feature:

## Cenário 1: Cliente Especial com saldo negativo
        Scenario: Cliente especial com saldo negativo
        Given Um cliente especial com saldo atual de -200 reais
        When for solicitado um saque no valor de 100 reais
        Then deve efetuar o saque e atualizar o saldo da conta para -300 reais
        And check more outcomes

## Cenário 2: Cliente comum com saldo negativo
        Scenario: Cliente comum com saldo negativo
        Given Um cliente comum com saldo atual de -200 reais
        When Solicitar um saque de 200 reais
        Then não deve efetuar o saque e deve retornar a mensagem Saldo Insuficiente

## Primeira Run:
![image](https://github.com/GabrielYamaya/AF_BDD_GABRIEL_212065/assets/117553594/37e9e6e7-f502-4fe8-b0ae-f11c7346ec33)

### Implementação: 
![image](https://github.com/GabrielYamaya/AF_BDD_GABRIEL_212065/assets/117553594/c9ef5ed5-47e6-4181-8f09-54f8697ef9cc)

### Teste do JUnit:
![image](https://github.com/GabrielYamaya/AF_BDD_GABRIEL_212065/assets/117553594/f23af9fd-15a3-4881-bafb-cb7c60d33702)


