# Pig Latin Translator

Este é um programa simples em Python que converte uma frase digitada pelo usuário em Pig Latin, que é um jogo linguístico que consiste em modificar as palavras de uma frase de acordo com uma regra específica.

## Como rodar o código

1. Certifique-se de ter o Python 3 instalado em sua máquina.
2. Abra o terminal e navegue até o diretório onde o arquivo `pig_latin_translator.py` está localizado.
3. Execute o comando `python pig_latin_translator.py` no terminal.
4. Digite uma frase quando solicitado pelo programa e pressione Enter.

## Como o código funciona

1. O programa pede ao usuário para digitar uma frase, que é armazenada na variável `original`.
2. A string é transformada em minúsculas e tem os espaços em branco removidos usando os métodos `strip()` e `lower()`.
3. A string é dividida em palavras individuais usando o método `split()` e armazenada em uma lista chamada `words`.
4. O programa entra em um loop `for` que percorre cada palavra da lista `words`.
5. Para cada palavra, ele verifica se a primeira letra é uma vogal (a, e, i, o, u). Se for, adiciona "yay" ao final da palavra e a armazena em uma nova lista chamada `new_words`.
6. Se a primeira letra não for uma vogal, o programa procura a primeira vogal na palavra usando um segundo loop `for` e armazena a posição em que ela é encontrada. Em seguida, separa a palavra em duas partes: uma parte com as consoantes iniciais (chamada de `cons`) e o restante da palavra após a primeira vogal (chamado de `the_rest`). Ele então une essas duas partes na ordem oposta e adiciona "ay" ao final da palavra. A nova palavra modificada é armazenada na lista `new_words`.
7. Depois que todas as palavras foram percorridas, o programa une todas as palavras na lista `new_words` de volta em uma única string usando o método `join()`, onde as palavras são separadas por um espaço em branco. Finalmente, a string resultante em Pig Latin é exibida usando a função `print()`.

## Observação

O projeto tem fins educativos e a língua utilizada no programa é fictícia. Projeto realizado na data 10/04/2023
