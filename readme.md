# Codigo de la tarea de algoritmos de cadenas en C++ y Python
## Codigo en c++ de diferentes tipos de cadena
```c++
#include <iostream>
#include <cstring>
#include <cctype>
using namespace std;
int main() {
	//ejemplo de como se usa strcpy
    char origen[] = "Hola";
    // Debe tener suficiente espacio para la copia
    char destino[20]; 
    // Copia la cadena origen en la cadena destino
    strcpy(destino, origen);
    // Imprime la cadena destino
    cout << "Copia: " << destino << endl;
	
	//ejemplo de como se usa strcat
    char palabra[50] = "Hola, ";
    char conc[] = "mundo";
    // Concatena la cadena conc a la cadena palabra
    strcat(palabra, conc);
    // Imprime la cadena destino
    cout << "Concatenar : " << palabra << endl;
    
    //ejemplo de como se usa strlen
    char cadena[] = "Hola, mundo";
    // Calcula la longitud de la cadena
    int longitud = strlen(cadena);
    // Imprime la longitud de la cadena
    cout << "Longitud de la cadena es: " << longitud <<endl;

	//ejemplo de como se usa strcmp
    char cadena1[] = "pizza";
    char cadena2[] = "pizzia";
    // Compara las cadenas 1 y 2
    int resultado = strcmp(cadena1, cadena2);
    if (resultado == 0) {
        cout << "Las cadenas son iguales." <<endl;
    } else if (resultado < 0) {
        cout << "cadena 2 es mayor que cadena 1" <<endl;
    } else {
        cout << "cadena 1 es mayor que cadena 2" <<endl;
	}

	//Ejemplo de como se usa Isalnum
    char caracter = 'E';
    // Verifica si el carácter es alfanumérico
    if (isalnum(caracter)) {
        cout << "El carácter '" << caracter << "' es alfanumérico." <<endl;
    } else {
        cout << "El carácter '" << caracter << "' no es alfanumérico." <<endl;
    }
    
    //Ejemplo de como se usa isalpha
    char caracteres[] = {'A', '1'};
    // Calculamos el número de elementos en el arreglo
    int num_caracteres = sizeof(caracteres) / sizeof(caracteres[0]);
    for (int i = 0; i < num_caracteres; i++) {
        char caracter = caracteres[i];
        if (isalpha(caracter)) {
            cout << "'" << caracter << "' es una letra del alfabeto." <<endl;
        } else {
            cout << "'" << caracter << "' no es una letra del alfabeto." <<endl;
        }
    }
    
	//como se usa isblank
    char espacio = ' ';
    if (isblank(espacio)) {
        cout << "'" << espacio << "' es un espacio en blanco." <<endl;
    } else {
        cout << "'" << espacio << "' no es un espacio en blanco." <<endl;
    }

	//ejemplo de como se usa substr
	string cad = "Buenas, tardes";
    // Extraer una subcadena que comienza en la posición 0 y tiene una longitud de 6 caracteres.
    string subcadena = cad.substr(0, 6);
    cout << "La subcadena es: " << subcadena << endl;

	//ejemplo de como se usa tolower
	char letraMayuscula = 'A';
    // Convierte la letra mayúscula 'A' a minúscula usando tolower.
    char letraMinuscula = tolower(letraMayuscula);
    cout << "La conversion a minuscula es: " << letraMinuscula << endl;

	//ejemolo de como se usa toupper
	char letraMin = 'a';
    // Convierte la letra minúscula 'a' a mayúscula usando toupper.
    char letraMay = toupper(letraMin);
    cout << "La conversion a mayuscula es: " << letraMay<< endl;
	
    return 0;
}
```
---
## Ejemplo en Python de diferentes tipos de cadenas
```py
#Ejemplo de capitalize
texto = "hola, mundo"
texto_capitalizado = texto.capitalize()
print(texto_capitalizado)

#Ejemplo de center
texto = "Python"
texto_centralizado = texto.center(20, "*")
print(texto_centralizado)

#Ejemplo de count
frase = "Python es un lenguaje de programación, y Python es divertido de aprender, y Python es mas facil de aprender"
contador_python = frase.count("Python")
print(f"La palabra 'Python' aparece {contador_python} veces en la frase.")

#Ejemplo de decode
cadena_bytes = b'Buenas, tardes'  # La 'b' antes de la cadena indica que es una secuencia de bytes codificada
cadena_decodificada = cadena_bytes.decode('utf-8')
print(cadena_decodificada)

#Ejemplo de encode
cadena = "Buenas, tardes"
bytes_codificados = cadena.encode('utf-8')
print(bytes_codificados)

#Ejemplo de endswith
nombre_archivo = "tarea.pdf"
resultado = nombre_archivo.endswith(".pdf")
if resultado:
    print(f"El nombre del archivo '{nombre_archivo}' termina con .pdf ")
else:
    print(f"El nombre del archivo '{nombre_archivo}' no termina con .pdf ")

#Ejemplo de expandtabs
texto_con_tabs = "Python\tes\tgenial."
texto_expandido = texto_con_tabs.expandtabs(4)
print("Texto original:")
print(texto_con_tabs)
print("Texto expandido:")
print(texto_expandido)

#Ejemplo de find
texto = "Hola, ¿cómo estás?"
posicion = texto.find(", ¿")
if posicion != -1:
    print(f"La subcadena ', ¿' comienza en la posición {posicion} de la cadena")
else:
    print("La subcadena ', ¿' no se encuentra en la cadena")

#Ejemplo de format
nombre = "Esau"
edad = 19
cadena_formateada = "Hola, soy {} y tengo {} años.".format(nombre, edad)
print(cadena_formateada)

#Ejemplo de lower
texto = "ESTA ES LA TAREA DE ALGORITMOS"
texto_en_minusculas = texto.lower()
print(texto_en_minusculas)

#Ejemplo de replace
texto = "Realizar la tarea en Python"
nuevo_texto = texto.replace("Python", "C++")
print(nuevo_texto)

#Ejemplo de split
frase = "La tarea es para el sabado"
palabras = frase.split()
print(palabras)
```
---
---
:sunglasses: :grin:
