# Dart

## 1. Conceptos básicos

El lenguaje *Dart*, es un lenguaje de programación fuertemente tipado, esto significa que cada variable del lenguaje que posea un tipo no podrá comportarse como una variable de otro tipo distinto al que fue definido para ella (a excepción de cuando se hace conversión de tipo). Además, es un lenguaje de *Programación Orientada a Objetos* (POO), lo que significa que para *Dart* cada valor es un objeto, incluso un simple número. 

### 1.1. Tipos

*String* = Se refiere a un formato de texto. El valor de una variable *String* debe encontrarse dentro de comillas (simples o dobles).

```dart
String saludo = 'Hola mundo';
```

*int* = Se refiere a valores numéricos de carácter entero. El valor de una variable *int* debe ser un número y no va acompañado de comillas. 

```dart
int numero = 22;
```

*float/double* = Se refiere a valores numéricos de carácter decimal. El valor de una variable *double* debe ser un número y no va acompañado de comillas. 

```dart
double numeroDecimal = 2,54;
```

*bool* = Se refiere a valores binarios. Se utiliza para determinar si un valor es verdadero o falso a través de las palabras clave *true* y *false*, no se acompañan con comillas.

```dart
bool = true;
```

*dynamic* = Se refiere a valores no tipados. Se asume que un valor es *dynamic* cuando se define como tal o cuando por el contrario la variable no ha sido definida con ningún tipo. Un valor *dynamic* puede asumir valores *int*, *String*, *double* u otros según sea requerido. 

```dart
dynamic noTipado = 3.1415;
```

*var* = Es un tipo diseñado para almacenar valores variables. Se utiliza para almacenar un valor que es, por ejemplo, el resultado de una función. A través de la *inferencia de tipo*, *Dart* puede inferir el tipo de dicha variable en función de los valores que admite. Solo debe usarse para declarar variables inicializadas. Para variables que no se han inicializado es recomendado usar un tipo específico. 

```dart
var resultado = sumarNumeros (1, 2.4);
// var detecta que los valores interactuantes son int y double. Por lo tanto, asume el tipo del valor más amplio, en este caso, double.
```

### 1.2. Funciones

*Dart* en términos de su sintaxis posee muchas similitudes con otros lenguajes fuertemente tipados, como por ejemplo *JavaScript*. 

Ejemplos de un función:

```dart
int sumarNumeros (int num1, int num2){ // la funcíon da como resultado un valor entero (int).
return num1+num2; // return define el valor que retornará la función una vez sea llamada.
}
```

```dart
void sumarNumeros (double num1, double num2){ // una función void no retorna ningún valor.
print(num1+num2); // imprime (en consola) el valor de la suma.
}
```

```dart
void main (){ // main es un nombre de función especial, es donde inicia la ejecución del código.
sumarNumeros (1,3); // llama a la función sumarNumeros para que sume los valores 1 y 3.
print(sumarNumeros(4,7)); // imprime en consola el resultado de la función con los valors 4 y 7.
}
```

### 1.3. Clases

Las clases, al igual que en otros lenguajes, son planos o moldes de un objeto que permiten almacenar un conjunto de valores independientemente de su tipo. Por lo tanto para crear (instanciar) un objeto de tipo *X*, es necesario primero crear una clase de tipo *X*. Una clase puede ser definida con valores para cada una de sus variables, los cuales pueden ser sobrescritos más adelante, o idealmente, pueden ser creadas sin valores para sus variables.

Ejemplos de clase:

```dart
class Persona { // el nombre de una clase debe empezar con mayúscula.
    String nombre;
    String sexo;
    int edad;
}

// En este caso, las variables son declaradas con tipado porque no se han inicializado. 
```

```dart
class Persona {
var nombre = 'Luis';
var sexo = 'Masculino';
var edad = 29;
}
// En este caso, como las variables han sido inicializadas, es posible usar el tipo var para que Dart haga inferencia de tipo. 
```

```dart
void main(){
var p1 = Persona(); // crea un objeto persona (no es necesario el 'New').
p1.name = 'Garbarichi'; // sustituye el nombre por defecto (si lo hubiera) por 'Garbarichi'.
}
```

