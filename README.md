# 📚 LiterAlura - Catálogo de Libros

Aplicación Java con Spring Boot que permite buscar, registrar y consultar libros usando la API pública de [Gutendex](https://gutendex.com). Toda la interacción se realiza desde la consola.

## 🚀 Tecnologías usadas

- Java 17
- Spring Boot
- Spring Data JPA
- PostgreSQL
- Jackson (para JSON)
- Maven

## ⚙️ Configuración del entorno

### 1. Instalar herramientas necesarias

- [Java JDK 17](https://adoptium.net)
- [PostgreSQL](https://www.postgresql.org/download/)
- [IntelliJ IDEA](https://www.jetbrains.com/idea/)
- Maven (viene con IntelliJ)

### 2. Crear base de datos en PostgreSQL

```sql
CREATE DATABASE literalura;
```

Asegúrate de que tu usuario y contraseña coincidan con el archivo `application.properties`:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/literalura
spring.datasource.username=postgres
spring.datasource.password=admin123
```

---

## 📦 Cómo ejecutar el proyecto

1. Abre IntelliJ IDEA
2. Selecciona `File > Open` y carga la carpeta del proyecto
3. Espera que Maven descargue las dependencias
4. Abre `LiteraluraApplication.java` y ejecuta con botón derecho → `Run`
5. Usa el menú en consola para interactuar

---

## 🎮 Funcionalidades principales

1. Buscar libro por título (vía API y guardar en base de datos)
2. Listar todos los libros registrados
3. Listar autores registrados
4. Listar autores vivos en un año dado
5. Listar libros por idioma
6. Validación para evitar libros duplicados
7. Manejo de errores si el libro no se encuentra

---

## 📂 Estructura del proyecto

```
literalura/
├── src/main/java/com/alura/literalura/
│   ├── LiteraluraApplication.java
│   ├── Principal.java
│   ├── dto/
│   ├── model/
│   ├── repository/
│   └── service/
├── src/main/resources/application.properties
├── pom.xml
```

---

## 🤝 Créditos

Desarrollado como parte del programa **Oracle Next Education** con [Alura Latam](https://www.aluracursos.com/).

---
