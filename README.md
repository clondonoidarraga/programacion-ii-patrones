# Programación II — Patrones de Diseño

> Repositorio del curso de **Programación II** para estudiantes de Ingeniería de Sistemas.
> Implementaciones prácticas en Java de los patrones de diseño clásicos (GoF), con enfoque en **entender el problema antes que la solución**.

![Java](https://img.shields.io/badge/Java-17-blue)
![Maven](https://img.shields.io/badge/build-Maven-red)
![JUnit](https://img.shields.io/badge/tests-JUnit%205-green)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

---

## 🎯 Sobre este repositorio

Este repositorio agrupa **todos los ejercicios prácticos** del curso de Programación II. Cada carpeta es un proyecto Maven independiente que ilustra uno o más patrones de diseño aplicados a un dominio concreto, acompañado de su diagrama UML, código comentado línea por línea y pruebas con JUnit 5.

La secuencia está diseñada para ir de lo más simple a lo integrador: primero los patrones **uno por uno** (aislados, fáciles de estudiar), y al final **un proyecto integrador** donde varios patrones conviven — que es como realmente aparecen en software de producción.

## 🤔 ¿Por qué estudiar patrones de diseño?

Un patrón no es una librería, ni un framework, ni código que se copia-pega. Es una **solución probada a un problema recurrente** de diseño. Estudiarlos te da tres superpoderes:

1. **Vocabulario común.** Cuando dices "acá uso un Observer", el otro ingeniero entiende en 3 segundos lo que tomaría 10 minutos explicar.
2. **Diseño preventivo.** Reconoces problemas antes de codearlos y eliges la estructura correcta desde el inicio, evitando deuda técnica.
3. **Pensamiento de arquitecto.** Dejás de pensar "¿cómo hago que esto funcione?" y empezás a pensar "¿cómo hago que esto sea mantenible, extensible y testeable?".

## 📚 Contenido del repositorio

| # | Ejercicio | Patrón(es) | Estado |
|---|---|---|---|
| 01 | `01-singleton-configuracion` | Singleton | ⏳ En preparación |
| 02 | `02-factory-method-notificaciones` | Factory Method | ⏳ En preparación |
| 03 | `03-abstract-factory-ui` | Abstract Factory | ⏳ En preparación |
| 04 | `04-builder-pizzas` | Builder | ⏳ En preparación |
| 05 | `05-adapter-pagos` | Adapter | ⏳ En preparación |
| 06 | `06-decorator-cafeteria` | Decorator | ⏳ En preparación |
| 07 | `07-composite-archivos` | Composite | ⏳ En preparación |
| 08 | `08-proxy-seguridad` | Proxy | ⏳ En preparación |
| 09 | `09-observer-eventos` | Observer | ⏳ En preparación |
| 10 | `10-strategy-pagos` | Strategy | ⏳ En preparación |
| **11** | **`11-sonicwave-patrones-combinados`** | **Singleton + Factory Method + Composite + Decorator + Proxy** | ✅ Disponible |

> *Los ejercicios se liberan progresivamente a medida que se avanza el curso.*

## 🗂️ Estructura general

```
programacion-ii-patrones/
├── README.md                              ← Este archivo
├── 01-singleton-configuracion/
│   ├── pom.xml
│   ├── README.md
│   └── src/
├── 02-factory-method-notificaciones/
│   └── ...
├── ...
└── 11-sonicwave-patrones-combinados/      ← Proyecto integrador
    ├── pom.xml
    ├── README.md
    ├── docs/
    │   └── diagrama-clases.jpg
    └── src/
        ├── main/java/com/sonicwave/
        └── test/java/com/sonicwave/
```

Cada carpeta es **autónoma**: tiene su propio `pom.xml`, su README explicativo y sus tests. Podés abrirla directamente en IntelliJ IDEA o VS Code como un proyecto Maven independiente.

## 🛠️ Tecnologías

- **Java 17** (versión LTS, ampliamente usada en la industria)
- **Maven** (gestión de dependencias y build)
- **JUnit 5** (pruebas unitarias)
- **IntelliJ IDEA Community** o **VS Code** (IDEs recomendados — ambos gratuitos)

## 🚀 Cómo clonar y ejecutar

```bash
# Clonar el repositorio completo
git clone https://github.com/<tu-usuario>/programacion-ii-patrones.git
cd programacion-ii-patrones

# Entrar al ejercicio que quieras estudiar
cd 11-sonicwave-patrones-combinados

# Compilar
mvn compile

# Ejecutar los tests
mvn test

# Correr la demo (si el ejercicio tiene Main.java)
mvn exec:java -Dexec.mainClass="com.sonicwave.Main"
```

## 🎓 Metodología del curso

Cada ejercicio sigue el mismo recorrido pedagógico:

1. **Problema real.** Una situación concreta del mundo del software donde surge la necesidad.
2. **Solución ingenua.** El código que escribiría alguien sin conocer el patrón — y por qué termina doliendo.
3. **El patrón.** La estructura formal: diagrama UML, roles, responsabilidades.
4. **Implementación paso a paso.** Código comentado, decisión por decisión.
5. **Pruebas.** Tests unitarios que validan el comportamiento y enseñan a pensar en testabilidad.
6. **Discusión.** Cuándo SÍ y cuándo NO usar el patrón. Alternativas. Antipatrones comunes.

## 👨‍🏫 Para docentes

Este repositorio está pensado para ser **reutilizable** por otros docentes:

- Cada ejercicio tiene su propio README con objetivos de aprendizaje.
- Los tests sirven como ejemplos de cómo evaluar aprendizaje automáticamente.
- Los diagramas UML están incluidos en `docs/` de cada proyecto.
- El código está documentado con Javadoc en español, pensado para estudiantes hispanohablantes.

Si usás este material en tu curso, ¡me encantaría saberlo! Abrí un *issue* o enviame un mensaje.

## ✍️ Autora

**Carolina Londoño Idárraga**
Máster en Inteligencia Artificial · Docente de Programación II
General Manager @ [Visualbit](https://visualbit.com.co) · Armenia, Quindío, Colombia

## 📖 Bibliografía recomendada

- Gamma, Helm, Johnson, Vlissides (1994). *Design Patterns: Elements of Reusable Object-Oriented Software*. Addison-Wesley. *(La "Gang of Four" — la referencia original.)*
- Freeman & Robson (2020). *Head First Design Patterns* (2ª ed.). O'Reilly. *(La forma más amable de empezar.)*
- Martin, Robert C. (2017). *Clean Architecture*. Prentice Hall.
- [refactoring.guru](https://refactoring.guru/design-patterns) — referencia online gratuita, con diagramas y ejemplos en múltiples lenguajes.

## 📄 Licencia

Este material se distribuye bajo licencia **MIT** para fines educativos. Eres libre de usarlo, modificarlo y compartirlo, citando la autoría.

---

*"Programs must be written for people to read, and only incidentally for machines to execute."* — Harold Abelson
