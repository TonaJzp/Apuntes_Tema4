# ⚙️ Optimización y refactorización de código

Optimizar el código significa **mejorarlo internamente sin cambiar su comportamiento externo**. El objetivo es hacerlo más **legible, mantenible, eficiente y profesional**. En Java (y cualquier otro lenguaje), esto es una parte clave del desarrollo de software de calidad.

---

## 🧠 ¿Qué es la refactorización?

La refactorización es el proceso de:
- **Reescribir el código sin alterar lo que hace**.
- Eliminar duplicaciones, mejorar nombres, simplificar estructuras.
- Preparar el código para nuevas funcionalidades.

> Refactorizar ≠ optimizar rendimiento. Es mejorar la estructura interna.

---

## 🎯 Beneficios de la refactorización

- Aumenta la claridad del código.
- Reduce errores futuros.
- Facilita las pruebas.
- Mejora la colaboración entre desarrolladores.

---

## 🧱 Ejemplo antes y después

### Código antes de refactorizar:

```java
System.out.println("Bienvenido");
System.out.println("Acceso concedido");
```

### Código después (extracción de método):

```java
saludar();

public void saludar() {
    System.out.println("Bienvenido");
    System.out.println("Acceso concedido");
}
```

---

## 🧰 Patrones comunes de refactorización

| Patrón | Descripción |
|--------|-------------|
| Extraer método | Convertir fragmentos repetidos en métodos |
| Renombrar variable | Dar nombres significativos |
| Inline variable | Eliminar variables innecesarias |
| Separar responsabilidades | Dividir clases muy grandes |
| Eliminar código muerto | Borrar lo que no se usa |

---

## 🔧 Herramientas de ayuda a la refactorización

- **IntelliJ IDEA** → Refactor > Rename / Extract Method
- **Eclipse** → Refactor > Extract Local Variable
- **VS Code** → Con extensiones de Java y atajos
- O manualmente, revisando tu propio código con buenas prácticas

---

## 🧪 Refactorización y pruebas

Refactorizar **no debe cambiar el comportamiento**. Por eso, se recomienda siempre tener **pruebas automatizadas antes y después** del proceso.

### Ejemplo de prueba unitaria:

```java
@Test
public void testSaludo() {
    assertEquals("Bienvenido", saludo());
}
```

Si la prueba sigue funcionando tras refactorizar, el cambio fue seguro.

---

## 📋 Tipos de pruebas en el desarrollo

- **Pruebas unitarias**: prueban métodos individuales.
- **Pruebas de integración**: verifican que los módulos funcionen juntos.
- **Pruebas del sistema**: validan el software completo.
- **Pruebas de regresión**: aseguran que un cambio no rompe lo anterior.
- **Pruebas de aceptación**: garantizan que cumple los requisitos del cliente.

---

## 📐 Medidas de calidad del software

| Medida | Qué evalúa |
|--------|-------------|
| Complejidad ciclomática | Nº de decisiones (if, for, etc.) en el código |
| Acoplamiento | Grado de dependencia entre clases |
| Cohesión | Qué tan relacionadas están las funciones de una clase |
| Cobertura de pruebas | % del código que se ejecuta en los tests |

---

## 🔍 Herramientas de análisis de calidad

- **SonarQube** – Analiza calidad y seguridad del código.
- **Checkstyle** – Revisa estilo y normas en Java.
- **PMD** – Detecta patrones peligrosos o mal uso del lenguaje.
- **JaCoCo** – Mide cobertura de pruebas.

---

## 🏅 Normas y certificaciones

- **ISO/IEC 25010**: define atributos de calidad del software.
- **CMMI (Capability Maturity Model Integration)**: niveles de madurez en desarrollo.
- **IEEE 829**: estándar para documentación de pruebas.
- **ISO 9126** (reemplazada por 25010): modelo de calidad previo.

---

## 📚 Recursos recomendados

- [Refactoring.Guru](https://refactoring.guru/es)
- [Documentación de JUnit](https://junit.org/junit5/docs/current/user-guide/)
- [SonarQube](https://www.sonarqube.org/)
- [Checkstyle para Java](https://checkstyle.sourceforge.io/)

---

## ✅ Buenas prácticas de optimización

- Refactoriza **después** de hacer que funcione.
- Usa nombres claros: métodos, clases y variables.
- Mantén las clases pequeñas y enfocadas.
- Prueba continuamente.
- Automatiza análisis de calidad.

---

## 📌 Conclusión

La optimización no es solo cuestión de velocidad. Es cuestión de claridad, estructura y calidad. Refactorizar el código y garantizar su calidad es una habilidad clave de todo buen programador.

---

**Autor:** Tona Jzp  
**Proyecto:** Apuntes Tema 4 - Optimización y refactorización  


