# DIO - Trilha .NET - Fundamentos

www.dio.me

## Desafio de projeto

Para este desafio, você precisará usar seus conhecimentos adquiridos no módulo de fundamentos, da trilha .NET da DIO.

## Contexto

Você foi contratado para construir um sistema para um estacionamento, que será usado para gerenciar os veículos estacionados e realizar suas operações, como por exemplo adicionar um veículo, remover um veículo (e exibir o valor cobrado durante o período) e listar os veículos.

## Proposta

Você precisará construir uma classe chamada "Estacionamento", conforme o diagrama abaixo:
![Diagrama de classe estacionamento](diagrama_classe_estacionamento.png)

A classe contém três variáveis, sendo:

**precoInicial**: Tipo decimal. É o preço cobrado para deixar seu veículo estacionado.

**precoPorHora**: Tipo decimal. É o preço por hora que o veículo permanecer estacionado.

**veiculos**: É uma lista de string, representando uma coleção de veículos estacionados. Contém apenas a placa do veículo.

A classe contém três métodos, sendo:

**AdicionarVeiculo**: Método responsável por receber uma placa digitada pelo usuário e guardar na variável **veiculos**.

**RemoverVeiculo**: Método responsável por verificar se um determinado veículo está estacionado, e caso positivo, irá pedir a quantidade de horas que ele permaneceu no estacionamento. Após isso, realiza o seguinte cálculo: **precoInicial** \* **precoPorHora**, exibindo para o usuário.

**ListarVeiculos**: Lista todos os veículos presentes atualmente no estacionamento. Caso não haja nenhum, exibir a mensagem "Não há veículos estacionados".

Por último, deverá ser feito um menu interativo com as seguintes ações implementadas:

1. Cadastrar veículo
2. Remover veículo
3. Listar veículos
4. Encerrar

## Solução

### Função AdicionarVeiculo

- Verifica se a placa já esta cadastrada
- Se ja estiver imprime uma mensagem avisando que o veiculo já esta no estacinamento
- Se não estiver imprime uma mensagem falando que o veiculo foi adicionado e adiciona a lista usando o metodo List.Add

### Função RemoverVeiculo

- Verifica se existe carros estacionados usando o metodo List.any
- Imprime a lista com todos os carros estacionados para facilitar a escrita da placa
- Verifica se a placa digitada está na lista de carros estacionados
- Faz a conta do preço final com base nas horas digitadas
- Remove a placa da lista com o metodo List.Remove

### Função ListarVeiculos

- Verifica se existe carros estacionados
- Caso não tenha imprime uma mensagem falando que o estacionamento esta vazio
- Caso tenha veiculo as placas são impressas usando o metodo foreach
