

# AulaLógica Web

Aplicativo web didáctico de **Fundamentos de Programación en Java**.

> Betancourt Steven
> Oogonaga Isaac
> Terán Julio 

![Estado](https://img.shields.io/badge/estado-Hito%201%3A%20dise%C3%B1o-yellow)
![Java](https://img.shields.io/badge/Java-21%20LTS-orange)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-Thymeleaf-green)
![Maven](https://img.shields.io/badge/build-Maven-blue)

## 1. Introducción

**AulaLógica Web** es un aplicativo web educativo desarrollado en Java que enseña los fundamentos de programación mediante explicaciones breves, ejemplos resueltos y prácticas con retroalimentación inmediata.

**Reto:** ¿cómo enseñar a otro estudiante los fundamentos de programación mediante una aplicación web sencilla, clara e interactiva desarrollada en Java?

**Problema:** quien inicia en programación suele saltar al código sin analizar el problema, lo que genera errores de lógica que no sabe explicar.

**Usuario objetivo:** estudiante de primer semestre sin experiencia previa.

**Objetivo general:** diseñar, construir, probar y presentar colaborativamente un aplicativo web didáctico en Java que integre los conocimientos del periodo y documente las etapas básicas del ciclo de vida del software.

## 2. Alcance (producto mínimo)

- 6 módulos: Algoritmos/EPS · Pseudocódigo/diagramas · Java básico · Condicionales · Ciclos · Validación y pruebas.
- 3 prácticas interactivas procesadas en Java (selección, ciclos, validación/cálculo).
- Evaluación de 10 preguntas o más, con puntaje y retroalimentación.
- Glosario de 15 conceptos o más.
- Sección del equipo con roles y créditos.
- Ejecución local en `http://localhost:8080`, sin base de datos (datos en memoria).

## 3. Integrantes y roles

| Integrante | Rol |
|---|---|
| _Betancourt Steven _ | Coordinación e integración |
| _Betancourt Steven _ | Análisis y contenido |
| _Teran Julio_ | Desarrollo Java/web |
| _Ogonaga Isaac_ | Pruebas y documentación |

> Los roles rotan cada dos semanas.

## 4. Tecnologías

| Elemento | Decisión |
|---|---|
| Lenguaje | Java (OpenJDK 21 LTS) |
| Framework | Spring Boot (Spring Web, Thymeleaf, Validation) |
| Construcción | Maven |
| Interfaz | HTML5 y CSS3 |
| Editor | Visual Studio Code (Extension Pack for Java + Spring Boot) |
| Versionado | Git y GitHub |

## 5. Arquitectura resumida

MVC por capas: **Vista (Thymeleaf) → Controlador → Servicio → Modelo/datos**.
Detalle completo en [`docs/02-arquitectura.md`](docs/02-arquitectura.md).

## 6. Estructura del proyecto

```
aulalogica-web/
├── src/main/java/ec/edu/uta/aulalogica/
│   ├── controller/     # rutas web y formularios
│   ├── service/        # reglas, cálculos, validación, puntajes
│   └── model/          # Tema, Ejercicio, Pregunta, Resultado
├── src/main/resources/
│   ├── templates/      # páginas Thymeleaf
│   └── static/
│       ├── css/        # estilos
│       └── img/        # imágenes con créditos
├── docs/               # requisitos, arquitectura, bosquejos, pruebas, evidencias
├── pom.xml
└── README.md
```

## 7. Cómo ejecutar (a completar desde la semana 9)

```bash
# Requisitos: JDK 21 y Maven (o el wrapper incluido)
git clone https://github.com/<usuario>/aulalogica-web.git
cd aulalogica-web
./mvnw spring-boot:run
```

Abrir en el navegador: <http://localhost:8080>

## 8. Documentación

| Documento | Contenido |
|---|---|
| [Problema y requisitos](docs/01-problema-y-requisitos.md) | Ficha del problema, requisitos y priorización |
| [Arquitectura](docs/02-arquitectura.md) | Capas, flujo de datos, rutas y estructura |
| [Bosquejos](docs/03-bosquejos.md) | Mapa de navegación y 5 pantallas |
| [Plan de trabajo](docs/04-plan-y-contribuciones.md) | Hitos y tabla de contribuciones |

## 9. Hitos

| Fecha 2026 | Resultado esperado | Estado |
|---|---|---|
| 11 SEP | Equipo, problema y repositorio | ✅ |
| 18 SEP | Requisitos, contenidos y prácticas | ✅ |
| 25 SEP | Arquitectura y bosquejos | ✅ |
| **30 SEP** | **Presentación del diseño (Hito 1)** | 🔄 |
| 9 OCT | Proyecto Java ejecutándose localmente | ⬜ |
| 30 OCT | Primer producto mínimo interactivo | ⬜ |
| 13 NOV | Módulos, práctica 3, evaluación y glosario | ⬜ |
| 27 NOV | Candidato final probado | ⬜ |
| 2 DIC | Entrega total y presentación final | ⬜ |

## 10. Pruebas, limitaciones y mejoras futuras

_Se completará durante las semanas 12–16._
