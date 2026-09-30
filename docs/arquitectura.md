## ARQUITECTURA                  

AulaLógica Web utilizará una arquitectura MVC (Modelo-Vista-Controlador), permitiendo organizar el proyecto en diferentes componentes y separar la presentación, la lógica y los datos.

                    USUARIO
                       │
                       ▼
                  NAVEGADOR WEB
                       │
                       ▼
              ┌─────────────────┐
              │      VISTA      │
              │ HTML + CSS +    │
              │   Thymeleaf     │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │   CONTROLADOR   │
              │   @Controller   │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │    SERVICIO     │
              │    @Service     │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │  MODELO / DATOS │
              │ Clases y listas │
              └─────────────────┘


COMPONENTES

VISTA
Será responsable de mostrar la información al usuario y recibir los datos mediante HTML, CSS y Thymeleaf.

CONTROLADOR
Recibirá las solicitudes del usuario, gestionará las rutas y determinará qué vista debe mostrarse.

SERVICIO
Contendrá las reglas del sistema, cálculos, validaciones y procesamiento de las actividades.

MODELO / DATOS
Representará la información utilizada por el sistema mediante clases y estructuras de datos Java.