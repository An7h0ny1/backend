# 🩺 Backend - Sistema de Gestión Clínica AURA
Este proyecto representa el backend del sistema de gestión de citas, pacientes y servicios de una clínica de terapias.

---

## 🚀 Tecnologías

| Componente        | Tecnología    | Justificación                          |
|-------------------|--------------|----------------------------------------|
| Lenguaje          | Java 17      | Familiaridad del equipo, robustez      |
| Framework         | Spring Boot  | Desarrollo rápido de APIs REST         |
| Base de Datos     | MySQL 8      | Relacional, conocimiento del equipo    |
| Autenticación     | JWT          | Seguridad para APIs                    |
| Control de Versiones | Git/GitHub | Colaboración eficiente                |

---

## 📁 Estructura del Proyecto

```bash
backend/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   ├── config/         # Configuraciones
│   │   │   ├── controllers/    # Controladores REST
│   │   │   ├── models/         # Entidades
│   │   │   ├── repositories/   # Acceso a datos
│   │   │   ├── services/       # Lógica de negocio
│   │   │   └── exceptions/     # Manejo de errores
│   │   └── resources/
│   │       ├── application.yml # Configuración
│   │       └── data.sql        # Datos iniciales
├── docs/
└── pom.xml             # Dependencias Maven
```

---

### 🔷 Gitflow y Commits
```markdown


🌿 Estrategia de Ramas (Gitflow)

| Rama          | Propósito                                 |
|---------------|-------------------------------------------|
| `main`        | Código en producción (estable)            |
| `develop`     | Integración de features                   |
| `feature/*`   | Desarrollo de nuevas funcionalidades      |
| `hotfix/*`    | Correcciones urgentes en producción       |
| `release/*`   | Preparación para nuevas versiones         |
```

## 💡 Convención de Commits

```bash

| Emoji | Tipo       | Descripción                           |
|-------|------------|---------------------------------------|
| ✨    | `feat`     | Nueva funcionalidad                   |
| 🐛    | `fix`      | Corrección de errores                 |
| 📚    | `docs`     | Cambios en documentación              |
| ♻️    | `refactor` | Reestructuración de código            |
| 🧪    | `test`     | Pruebas unitarias/integración         |
| 🎨    | `style`    | Formato de código                     |
| 🔧    | `chore`    | Tareas de mantenimiento               |

```

---

### 🔷 Requisitos e Instalación
```markdown

🛠️ Requisitos

- Java JDK 17+
- MySQL 8+
- Maven 3.6+
```
---

## 🔧 Instalación

1. **Clonar repositorio**:
```bash
git clone https://github.com/AuraFTG/backend.git
```
2. 🔧 **Configuración de la Base de Datos**

Configura el archivo `src/main/resources/application.yml` con:

```yaml
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/aura_db
    username: usuario
    password: contraseña
```
3. **Ejecutar aplicación**:
```bash
mvn spring-boot:run
```
---

## 📄 Licencia

Este proyecto está bajo licencia MIT. Ver [LICENSE](LICENSE) para más detalles.
