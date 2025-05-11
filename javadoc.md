# 📄 Documentación de código con Javadoc

Javadoc es una herramienta incluida en el JDK (Java Development Kit) que permite **generar documentación en formato HTML** a partir del código fuente Java. Esta documentación se basa en **comentarios estructurados** insertados en el propio código.

---

## 🧠 ¿Por qué documentar el código?

Documentar el código:
- Facilita la comprensión de clases y métodos por otros desarrolladores (o por uno mismo en el futuro).
- Mejora el mantenimiento del software.
- Permite generar manuales de uso automáticos.
- Es fundamental para proyectos colaborativos y profesionales.

---

## 🛠 ¿Qué es Javadoc?

Javadoc es:
- Una herramienta incluida en el JDK.
- Un sistema de generación automática de documentación.
- Un estándar para proyectos Java de cualquier tamaño.

---

## 🖊 Sintaxis básica de un comentario Javadoc

Los comentarios de Javadoc siempre van justo antes de **clases, métodos o atributos** y tienen esta estructura:

```java
/**
 * Descripción general.
 * @etiqueta información
 */
```

---

## ✍️ Ejemplo completo de clase documentada

```java
/**
 * Clase que representa un estudiante de un curso.
 * Incluye nombre, edad y métodos para acceder a los datos.
 * 
 * @author Tona
 * @version 1.0
 */
public class Estudiante {

    private String nombre;
    private int edad;

    /**
     * Constructor del estudiante.
     * 
     * @param nombre Nombre del estudiante
     * @param edad Edad del estudiante
     */
    public Estudiante(String nombre, int edad) {
        this.nombre = nombre;
        this.edad = edad;
    }

    /**
     * Obtiene el nombre del estudiante.
     * 
     * @return El nombre como String
     */
    public String getNombre() {
        return nombre;
    }

    /**
     * Establece el nombre del estudiante.
     * 
     * @param nombre Nuevo nombre a asignar
     */
    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    /**
     * Muestra la información del estudiante en consola.
     */
    public void mostrarDatos() {
        System.out.println("Nombre: " + nombre + ", Edad: " + edad);
    }
}
```

---

## 🧷 Principales etiquetas Javadoc

| Etiqueta | Descripción |
|---------|-------------|
| `@author` | Nombre del autor |
| `@version` | Versión de la clase |
| `@param` | Parámetro de un método |
| `@return` | Valor devuelto por un método |
| `@see` | Referencia a otra clase o método |
| `@throws` | Excepción que puede lanzar el método |
| `@deprecated` | Marca el método como obsoleto |

---

## 🔧 Generar documentación con Javadoc (en consola)

### 📦 Requisitos:
- Tener instalado el **JDK**
- Tener los archivos `.java` bien comentados

### 🧪 Comando básico

```bash
javadoc Estudiante.java
```

Esto genera los archivos HTML de documentación en el mismo directorio.

---

## 📁 Especificar una carpeta de salida

```bash
javadoc -d doc Estudiante.java
```

El contenido generado estará en la carpeta `doc`.

---

## 💡 Añadir versión, autor y miembros privados

```bash
javadoc -d doc -author -version -private Estudiante.java
```

---

## 📸 Capturas recomendadas

Guarda tus capturas en `javadoc/img` y referencia aquí:

### 🔹 Comentarios Javadoc en el código

```text
Fragmento de clase Estudiante comentada
```
![comentarios](img/comentarios-javadoc.png)

### 🔹 Ejecución del comando en consola

```text
javadoc -d doc Estudiante.java
```
![javadoc-terminal](img/javadoc-generado.png)

### 🔹 Vista del HTML generado

```text
Captura del archivo index.html abierto en el navegador
```
![html](img/javadoc-html.png)

---

## 🧑‍🏫 Casos de uso en proyectos reales

- Bibliotecas públicas de Java (por ejemplo, Java Collections Framework).
- Proyectos de código abierto con documentación accesible.
- API internas de equipos de desarrollo.
- Manuales técnicos generados automáticamente.

---

## 🔍 Buenas prácticas con Javadoc

- Documentar todas las clases públicas y sus métodos.
- Usar descripciones claras y concisas.
- No repetir lo que ya es obvio por el nombre del método.
- Actualizar los comentarios si el código cambia.
- Generar documentación con cada versión del proyecto.

---

## 📚 Recursos recomendados

- [Documentación oficial de Javadoc](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/javadoc.html)
- [Tutorial Java - Uso de Javadoc (JavaTPoint)](https://www.javatpoint.com/javadoc-tool)
- [Guía completa de etiquetas Javadoc (Baeldung)](https://www.baeldung.com/javadoc)

---

## ✅ Conclusión

Javadoc es una herramienta fundamental para crear proyectos Java bien documentados. No solo mejora el trabajo en equipo, sino que también profesionaliza el código y facilita su uso y mantenimiento a largo plazo.

---

**Autor:** Tona Jzp  
**Proyecto:** Apuntes Tema 4 - Javadoc  
**Fecha:** Mayo 2025
