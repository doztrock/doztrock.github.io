
## CONDICIONALES

Los condicionales pueden tener esta forma, usando la sentencia `if`:

```java
int a = 1;

if (a = 0) {
    point(50, 50);
}
```

Lo que se hace es evaluar la condición expresada entre paréntesis y, 
si es cierta, ejecutan las instrucciones indicadas entre llaves. 

Lo cual podríamos analizarlo como:  

> Sí la variable `a` es igual a 0, dibujar un punto en las coordenadas (50, 50). 

Si la condición no se da, las instrucciones no se ejecutan. Para ejecutar unas u otras instrucciones dependiendo de si una condición se cumple o no, podemos usar la sentencia `else`:

```java
int a = 1;

if (a = 0) {
    point(50, 50);
} else {
    ellipse(50, 50, 100, 100);
}
```

Lo cual podríamos analizarlo como: 

> Si la variable `a` es igual a 0, dibujar un punto, en caso contrario dibujar una circunferencia.

Para evaluar una serie de condiciones, usamos la sentencia `else if`:
```java
int a = random(10);

if (a < 3) {
    point(50, 50);
} else if (a > 6) {
    ellipse(50, 50, 100, 100);
} else {
    rect(10, 10, 90, 90);
}
```

Lo cual podríamos analizarlo como: 

> Sí la variable `a` es menor que 3, dibuja un punto. Si es mayor que 6, dibuja una circunferencia y sí ninguna de las dos condiciones es cierta, dibuja un cuadrado.

Los condicionales se pueden anidar, así si se da una primera condición, se puede evaluar si se cumple una segunda:

```java
int a = random(10);
int b = random(5);

if (a < 6) {

    if (b < 2.5) {
        point(50, 50);
    } else {
        ellipse(50, 50, 100, 100);
    }

}
```

Lo cual podríamos analizarlo como: 

> Si la variable `a` es menor que 6 y la variable `b` es menor que 2.5, dibujar un punto. Si la variable `a` es menor que 6 y la variable `b` no es menor que 2.5, dibujar una circunferencia; si a es mayor que 6, no hagas nada.

Para poder evaluar una serie de condiciones que queremos que se ejecuten cuando el valor de una variable coincida con el que le indiquemos, usamos la sentencia `switch`:

```java
switch (condicion) {

    case A:
        funcion_1();
        break;
    case B:
        funcion_2();
        break;
    case C:
        funcion_3();
        break;

}
```