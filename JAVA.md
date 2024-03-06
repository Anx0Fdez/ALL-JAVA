# ***JAVA PARA IMBECILES***
*by: [Anxo Fdez]*

*github: [Anx0Fdez](https://github.com/Anx0Fdez)*


## *Ecritura y lectura de ficheros*
### `Escritura`

### `Lectura`


## *Genéricos*
```java
public class Box<T> {
    private T t;[Programación](DAM%2FProgramaci%F3n)

    public void set(T t) {
        this.t = t;
    }

    public T get() {
        return t;
    }
}
```


## *Colecciones*
### `HashSet`
Un HashSet es una colección de elementos únicos. No puede haber elementos duplicados.
```java
HashSet<String> set = new HashSet<String>();
set.add("Apple");
set.add("Banana");
set.add("Mango");
```
### `TreeSet`
Un TreeSet es una colección de elementos únicos. Los elementos se almacenan en orden ascendente.
```java
TreeSet<String> set = new TreeSet<String>();
set.add("Apple");
set.add("Banana");
set.add("Mango");
```
### `HashMap`
Un HashMap es una colección de pares clave-valor. Cada clave es única y no puede repetirse. Cada clave está asociada a un valor.
```java
HashMap<String, String> map = new HashMap<String, String>();
map.put("Spain", "Madrid");
map.put("France", "Paris");
map.put("England", "London");
```
### `TreeMap`
Un TreeMap es una colección de pares clave-valor. Las claves se almacenan en orden ascendente.
```java
TreeMap<String, String> map = new TreeMap<String, String>();
map.put("Spain", "Madrid");
map.put("France", "Paris");
map.put("England", "London");
```


## *ArrayList*
```java
ArrayList<String> list = new ArrayList<String>();
list.add("Mango");
list.add("Apple");
list.add("Banana");
```
## *For each*
```java
for (String fruit : list) {
    System.out.println(fruit);
}
```


## *Interfaces*
`Una interfaz es una colección de métodos abstractos. Una clase implementa una interfaz, lo que significa que la clase proporciona una implementación para todos los métodos definidos en la interfaz.`
## *Clases abstractas*
`Una clase abstracta es una clase que no se puede instanciar. Se utiliza para definir clases que comparten algunas características comunes.`

## *Exceptions [try cach]*
```java
try {
    // código que puede lanzar una excepción
} catch (Exception e) {
    // código que se ejecuta si se lanza una excepción
} finally {
    // código que se ejecuta siempre
}
```

## *Arrays*
### *Array*
```java
int[] a = new int[5];
int[] b = {1, 2, 3, 4, 5};
```
### *Array multidimensional*
```java
int[][] a = new int[2][3];
int[][] b = {{1, 2, 3}, {4, 5, 6}};
```
---

---
#### *Recorrer un array*
```java
for (int i = 0; i < a.length; i++) {
    System.out.println(a[i]);
}
```
#### *Ordenar un array*
```java
Arrays.sort(a);
```
#### *Buscar un elemento en un array*
```java
Arrays.binarySearch(a, 3);
```

---


## *Extends*
```java
//con extends se hereda de la clase Vehicle
public class Car extends Vehicle {
    // ...
    //con super se llama al constructor de la clase padre
    super(a, b);
}
```



## *MODIFICADORES DE ACCESO*
### `public` *El acceso a la clase, método o variable es ilimitado.*
### `private` *El acceso a la clase, método o variable es limitado.*
### `protected` *El acceso a la clase, método o variable es limitado, pero también se puede acceder a través de clases hijas.*
### `default` *El acceso a la clase, método o variable es limitado, pero también se puede acceder a través de clases del mismo paquete.*

## *Constructor*
### Constructor por defecto
```java
public class Car {
    public Car() {
        System.out.println("Car is created");
    }
}
```
### Constructor con parametrizado
```java
public class Car {
    private String color;
    private int maxSpeed;

    public Car(String color, int maxSpeed) {
        this.color = color;
        this.maxSpeed = maxSpeed;
    }
}
```
##  *Métodos*
```java
//void: retorna nada
//() : no recibe parámetros
public class Car {
    public void drive() {
        System.out.println("Car is moving");
    }
}
```
##  *Crear y llamar objetos*
```java
public class Main {
    public static void main(String[] args) {
        // Crear un objeto
        Car car = new Car();
        // Llamar a un método
        car.drive();
    }
}
```

##  *Condicionales*
###  `If else`
```java
if (a > b) {
    System.out.println("a es mayor que b");
} else if (a < b) {
    System.out.println("a es menor que b");
} else {
    System.out.println("a es igual a b");
}
```
###  `Switch`
```java
switch (a) {
    case 1:
        System.out.println("a es 1");
        break;
    case 2:
        System.out.println("a es 2");
        break;
    default:
        System.out.println("a no es ni 1 ni 2");
        break;
}
```
##  *Bucles*
### `while`
```java
while (int a = 0, a < 10) {
    System.out.println(a);
    a++;
}
```
### `do while`
```java
do {
    System.out.println(a);
    a++;
} while (a < 10);
```
### `for`
```java
for (int a = 0; a < 10; a++) {
    System.out.println(a);
}
```

##  *Constantes*
Las constantes se declaran con la palabra reservada `final` y en mayúsculas.
```java
final int NUM = 10;
```


##  *Variables y tipos de datos*
```java
int a = 10;
float b = 10.5f;
double c = 10.5;
char d = 'A';
String e = "Hello";
boolean f = true;
```
##  *Clases*

```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Hello World");
    }
}
```