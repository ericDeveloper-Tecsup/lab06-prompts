# Bitacora de prompts
 
Laboratorio 06: Fundamentos de Ingenieria de Prompts.
 
Herramienta de IA usada: (escribe aqui cual usaste)
 
## Ejercicio 2: Tokens y ventana de contexto

| Texto | Caracteres | Tokens |
|-------|------------|--------|
| Los estudiantes programan en Java. |34 | 7|
| The students program in Java. |29 | 6|
| desafortunadamente | 18| 4|

    En el paso 4 y 5 se verifica que segun el chat que se inicio, este guarda el contexto de la consulta, mientras que en un chat nuevo comenzamos con una pregunta y no tenemos contexto la IA te responde que no tiene informacion al respecto.

 
## Ejercicio 3: Temperatura

| Temperatura | % de BiblioTec | Nombres en los 5 intentos |
|-------------|----------------|---------------------------|
| 0 | 100| BiblioTec, BiblioTec, BiblioTec, BiblioTec, BiblioTec|
| 0.5 | 65.3| LibroYa, LibroYa, PrestaLibro, BiblioTec, BiblioTec|
| 1 | 44.5| LibroYa, BiblioTec, LibroYa, BiblioTec, BiblioTec|
| 1.8 |32.2 | PaginaLibre, LectoGo, BiblioTec, BiblioTec, LibroYa|

    El simulador nunca inventa un nombre nuevo porque solo puede escoger entre los nombres que ya están almacenados en el arreglo opciones; la temperatura cambia las probabilidades, pero no crea opciones nuevas.

## Ejercicio 4: Prompt vago vs estructurado

| Criterio | Prompt vago | Prompt estructurado |
|----------|-------------|---------------------|
| Menciona el objetivo del sistema |Si |Si |
| Menciona a los usuarios principales |No | Si|
| Tiene exactamente 3 funcionalidades |No |Si |
| Esta en 3 parrafos |No | Si|
| Lo usaria en un informe real |No |Si |

 
## Ejercicio 5: Anatomia de un prompt

| Componente | Texto de mi prompt |
|------------|--------------------|
| Rol | Actua como desarrollador Java |
| Instruccion |Usando una clase Producto con los atributos codigo, nombre, precio y stock |
| Contexto | Crea un programa en Java para gestionar los productos de una tienda.|
| Ejemplo | Usa este estilo para los metodos: getPrecio(), setPrecio(double precio)|
| Formato | Explica primero la estructura de la clase y luego presenta el codigo Java.|

