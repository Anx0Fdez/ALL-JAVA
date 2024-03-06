# ***JAVA PARA IMBECILES***
### *by: [Anxo Fdez]*
#### *github: [Anx0Fdez](https://github.com/Anx0Fdez)*

---
## *Escritura y lectura de ficheros*
### `Escritura`

### `Lectura`


## *Genéricos*
*Te permite engloar todos los tipos de datos mediante el dato genérico `T`*
```java
public class Box<T> {
    private T t;
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
*Es una lista que almacena objetos o tipos de datos primitivos.*
```java
Coche audi = new Coche("Audi", "A3", 2000);
Coche mercedes = new Coche("Mercedes", "Clase A", 2000);

ArrayList<Coche> list = new ArrayList<>();
list.add(audi);
list.add(mercedes);
```
## *For each*
*El bucle for-each se utiliza para recorrer una colección de elementos.*
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
//array de 5 elementos
int[] a = new int[5];
//array de 5 elementos inicializado
int[] b = {1, 2, 3, 4, 5};

//introducir un valor en un array
a[0] = 1;
a[1] = 21;
a[2] = 13;
```
### *Array multidimensional*
```java
//array de 5 elementos
int[][] a = new int[2][3];
//array de 5 elementos inicializado
int[][] b = {{1, 2, 3}, {4, 5, 6}};
//introducir un valor en un array
a[0][0] = 1;
a[0][1] = 2;
a[0][2] = 3;
```
---
### `Recorrer un array`
```java
for (int i = 0; i < a.length; i++) {
    System.out.println(a[i]);
}
```
### `Ordenar un array`
```java
Arrays.sort(a);
```
### `Buscar un elemento en un array`
```java
Arrays.binarySearch(3);
```
---
## *Extends*
```java
public class Car extends Vehicle {
    private int espejos;
    // constructor con super
    public Car(String color, int maxSpeed, int espejos) {
        super(color, maxSpeed);
        this.espejos = espejos;
    }
}
```
## *MODIFICADORES DE ACCESO*
### `public` *El acceso a la clase, método o variable es ilimitado.*
### `private` *El acceso a la clase, método o variable es limitado.*
### `protected` *El acceso a la clase, método o variable es limitado, pero también se puede acceder a través de clases hijas.*
### `default` *El acceso a la clase, método o variable es limitado, pero también se puede acceder a través de clases del mismo paquete.*

## *Constructor*
### Constructor por defecto
- *Se utiliza para llamar metodos o atributos de la clase*
```java
//
public class Car {
    public Car() {
    }
}
```
### Constructor con parametrizado
- *Sirve crear un objeto con parametros o atributos*
- *Se utiliza para crear objetos*
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
- *El valor que va despues del case es le valor que tenemos que meter por teclado para que se ejecute*
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
### `while` Mientras se cumpla la condición  (true/false)
- *No se ejecuta si la condición es falsa*
- *Se ejecuta 0 o más veces*
```java
while (int a = 0, a < 10) {
    System.out.println(a);
    a++;
}
```
### `do while` Haz esto mientras se cumpla la condición (true/false)
- *Se ejecuta al menos una vez*
- *Se ejecuta 1 o más veces*
```java
do {
    System.out.println(a);
    a++;
} while (a < 10);
```
### `for`
- *El bucle for se ejecuta un número específico de veces establecido en el limite*
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