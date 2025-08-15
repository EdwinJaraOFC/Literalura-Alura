# 📚 Literalura - Alura Challenge

Este proyecto es una aplicación en Java desarrollada como parte del reto del programa **Alura Challenge - Oracle Next Education**. Permite buscar y listar libros utilizando la API pública de **Gutendex**, que ofrece un extenso catálogo de obras literarias en dominio público.

## 🚀 Funcionalidades
- **Menú interactivo por consola** para navegar entre las opciones.
- **Búsqueda de libros por título** con resultados obtenidos en tiempo real desde la API.
- **Listado de libros registrados** (ejemplo inicial con datos obtenidos de la API).
- Opciones en desarrollo:
  - Listar autores registrados.
  - Listar autores vivos en un determinado año.
  - Listar libros por idioma.
- Manejo de entradas y validaciones básicas.

## 🛠️ Tecnologías utilizadas
- **Java 17+**
- **HttpClient** (para consumir la API REST)
- **Gson** (para parsear JSON)
- Estructura modularizada en paquetes: `principal`, `model`, `service`

## 🏗️ Estructura del proyecto
```
src/
└── com.aluracursos.literalura
    ├── model           # Clases modelo que representan los datos obtenidos
    │   ├── Datos.java
    │   ├── DatosLibros.java
    │   └── ...
    ├── service         # Servicios para consumo de API y conversión de datos
    │   ├── ConsumoAPI.java
    │   └── ConvierteDatos.java
    └── principal       # Clase principal con menú y ejecución de la app
        └── Principal.java
```

## ⚙️ ¿Cómo ejecutar el proyecto?
1. Clona el repositorio:
   ```bash
   git clone https://github.com/tu-usuario/literalura.git
   cd literalura
   ```

2. Asegúrate de tener Java 17+ instalado:
   ```bash
   java -version
   ```

3. Compila y ejecuta desde la consola (o usando tu IDE preferido como IntelliJ o Eclipse):
   ```bash
   javac -d out src/com/aluracursos/literalura/**/*.java
   java -cp out com/aluracursos/literalura/principal/Principal
   ```

## 🔑 Sobre la API utilizada
Este proyecto consume datos desde:  
🌍 [https://gutendex.com/books/](https://gutendex.com/books/)  
No requiere autenticación ni clave de API para su uso.

## ✨ Posibles mejoras futuras
- Guardar los libros buscados en una base de datos local.
- Implementar filtros avanzados por idioma, autor o fecha.
- Añadir una interfaz gráfica (Swing o JavaFX).
- Manejo más robusto de excepciones y errores de conexión.

## 📚 Créditos
Desarrollado por **Edwin Junior** como parte del programa **Oracle + Alura LATAM**.

## 📝 Licencia
Este proyecto es de código abierto y puede ser adaptado libremente con fines educativos.
