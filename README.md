# AF_BDD_GABRIEL_212065

Imagine que você está planejando alugar um carro para uma viagem. Para facilitar esse processo, uma empresa de locação de carros desenvolveu um sistema com diferentes comportamentos, dependendo das circunstâncias da locação e do cliente.

Inicialmente, considere um cliente que deseja alugar um carro de luxo. Se esse cliente realizar a reserva com antecedência de pelo menos uma semana, o sistema deve oferecer um desconto especial no valor total da locação. Por outro lado, suponha um cliente que necessita alugar um carro utilitário de última hora, sem qualquer reserva prévia. Nesse caso, o sistema deve ainda conseguir encontrar um veículo disponível e processar a locação rapidamente, mesmo que isso implique em um custo um pouco mais elevado devido à demanda urgente.

## Cenário de exemplo:

### Feature: Locação de carros


### Cenário 1: Aluguel de carro de luxo com antecedência
    Given um cliente deseja alugar um carro de luxo
    And o cliente reserva com antecedência de pelo menos uma semana
    When o cliente confirma a reserva
    Then deve reservar o carro
    And deve aplicar um desconto especial no valor total da locação


### Cenário 2: Aluguel de carro utilitário com demanada urgente
    Given um cliente deseja alugar um carro utilitário
    And o cliente solicita o carro com urgência de menos de uma semana
    When o cliente confirma a reserva
    Then deve encontrar um carro utilitário disponível
    And reservar o carro 
    And Aplicar um custo um pouco mais elevado no valor total da locação
  
