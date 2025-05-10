# Documentación con Javadoc

## ¿Qué es Javadoc?

Javadoc es una herramienta que permite generar documentación HTML de proyectos Java, a partir de comentarios especiales en el código.

## Comentarios Javadoc

```java
/**
 * Clase que representa un estudiante.
 */
public class Estudiante {
    private String nombre;

    public Estudiante(String nombre) {
        this.nombre = nombre;
    }

    public String getNombre() {
        return nombre;
    }
}
