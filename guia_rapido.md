# Guia Rápido de Estruturas de Programação

Versão prática e rápida para consulta. Comparativo de sintaxe entre linguagens.

## 1. Estruturas Condicionais

| Linguagem | If / Else | Switch / Match-Case |
|-----------|-----------|-------------------|
| C / C++ / C# | ```c if(cond){ } else if(cond2){ } else{ }``` | ```c switch(val){ case 1: break; default: }``` |
| Java | ```java if(cond){ } else if(cond2){ } else{ }``` | ```java switch(val){ case 1 -> ; default -> ; }``` |
| JavaScript | ```js if(cond){ } else if(cond2){ } else{ }``` | ```js switch(val){ case 1: break; default: }``` |
| Python | ```python if cond: elif cond2: else:``` | ```python match val: case 1: case _:``` |
| Ruby | ```ruby if cond elsif cond2 else end``` | ```ruby case val; when 1; else; end``` |
| PHP | ```php if($cond){ } elseif($cond2){ } else{ }``` | ```php switch($val){ case 1: break; default: }``` |
| Go | ```golang if cond { } else if cond2 { } else { }``` | ```golang switch val { case 1: default: }``` |

---

## 2. Estruturas de Repetição

| Linguagem | For | While | Do-While |
|-----------|-----|-------|-----------|
| C / C++ / C# / Java / JS / PHP | ```for(int i=0;i<5;i++){ }``` | ```i=0; while(i<5){ i++; }``` | ```i=0; do{i++;}while(i<5);``` |
| Python | ```for i in range(5):``` | ```i=0; while i<5: i+=1``` | ```i=0; while True: i+=1; if i>=5: break``` |
| Ruby | ```for i in 0...5``` | ```while i<5``` | ```begin; i+=1; end while i<5``` |
| Go | ```for i:=0;i<5;i++``` | ```i:=0; for i<5{i++}``` | ```i:=0; for {i++; if i>=5{break}}``` |

---

## 3. Procedimentos e Funções

| Linguagem | Procedimento | Função / Retorno |
|-----------|-------------|----------------|
| C | ```void proc(){}``` | ```int func(){return 1;}``` |
| C++ | Igual C | Igual C |
| C# | ```static void Proc(){}``` | ```static int Func(){return 1;}``` |
| Java | ```void proc(){}``` | ```int func(){return 1;}``` |
| JavaScript | ```function proc(){}``` | ```function func(){return 1;}``` |
| Python | ```def proc():``` | ```def func(): return 1``` |
| Ruby | ```def proc; end``` | ```def func; return 1; end``` |
| PHP | ```function proc(){}``` | ```function func(){return 1;}``` |
| Go | ```func proc() {}``` | ```func func() int{return 1}``` |

---

## 4. Vetores / Arrays

| Linguagem | Sintaxe |
|-----------|---------|
| C | `int v[5] = {1,2,3,4,5};` |
| C++ | Igual C ou `std::vector<int> v={1,2,3};` |
| C# / Java | `int[] v={1,2,3,4,5};` |
| JavaScript | `let v=[1,2,3,4,5];` |
| Python | `v=[1,2,3,4,5]` |
| Ruby | `v=[1,2,3,4,5]` |
| PHP | `$v=array(1,2,3,4,5);` |
| Go | `v:=[]int{1,2,3,4,5}` |

---

## 5. Matrizes / Arrays Multidimensionais

| Linguagem | Sintaxe |
|-----------|---------|
| C / C++ / C# | `int m[2][3]={{1,2,3},{4,5,6}};` |
| Java | `int[][] m={{1,2,3},{4,5,6}};` |
| JavaScript | `let m=[[1,2,3],[4,5,6]];` |
| Python | `m=[[1,2,3],[4,5,6]]` |
| Ruby | `m=[[1,2,3],[4,5,6]]` |
| PHP | `$m=array(array(1,2,3),array(4,5,6));` |
| Go | `m:=[][]int{{1,2,3},{4,5,6}}` |


---

Copyright (c) 2025 Lucas Silva de Deus (Dr@c0)