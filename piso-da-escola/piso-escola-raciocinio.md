# Questão Piso da escola

### Acesse a questão clicando [AQUI!](https://olimpiada.ic.unicamp.br/pratique/pu/2018/f1/piso/)

Na questão é pedido que se encontre o numero de lajotas do tipo 1 e do tipo 2.

Iremos começar com as lajotas do tipo 1, para encontrarmos um padrão basta contarmos quantas lajotas há no comprimento e como ela se alterna.

![](https://github.com/davialvb/OBI-solutions/blob/master/piso-da-escola/img/lajota1.png)

Pode-se notar que no comprimento temos 5 lajotas que se repetem por 3 vezes. Assim como se olharmos pela perspectiva da largura temos 3 lajotas que se repetem 5 vezes. Se multiplicarmos 3*5=15 já descobrimos aproximadamente 65% do numero de lajotas. Se olharmos as que sobram podemos mais uma vez observar um padrão.

![](https://github.com/davialvb/OBI-solutions/blob/master/piso-da-escola/img/lajota2.png)

Pode-se notar aqui que no comprimento temos 4 lajotas que se repetem por 2 vezes. Assim como se olharmos pela perspectiva da largura temos 2 lajotas que se repetem por 4 vezes. Se multiplicarmos esse valor teremos 2*4=8 que seriam o restante de lajotas para completarmos as 23. Note que aqui temos L-1 e C-1 multiplicados.

Aqui por dedução matematica temos:
```math
L*C + (L-1) * (C-1)
```

Agora para encontrarmos a solução para sabermos o número de lajotas do tipo 2 teremos mais uma vez que observar e encontrar um padrão.

![](https://github.com/davialvb/OBI-solutions/blob/master/piso-da-escola/img/lajota3.png)

Podemos iniciar somando os 2 grupos de 4 lajotas, 4+4=8. Aqui já é possível observar que C-1 + C-1 nos da o resultado esperado para esse grupo de lajotas.

![](https://github.com/davialvb/OBI-solutions/blob/master/piso-da-escola/img/lajota4.png)

Logo após podemos usar a mesma ideia somando os 2 grupos de 2 lajotas, 2+2=4. O que também já é possível observar que L-1 + L-1 nos da o resultado esperado para esse grupo. 
Ao final podemos somar tudo, ou seja (C-1 + C-1) + (L-1 + L-1).
Simplificando temos:
```math
 2*(C-1) + 2*(L-1)
 2C-2 + 2L-2
 2(C+L)-4 ou 2(C+L-2)
```
