# Apuntes de programacion competitiva
Este es un repositorio sobre mis apuntes de programacion competitiva, tome en cuenta que estos están escritos para ser usados con c++ pero pueden ser usados con cualquier otro lenguaje.

## Leer y escribir datos
Tanto para leer y escribir datos, tenemos dos opciones, las cuales son **Archivos** y **Terminal**

### Leer y escribir desde TERMINAL

Para leer y escribir desde terminal hay varios comandos, pero a mi me gusta usar
- Para escribir ``cout``
- Para leer ``cin``   
Ambos del namespace ``std``, puesto que es muy sencillo de usar y no debes de formatear la lectura y escritura, veamos como se usan:
```cpp
#include <bits/stdc++.h>
using namespace std;

int a;

int main(){
    ios::sync_with_stdio(0);cin.tie(0);

    cout << "Ingresa el numero a: \n";
    cin >> a;
    cout << "El numero que ingresaste es: " << a;
}
```

En este ejemplo, la linea ``ios::sync_with_stdio(0); cin.tie(0)`` se encarga de acelerar la lectura/escritura de datos, la  verdad, a terminos tecnicos no se que es lo que hace, pero logra igualar los tiempos de ``printf`` y ``scanf``

Con ``cin >> a`` le estamos diciendo "Valmos a leer algo, y lo debemos de guardar en la variable a" debido a que la variable ``a`` de tipo entero, la entrada tambien lo será.

### Lectura/Escriura con ARCHIVOS

Es lo mismo que el ejempo anterior pero se le agregan las lineas 
```cpp
freopen("miArchivoLectura.txt", 'r', stdin);
freopen("miArchivoEscritura.txt", 'w', stdout);
```
al inicio de la funcion ``main()``, notese que para leer se usa ``'r'`` (read) y para escribir ``'w'`` (write), asi como ``stdin`` para leer y ``stdout`` para escribir.
