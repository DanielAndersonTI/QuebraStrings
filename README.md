# Conversor de CamelCase para Lista de Palavras

Este projeto implementa um método que converte uma string no formato CamelCase em uma lista de palavras, e inclui uma suíte de testes para garantir a funcionalidade do método. A implementação cuida de palavras com letras maiúsculas, letras minúsculas, números, caracteres especiais e siglas.

## Estrutura do Projeto

- **Pacote `com.quebraStrings`**: Contém a classe `ConverterCamelCase` com o método `converterCamelCase`, responsável por converter strings CamelCase em listas de palavras.
- **Pacote `com.testQuebraStrings`**: Contém a classe `TesSimplestCamelCase`, que inclui testes unitários com diversos cenários para validar o método `converterCamelCase`.

## Funcionalidades

O método `converterCamelCase` oferece as seguintes funcionalidades:

1. Converte uma string CamelCase em uma lista de palavras, onde cada palavra é minúscula, exceto para siglas (ex.: `HTML`, `CSS`).
2. Ignora palavras que começam com números.
3. Divide palavras quando encontra caracteres especiais, como hífen (`-`) ou sublinhado (`_`).

## Testes

Os testes foram desenvolvidos utilizando a biblioteca **JUnit 5**. Abaixo, estão os casos de teste cobertos:

- **testPalavraMinuscula**: Testa a conversão de uma palavra simples em minúsculas.
- **testPrimeiraLetraMaiuscula**: Testa a conversão de uma palavra onde apenas a primeira letra é maiúscula.
- **testMultiplasPalavras**: Verifica a conversão correta de uma string CamelCase com múltiplas palavras.
- **testStringVazia**: Verifica se a string vazia retorna uma lista vazia.
- **testUmCaractere**: Testa a conversão de uma string com um único caractere.
- **testEspacosEmBranco**: Verifica a conversão de uma string com apenas espaços em branco.
- **testHifen**: Verifica a conversão de uma string contendo hífens como separadores de palavras.
