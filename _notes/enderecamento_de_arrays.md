---
title: Endereçamento de arrays
---

_Oh, memory! You heartless bitch..._

Arrays são estruturas de dados lineares, isto é, estruturas de dados que armazenam os seus elementos em espaços contíguos na memória. Essa particularidade permite que os elementos sejam acessados em tempo constante, ou _O(1)_. 

Quando declaramos variáveis, o compilador ou interpretador da linguagem cria uma referência para essa variável em uma tabela de símbolos. Assim, toda vez que a variável é referenciada ao longo do programa, uma simples consulta na tabela de símbolos retorna o endereço associado ao nome da variável e, dessa forma, podemos alterar e acessar o valor lá armazenado.

Considerando que um array é uma coleção de elementos, criar uma referência para cada um dos elementos na tabela de símbolos seria pouco performático. Portanto, apenas o endereço do primeiro elemento é armazenado.

A pergunta a ser feita aqui é: como acessamos os demais elementos? Lembre que os elementos de um array são armazenados em posições contiguas na memória e, não só isso, arrays tradicionais impõem a restrição de apenas elementos de um mesmo tipo serem armazenados em um mesmo array. Como os elementos são do mesmo tipo, a quantidade de bytes utilizada para representar tais elementos também é a mesma. Tome como exemplo um array de inteiros. Cada inteiro ocupa 4 bytes. A partir do endereço base, basta realizarmos operações com ponteiros para avançarmos 4 bytes na memória e pronto: obtemos o endereço do segundo elemento. Uma fórmula genérica para endereçamento de arrays pode ser expressa como:

_a[i] = b + (i * s)_

_a[i]_, conhecida como notação de índice, referencia um elemento contido no array _a_, no índice _i_. O endereço base é expresso por _b_ e _s_ é o tamanho do tipo de dado do array.

Em um array do tipo:

`int a[i] = {7, 3, 12, 42, 9}`

Com o endereço base sendo _Ox1000_, o endereço do elemento 12 (que está no índice 2) pode ser calculado da seguinte forma:

_a[2] = 0x1000 + (2 * 4)_

Portanto, o endereço do elemento 12 é _0x1008_.

Essa abordagem tem sido usada por anos e funciona muito bem. No entanto, vamos imaginar um cenário onde fosse permitido diferentes tipos de dados serem armazenados em um mesmo array. Esse é o caso das listas em Python - um tipo de estrutura de dados que, embora não seja um array no sentido estrito, se comporta de uma forma semelhante.

A pergunta da vez é: se os elementos possuem tamanhos diferentes, como o endereçamento é calculado? E a resposta, como na maior parte dos assuntos envolvendo memória, é ponteiros!
