# 🛠️ Prácticas Temas 9 y 10 - Entornos de Desarrollo

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white)
![Eclipse](https://img.shields.io/badge/Eclipse-2C2255?style=for-the-badge&logo=eclipse&logoColor=white)
![JUnit5](https://img.shields.io/badge/JUnit5-25A162?style=for-the-badge&logo=junit5&logoColor=white)
![SonarLint](https://img.shields.io/badge/SonarLint-CB2029?style=for-the-badge&logo=sonarsource&logoColor=white)

**Autor:** José Manuel López Montesinos  
**Curso:** 1º DAW  
**Módulo:** Entornos de Desarrollo  

---

## 📖 Descripción del Proyecto

Este repositorio contiene la resolución integral de las **5 prácticas** correspondientes a los temas 9 y 10. El objetivo principal de estos ejercicios es aplicar técnicas de aseguramiento de la calidad del software (Clean Code), abarcando desde la creación de pruebas unitarias y análisis de cobertura, hasta el análisis estático de código, refactorización automatizada y documentación técnica.

El proyecto original está desarrollado en **Java** utilizando el IDE **Eclipse**.

---

## 📂 Estructura del Repositorio y Ejercicios

La entrega está estructurada por ejercicios para facilitar su revisión. A continuación, se detalla el contenido y las tareas realizadas en cada uno de ellos:

### 1️⃣ Ejercicio 1: Tests Unitarios con JUnit 5
Se ha creado la clase principal y su correspondiente clase de pruebas (`Test`). Se han modificado los métodos de área y perímetro para cumplir con los requisitos de negocio:
- ✔️ Devolver `-1` si algún parámetro es negativo.
- ✔️ Devolver `0` si algún parámetro es igual a cero.

En la clase de test, se han cubierto todas las casuísticas posibles (valores positivos, negativos y ceros), incluyendo además una **aserción errónea a propósito** para verificar que el framework JUnit la detecta y hace fallar la prueba correctamente.

### 2️⃣ Ejercicio 2: Cobertura de Tests con EclEmma
Se ha ejecutado la herramienta EclEmma sobre los tests del Ejercicio 1 para verificar el grado de comprobación del código.
- **Resultado:** Se ha alcanzado un **100% de cobertura** en la clase principal.
- **Entregable:** En la carpeta de este ejercicio se adjunta el informe en formato HTML exportado desde Eclipse.

### 3️⃣ Ejercicio 3: Analizador de Código (SonarLint)
Se ha llevado a cabo un análisis estático del código empleando el plugin **SonarLint** para detectar posibles "code smells" o vulnerabilidades tempranas.
- **Entregable:** Se incluye un documento en formato PDF que contiene las capturas de pantalla de la ejecución de SonarLint en Eclipse, así como una investigación teórica detallando la relación, diferencias y casos de uso entre **SonarLint** y **SonarQube**.


### 4️⃣ Ejercicio 4: Refactorización en Eclipse
Partiendo del código inicial, se han aplicado de forma automatizada (mediante las herramientas *Refactor* de Eclipse) las siguientes mejoras de diseño, sin alterar el funcionamiento del programa:
1. **Extract Constant:** Se ha extraído el número `2` del cálculo del perímetro a una constante (`DOS`).
2. **Rename (Métodos):** Se han renombrado los métodos `area` y `perimetro` a su equivalente en inglés: `surface` y `perimeter`.
3. **Rename (Clase):** Se ha renombrado la clase principal de `Rectangulo` a `Rectangle`.
4. **Mantenimiento de tests:** Se han vuelto a ejecutar todos los tests de JUnit tras la refactorización, confirmando que el código sigue pasando todas las pruebas con éxito.

> ⚠️ *Nota técnica:* Las validaciones de valores (negativos y ceros) se han mantenido estructuradas de forma segura dentro de los métodos `surface` y `perimeter` en la versión final refactorizada.

### 5️⃣ Ejercicio 5: Documentación Automática (Javadoc)
Se ha documentado el código final refactorizado de la clase `Rectangle` siguiendo el estándar **Javadoc**.
- Se han incluido las etiquetas `@author` y `@version`.
- Se han documentado todos los parámetros (`@param`) y valores de retorno (`@return`) especificando las condiciones lógicas de los métodos.
- **Entregable:** La carpeta `doc` alojada en este repositorio contiene la página web generada automáticamente por la herramienta Javadoc de Eclipse.

---

## ✅ Requisitos Cumplidos
- [x] Nombre del repositorio correcto (`PRACTICAS-9-10-EED-2026`).
- [x] Implementación de pruebas unitarias.
- [x] Cobertura del 100%.
- [x] Informe comparativo SonarLint/SonarQube en PDF.
- [x] Código refactorizado a convenciones inglesas y constantes.
- [x] Documentación Javadoc generada.
- [x] Archivo README.md maquetado en Markdown.
