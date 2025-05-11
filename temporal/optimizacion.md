# Optimización de código

## Refactorización

Proceso de mejorar el código sin cambiar su comportamiento externo.

### Ejemplo: extraer método

Antes:
```java
System.out.println("Bienvenido usuario");
System.out.println("Cargando...");

saludar();

public void saludar() {
    System.out.println("Bienvenido usuario");
    System.out.println("Cargando...");
}

