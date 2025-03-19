# TestUnitarioTeoria

### 🧪 **Diseño de Pruebas de Software** 🖥️

La etapa de pruebas es **esencial** en el desarrollo de software. Nos ayuda a asegurar que el producto final funcione correctamente y cumpla con los estándares de calidad. Aunque requiere tiempo, es una inversión que evita problemas costosos a futuro.

---

### 🧩 **¿Qué es un Caso de Prueba?** 🧩

Un **caso de prueba** es un escenario específico donde se verifica si una funcionalidad del programa se comporta como se espera.

#### Ejemplo 1: Videojuego �
- **Objeto de la prueba**: Asegurar que el personaje pierde una vida al caer al agua.
- **Caso de prueba**: Llevar al personaje a un punto donde caiga al agua y verificar que el nivel se reinicia.

#### Ejemplo 2: Función Matemática ➗
- **Objeto de la prueba**: Asegurar que `Math.abs(-7)` devuelve `7`.
- **Caso de prueba**: Ejecutar `Math.abs(-7)` y verificar que el resultado es `7`.

---

### 🎯 **Tipos de Pruebas según su Enfoque**

#### 1. **Pruebas de Caja Negra** 🖤
- **Qué se prueba**: Las salidas del sistema sin conocer su funcionamiento interno.
- **Enfoque**: "¿Qué hace el sistema?".
- **Ejemplo**: Probar una calculadora sin saber cómo está programada.

#### 2. **Pruebas de Caja Blanca** 🤍
- **Qué se prueba**: El flujo interno del programa (bucles, condicionales, etc.).
- **Enfoque**: "¿Cómo lo hace el sistema?".
- **Ejemplo**: Verificar que un método ejecuta correctamente todas sus condiciones.

---

### 📏 **Tipos de Pruebas según su Alcance**

#### 1. **Pruebas Unitarias** 🧱
- **Qué se prueba**: Una sección específica del código (por ejemplo, un método).
- **Herramientas**: 
  - JUnit (Java) 
  - PHPUnit (PHP) 
  - PyUnit (Python)
- **Ejemplo**: Probar un método que suma dos números.

#### 2. **Pruebas de Integración** 🔗
- **Qué se prueba**: La interacción entre diferentes módulos del sistema.
- **Ejemplo**: Verificar que una interfaz gráfica se comunica correctamente con la base de datos.

#### 3. **Pruebas de Usabilidad** 👥
- **Qué se prueba**: La experiencia del usuario al interactuar con la aplicación.
- **Ejemplo**: Observar cómo los usuarios realizan tareas específicas y detectar dificultades.

---

### 🛠️ **Herramientas: JUnit** 🧪

JUnit es un **framework** para realizar pruebas unitarias en Java. Permite escribir y ejecutar tests de forma organizada.

#### Ejemplo de Clase de Pruebas en JUnit:
```java
public class MatematicasTest {
    @Test
    public void testSuma() {
        assertEquals(5, Matematicas.suma(2, 3)); // Verifica que 2 + 3 = 5
    }
}
```

#### Anotaciones Comunes en JUnit:
- **@Test**: Indica que el método es una prueba.
- **@BeforeEach**: Se ejecuta antes de cada prueba.
- **@AfterEach**: Se ejecuta después de cada prueba.
- **@BeforeAll**: Se ejecuta una vez antes de todas las pruebas.
- **@AfterAll**: Se ejecuta una vez después de todas las pruebas.

---

### 📝 **Características de un Buen Caso de Prueba** ✅

1. **Prueba una sola cosa**: Cada caso debe enfocarse en una funcionalidad específica.
2. **Propósito claro**: Debe ser fácil entender qué se está probando.
3. **Independiente**: No debe depender de otros casos de prueba.
4. **Repetible**: Debe poder ejecutarse múltiples veces sin cambiar el resultado.

---

### 🔍 **Métodos de Prueba vs Casos de Prueba**

- **Método de Prueba**: Código que realiza una comprobación (por ejemplo, un método con `@Test`).
- **Caso de Prueba**: Escenario específico que se está probando (por ejemplo, "sumar 2 + 3 debe dar 5").

