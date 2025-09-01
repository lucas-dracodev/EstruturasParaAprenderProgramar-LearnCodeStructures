# Guia de Estruturas de Programação

Aqui iremos seguir a seguinte ordem: Condicionais → Estruturas de repetição → Procedimentos/Funções → Vetores → Matrizes.

Este guia apresenta os conceitos e exemplos de estruturas de programação em múltiplas linguagens:  
C, C++, C#, Java, JavaScript, Python, Ruby, PHP e Go.

---

# 1️⃣ Estruturas Condicionais

**Conceito:**  
Permitem executar blocos de código dependendo de condições lógicas (verdadeiro/falso).  
São essenciais para tomada de decisão em programas.

| Estrutura | Descrição | Linguagens / Particularidades |
|-----------|-----------|------------------------------|
| if / if-else / if-elif-else | Executa código se a condição for verdadeira. Pode ter ramificações. | Python usa `elif` no lugar de `else if`. |
| switch / match-case | Seleção múltipla baseada no valor de uma variável. | Python usa `match-case`. Algumas linguagens não têm switch (ex: Ruby). |

### Exemplos de If / Else

```c
// C, C++, C#
int x = 10;
if(x > 5) {
    printf("Maior que 5\n");
} else if(x == 5) {
    printf("Igual a 5\n");
} else {
    printf("Menor que 5\n");
}
```
```java
// Java
int x = 10;
if(x > 5) {
    System.out.println("Maior que 5");
} else if(x == 5) {
    System.out.println("Igual a 5");
} else {
    System.out.println("Menor que 5");
}
```
```js
// JavaScript
let x = 10;
if(x > 5) {
    console.log("Maior que 5");
} else if(x === 5) {
    console.log("Igual a 5");
} else {
    console.log("Menor que 5");
}
```
```python
# Python
x = 10
if x > 5:
    print("Maior que 5")
elif x == 5:
    print("Igual a 5")
else:
    print("Menor que 5")
```
```ruby
# Ruby
x = 10
if x > 5
    puts "Maior que 5"
elsif x == 5
    puts "Igual a 5"
else
    puts "Menor que 5"
end
```
```php
// PHP
$x = 10;
if($x > 5) {
    echo "Maior que 5";
} elseif($x == 5) {
    echo "Igual a 5";
} else {
    echo "Menor que 5";
}
```
```go
// Go
x := 10
if x > 5 {
    fmt.Println("Maior que 5")
} else if x == 5 {
    fmt.Println("Igual a 5")
} else {
    fmt.Println("Menor que 5")
}
```

### Exemplos de Switch / Match-case

```c
// C, C++, C#
int n = 2;
switch(n) {
    case 1:
        printf("Um\n");
        break;
    case 2:
        printf("Dois\n");
        break;
    default:
        printf("Outro\n");
}
```
```java
// Java
int n = 2;
switch(n) {
    case 1 -> System.out.println("Um");
    case 2 -> System.out.println("Dois");
    default -> System.out.println("Outro");
}
```
```js
// JavaScript
let n = 2;
switch(n) {
    case 1:
        console.log("Um");
        break;
    case 2:
        console.log("Dois");
        break;
    default:
        console.log("Outro");
}
```
```python
# Python 3.10+
n = 2
match n:
    case 1:
        print("Um")
    case 2:
        print("Dois")
    case _:
        print("Outro")
```
```ruby
# Ruby
n = 2
case n
when 1
  puts "Um"
when 2
  puts "Dois"
else
  puts "Outro"
end
```
```php
// PHP
$n = 2;
switch($n) {
    case 1:
        echo "Um";
        break;
    case 2:
        echo "Dois";
        break;
    default:
        echo "Outro";
}
```
```go
// Go
n := 2
switch n {
case 1:
    fmt.Println("Um")
case 2:
    fmt.Println("Dois")
default:
    fmt.Println("Outro")
}
```
---

# 2️⃣ Estruturas de Repetição

**Conceito:**
Executam blocos de código várias vezes, controlando o fluxo por **contadores** ou **condições**.

## Principais Estruturas

- **for** → Laço com inicialização, condição e incremento/decremento.  
- **while** → Executa enquanto a condição for verdadeira.  
- **do-while** → Executa ao menos uma vez, depois repete enquanto a condição for verdadeira.  

---

### Tabela Comparativa

| Estrutura | Descrição | Observações |
|-----------|-----------|-------------|
| **for** | Laço com inicialização, condição e incremento/decremento | Python utiliza `for in range()` |
| **while** | Executa enquanto a condição for verdadeira | Igual em várias linguagens; em Python usa `:` |
| **do-while** | Executa ao menos uma vez, depois repete enquanto a condição for verdadeira | Python não possui `do-while` nativo |

---

### Exemplos de For
```c
// C, C++, C#
for(int i = 0; i < 5; i++) {
    printf("%d\n", i);
}
```
```java
// Java
for(int i = 0; i < 5; i++) {
    System.out.println(i);
}
```
```js
// JavaScript
for(let i = 0; i < 5; i++) {
    console.log(i);
}
```
```python
# Python
for i in range(5):  # 0 a 4
    print(i)
```
```ruby
# Ruby
for i in 0...5
    puts i
end
```
```php
// PHP
for($i = 0; $i < 5; $i++) {
    echo $i;
}
```
```go
// Go
for i := 0; i < 5; i++ {
    fmt.Println(i)
}
```
### Exemplos de While / Do-While
```c
// C, C++, C#
int i = 0;
while(i < 5) {
    printf("%d\n", i);
    i++;
}

int j = 0;
do {
    printf("%d\n", j);
    j++;
} while(j < 5);
```
```java
// Java
int i = 0;
while(i < 5) {
    System.out.println(i);
    i++;
}

int j = 0;
do {
    System.out.println(j);
    j++;
} while(j < 5);
```
```js
// JavaScript
let i = 0;
while(i < 5) {
    console.log(i);
    i++;
}

let j = 0;
do {
    console.log(j);
    j++;
} while(j < 5);
```
```python
# Python
i = 0
while i < 5:
    print(i)
    i += 1

# Simulação de do-while
j = 0
while True:
    print(j)
    j += 1
    if j >= 5:
        break
```
```ruby
# Ruby
i = 0
while i < 5
    puts i
    i += 1
end

j = 0
begin
    puts j
    j += 1
end while j < 5
```
```php
// PHP
$i = 0;
while($i < 5) {
    echo $i;
    $i++;
}

$j = 0;
do {
    echo $j;
    $j++;
} while($j < 5);
```
```go
// Go
i := 0
for i < 5 {
    fmt.Println(i)
    i++
}

// Simulação do do-while
j := 0
for {
    fmt.Println(j)
    j++
    if j >= 5 { break }
}
```

---

# 3️⃣ Procedimentos / Funções

**Conceito:**
Blocos de código reutilizáveis.
- Procedimento: executa ações, **não retorna valor**
- Função: executa ações, **retorna valor**

---

```c
// C, C++
void saudacao() {
    printf("Olá!\n");
}

int soma(int a, int b) {
    return a + b;
}
```
```java
// Java
void saudacao() {
    System.out.println("Olá!");
}

int soma(int a, int b) {
    return a + b;
}
```
```js
// JavaScript
function saudacao() {
    console.log("Olá!");
}

function soma(a, b) {
    return a + b;
}
```
```python
# Python
def saudacao():
    print("Olá!")

def soma(a, b):
    return a + b
```
```ruby
# Ruby
def saudacao
  puts "Olá!"
end

def soma(a, b)
  a + b
end
```
```php
// PHP
function saudacao() {
    echo "Olá!";
}

function soma($a, $b) {
    return $a + $b;
}
```
```go
// Go
func saudacao() {
    fmt.Println("Olá!")
}

func soma(a int, b int) int {
    return a + b
}
```

---

# 4️⃣ Vetores / Arrays

**Conceito:**
Estrutura de dados que armazena múltiplos valores do mesmo tipo, acessíveis por índice.

---

```c
// C
int numeros[5] = {1, 2, 3, 4, 5};
```
```java
// Java
int[] numeros = {1, 2, 3, 4, 5};
```
```js
// JavaScript
let numeros = [1, 2, 3, 4, 5];
```
```python
# Python
numeros = [1, 2, 3, 4, 5]
```
```ruby
# Ruby
numeros = [1, 2, 3, 4, 5]
```
```php
// PHP
$numeros = array(1, 2, 3, 4, 5);
```
```go
// Go
numeros := []int{1, 2, 3, 4, 5}
```

---

# 5️⃣ Matrizes / Arrays Multidimensionais

**Conceito:**
Estruturas que armazenam dados em múltiplas dimensões (linhas e colunas).

---

```c
// C
int matriz[2][3] = {{1, 2, 3}, {4, 5, 6}};
```
```java
// Java
int[][] matriz = {{1, 2, 3}, {4, 5, 6}};
```
```js
// JavaScript
let matriz = [[1, 2, 3], [4, 5, 6]];
```
```python
# Python
matriz = [[1, 2, 3], [4, 5, 6]]
```
```ruby
# Ruby
matriz = [[1, 2, 3], [4, 5, 6]]
```
```php
// PHP
$matriz = array(
    array(1, 2, 3),
    array(4, 5, 6)
);
```
```go
// Go
matriz := [][]int{{1, 2, 3}, {4, 5, 6}}
```

---

Copyright (c) 2025 Lucas Silva de Deus (Dr@c0)