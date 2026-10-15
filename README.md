# Actividad Spring Boot: holamundo

Aplicación Spring Boot con tres endpoints REST, creada como práctica de controladores, servicios, inyección de dependencias y configuración externa.

## Tecnologías
- Java 25
- Spring Boot 4.1.1
- Maven
- Spring Web (`spring-boot-starter-webmvc`)

## Cómo ejecutarlo
1. Clonar el repositorio:
```bash
   git clone https://github.com/Jonathanluna0803/Actividad-SpringBoot.git
```
2. Abrir la carpeta en IntelliJ IDEA y esperar a que Maven descargue las dependencias.
3. Ejecutar `HolamundoApplication`.
4. Cuando la consola muestre `Tomcat started on port 8080`, la aplicación está lista.

## Endpoints

| Método | Endpoint | Respuesta |
|---|---|---|
| GET | `/api/hola` | ¡Hola Mundo desde Spring Boot! |
| GET | `/saludo` | ¡Hola desde el servicio! |
| GET | `/config` | ¡Bienvenido a Spring Boot! |

## Estructura
```
src/main/java/com/ejemplo/holamundo/
├── HolamundoApplication.java
├── controller/
│   ├── HolaMundoController.java
│   ├── SaludoController.java
│   └── ConfigController.java
└── service/MiServicio.java
src/main/resources/application.properties
```

## Diferencia entre @RestController y @Service
`@RestController` marca una clase que recibe peticiones HTTP y devuelve la respuesta directamente. `@Service` marca una clase con la lógica de negocio. Spring puede entregar el servicio al controlador sin usar `new` porque detecta `@Service` al arrancar, crea el objeto (bean) y lo inyecta por el constructor del controlador.

## Capturas

<img width="415" height="1030" alt="Captura de pantalla 2026-10-15 174201" src="https://github.com/user-attachments/assets/0ae1e26f-94ca-4507-bc5a-1da66fa6f14f" />

<img width="1730" height="207" alt="Captura de pantalla 2026-10-15 174316" src="https://github.com/user-attachments/assets/81afd1ea-d8b2-4d34-9e96-b00051a2f38e" />

<img width="1274" height="797" alt="Captura de pantalla 2026-10-15 171952" src="https://github.com/user-attachments/assets/143358c4-8dec-44f3-9ec8-06aa3c191164" />

<img width="1276" height="789" alt="Captura de pantalla 2026-10-15 172147" src="https://github.com/user-attachments/assets/c66be3a1-34aa-49b0-bf4f-e4f833ae07d1" />

<img width="1919" height="1079" alt="Captura de pantalla 2026-10-15 172345" src="https://github.com/user-attachments/assets/7611d44b-c3cc-4f27-8d7e-5736c23651b2" />






