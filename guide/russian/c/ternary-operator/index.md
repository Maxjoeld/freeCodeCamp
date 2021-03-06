---
title: Ternary Operator
localeTitle: Тернарный оператор
---## Тернарный оператор

Программисты используют тернарные операторы в C для принятия решений вместо условных операторов **if** и **else** . Тернарный оператор является оператором, который принимает три аргумента. Первый аргумент - это аргумент сравнения, второй - результат при истинном сравнении, а третий - результат при ложном сравнении. Если это поможет вам думать о том, что оператор является сокращенным способом написания оператора if-else.

Вот простой пример принятия решений, используя **if** и **else** :

```c
int a = 10, b = 20, c; 
 
 if (a < b) { 
    c = a; 
 } 
 else { 
    c = b; 
 } 
 
 printf("%d", c); 
```

Этот пример занимает более 10 строк, но это необязательно. Вы можете написать вышеуказанную программу всего за 3 строки кода, используя **тернарный оператор** .

### Синтаксис

`condition ? value_if_true : value_if_false`

Утверждение evalutes к statement\_1, если условие истинно, и statement\_2 в противном случае.

Вот приведенный выше пример, переписанный для использования тернарного оператора:

```c
int a = 10, b = 20, c; 
 
 c = (a < b) ? a : b; 
 
 printf("%d", c); 
```

Результат примера должен быть:

```c
10 
```

`c` устанавливается равным `a` , так как условие `a<b` истинно.

Это выглядит довольно просто, не так ли? Обратите внимание, что `value_if_true` и `value_if_false` должны иметь один и тот же тип, и они не могут быть полными операторами, а просто выражениями.

Тернарный оператор может быть вложен так же, как вложенные операторы if-else. Рассмотрим это вложенное выражение if-else:

```c
int a = 1, b = 2, ans; 
 if (a == 1) { 
    if (b == 2) { 
        ans = 3; 
    } else { 
        ans = 5; 
    } 
 } else { 
    ans = 0; 
 } 
 printf ("%d\n", ans); 
```

Вот приведенный выше код переписан с использованием вложенного троичного оператора:

```c
int a = 1, b = 2, ans; 
 ans = (a == 1 ? (b == 2 ? 3 : 5) : 0); 
 printf ("%d\n", ans); 
```

Результат обоих вышеуказанных кодов должен быть:

```c
3 

```