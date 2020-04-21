## SINTAXIS BASICA

Cualquier programa en Processing siempre debe contener dos funciones de manera obligatoria.

```java
void setup(){
}
void draw(){
}
```

En estas la funcion `setup()`se definen todos los elementos de los que se hara uso durante la ejecucion del programa.

```java
void setup(){
	// Definimos un tamaño de 800x600
	size(800, 600);
}
```

En este caso, cualquier parametro definido en `setup()` puede ser modificado dentro de la función `draw()`que es la funcion que se encuentra corriendo como un bucle infinito hasta la finalizacion del programa.

```java
void setup(){

	// Definimos un tamaño de 800x600
	size(800, 600);

	// Definimos un color de fondo
	background(0);

}

void draw(){

	// Redefinimos un color de fondo
	background(255);

}
```

En el caso anterior, definimos un color de fondo negro durante la funcion `setup()` y posteriormente lo sobreescribimos durante la funcion `draw()`en ese orden de ideas, la funcion `draw()`es la que está ejecutandose todo el tiempo, mas la funcion `setup()`solo se ejecuta una vez.

#### PALABRAS RESERVADAS

| Listado    |              |            |          |           |           |
|------------|--------------|------------|----------|-----------|-----------|
| abstract   | assert       | boolean    | break    | byte      | case      |
| catch      | char         | class      | const    | continue  | default   |
| double     | do           | else       | enum     | extends   | false     |
| final      | finally      | float      | for      | goto      | if        |
| implements | import       | instanceof | int      | interface | long      |
| native     | new          | null       | package  | private   | protected |
| public     | return       | short      | static   | strictfp  | super     |
| switch     | synchronized | this       | throw    | throws    | transient |
| true       | try          | void       | volatile | while     |           |

#### Comentarios

Para poder insertar comentarios dentro de Processing basta seguir la sintaxis de Java.

```java
/*
 * Este es un comentario
 * de varias
 * lineas
 */

// Este es un comentario de una linea
// Esta es otra linea
```