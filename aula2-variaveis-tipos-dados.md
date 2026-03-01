
Variáveis

Uma variável é um espaço na memória do computador reservado para armazenar um valor. Pense nela como uma caixa com uma etiqueta: a etiqueta é o nome da variável e o conteúdo da caixa é o valor que ela armazena. O valor de uma variável pode ser alterado durante a execução de um programa.

Tipos de Dados

Os tipos de dados especificam qual tipo de valor uma variável pode armazenar e quais operações podem
ser realizadas com ela. A escolha do tipo de dado correto é crucial para a eficiência e a correção do
programa.

Tipos Primitivos

Os tipos de dados primitivos são os mais básicos e fundamentais. Eles incluem:
• Inteiro: Para armazenar números inteiros, sem casas decimais. Exemplos: -10, 0, 150.
• Real (ou Ponto Flutuante): Para armazenar números com casas decimais. Exemplos: 3.14, -0.001,
15.5.
• Caractere (ou String/Texto): Para armazenar sequências de caracteres, como letras, números e
símbolos. Exemplos: "Olá, mundo!", "12345", "R$ 50,00".
• Lógico (ou Booleano): Para armazenar valores de verdade, que podem ser verdadeiro ou falso. É
fundamental para estruturas de decisão.

Tipos Compostos

Além dos tipos primitivos, existem tipos de dados mais complexos, que agrupam múltiplos valores. Os mais
comuns são:

Os tipos de dados em programação podem ser divididos em tipos primitivos (inteiro, real, texto, booleano)
e tipos compostos (vetores, matrizes, registros). Cada tipo possui características específicas para diferentes
necessidades de armazenamento.
• Vetores (Arrays): Coleções de elementos do mesmo tipo, acessados por um índice. Pense em uma lista
de compras ou em uma fileira de assentos no cinema.
• Matrizes: Estruturas bidimensionais, como uma tabela ou um tabuleiro de xadrez, onde os elementos
também são do mesmo tipo.
• Registros (Structs): Estruturas que agrupam variáveis de tipos diferentes em uma única unidade. Por
exemplo, um registro aluno pode conter um nome (texto), uma idade (inteiro) e uma media (real).

Operadores

Operadores são símbolos especiais que executam operações em operandos (variáveis e valores). Eles são a
base para a manipulação de dados em um programa.

Os operadores em programação são comumente organizados em três categorias: aritméticos (para cálculos
matemáticos), relacionais (para comparações) e lógicos (para operações booleanas). Cada operador possui
símbolo, descrição e função específica.

Operadores Aritméticos

Realizam operações matemáticas.
Operador Descrição Exemplo (a=10, b=3) Resultado
+ Adição a + b 13
- Subtração a – b 7
* Multiplicação a * b 30
/ Divisão a / b 3.33...
% Módulo (resto da divisão) a % b 1

Operadores Relacionais

Comparam dois valores e retornam um resultado booleano (verdadeiro ou falso).
Operador Descrição Exemplo (a=10, b=3) Resultado
== Igual a a == b falso
!= Diferente de a != b verdadeiro
> Maior que a > b verdadeiro
< Menor que a < b falso
>= Maior ou igual a a >= 10 verdadeiro
<= Menor o igual a b <= 3 verdadeiro


Operadores Lógicos

Combinam expressões booleanas para formar expressões mais complexas.

Operador 
(a=verdadeiro, b=falso)
Resultado
E (&&) Retorna verdadeiro se ambos
os operandos forem
verdadeiros
a E b
a && b
falso
OU (||) Retorna verdadeiro se pelo
menos um operando for
verdadeiro
a OU b
a || b
verdadeiro
NÃO (!) Inverte o valor do operando NÃO a
!a
falso
4.4.Operadores de Atribuição
Atribuem valores a variáveis. O operador de atribuição básico é o sinal de igual (=).
