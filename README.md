# Calculadora IMC em MSTest

Esta calculadora IMC calcula o índice de massa corporal (IMC) de uma pessoa, de acordo com a fórmula:

IMC = peso / altura^2
O IMC é uma medida da relação entre o peso e a altura de uma pessoa. É um indicador de saúde geral, e valores de IMC fora da faixa normal podem indicar um risco aumentado de doenças.

## A calculadora IMC também classifica o IMC de uma pessoa em uma das seguintes categorias:

Abaixo do peso: IMC < 18,5
Peso normal: IMC >= 18,5 e IMC < 25
Sobrepeso: IMC >= 25 e IMC < 30
Obesidade Grau I: IMC >= 30 e IMC < 35
Obesidade Grau II: IMC >= 35 e IMC < 40
Obesidade Grau III: IMC >= 40

## Requisitos

.NET 6.0 ou superior
MSTest

## Instalação

dotnet new console -n CalculadoraIMC
cd CalculadoraIMC
dotnet add package MSTest

## Execução

dotnet test

## Testes

A calculadora IMC inclui testes automatizados para garantir que ela funcione corretamente. Os testes são escritos usando o MSTest.

### Para executar os testes, use o comando a seguir:

dotnet test

## Exemplo de uso

C#
// Cria um objeto IMC
IMC i = new IMC();

// Define o peso e a altura
i.peso = 80;
i.altura = 1.60;

// Calcula o IMC
i.Calcular_IMC();

// Exibe o IMC
Console.WriteLine(i.imc);

// Classifica o IMC
i.Classificar_IMC();

// Exibe a categoria do IMC
Console.WriteLine(i.categoria);
Use o código com cuidado. Saiba mais

### Este código produzirá o seguinte resultado:

31.25
Obesidade Grau I

## Observações

A calculadora IMC pode ser estendida para incluir outras funcionalidades, como a possibilidade de calcular o IMC de uma pessoa com base em outras unidades de medida.
Os testes da calculadora IMC podem ser melhorados para incluir mais casos de teste.
