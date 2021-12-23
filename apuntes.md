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
    ios::sync_whit_stdio(0);
    cin.tie(0);

    cout << "Ingresa el numero a: \n";
    cin >> a;
    cout << "El numero que ingresaste es: " << a;
}
```

En estos 