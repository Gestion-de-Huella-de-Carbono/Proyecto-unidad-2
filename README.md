# EcoFootprint-BackEnd

## Descripción

EcoFootprint es una aplicación web que permite a los usuarios registrar datos sobre su huella de carbono personal, incluyendo transporte, consumo de energía, hábitos alimenticios, etc. Basado en esta información, la aplicación ofrece sugerencias para reducir el impacto ambiental de los usuarios.

## Diagrama de Clases

Puedes encontrar el diagrama de clases en el siguiente enlace: [Diagrama de Clases](https://drive.google.com/file/d/18HfHExuM7N_Qcn1890f2Ui1pYyvJTv0r/view?usp=sharing)

## Diagrama de Despliegue

Puedes encontrar el diagrama de despliegue en el siguiente enlace [Diagrama de Despliegue]()

## Despliegue del Backend

### Instalación

1. Clonar el repositorio:
    ```sh
    git clone https://github.com/Gestion-de-Huella-de-Carbono/EcoFootprint-BackEnd.git
    ```

2. Navegar al directorio del proyecto:
    ```sh
    cd EcoFootprint-BackEnd
    ```

3. Configurar la base de datos en `src/main/resources/application.properties`:
    ```properties
   spring.datasource.url=jdbc:h2:mem:Db-EcoFootprint
   spring.datasource.driverClassName=org.h2.Driver
   spring.datasource.username=sa
   spring.datasource.password=
   spring.h2.console.enabled=true
   spring.h2.console.path=/h2-console
   spring.h2.console.settings.web-allow-others=true
   spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
   spring.jpa.hibernate.ddl-auto=update
   spring.jpa.show-sql=true
    ```

4. Instalar las dependencias y compilar el proyecto:
    ```sh
    mvn clean install
    ```

### Ejecución

Para ejecutar la aplicación en un entorno local:

```sh
mvn spring-boot:run
```
## Despliegue del Frontend
### Instalación

Clonar el repositorio del frontend:

      git clone https://github.com/Gestion-de-Huella-de-Carbono/EcoFootprint-FrontEnd.git


### Uso

Para utilizar el frontend, abre el archivo `index.html` en tu navegador web:

1. Desde la raíz del repositorio clonado del frontend, abre el archivo `index.html`.

2. Puedes navegar por las distintas funcionalidades utilizando los enlaces proporcionados en la página.

   Por ejemplo, para listar personas, ve a _Listar_.

   Para registrar una nueva persona, ve a _Registrar Nueva Persona_.

   Y así sucesivamente para las otras funcionalidades.

3. Asegúrate de que el backend esté en ejecución en [http://localhost:8080](http://localhost:8080/api/eco-footprint/persons) mientras utilizas el frontend.



## Tareas y Responsabilidades

| Miembro del Equipo         | Funciones                                           |
|----------------------------|-------------------------------------------------|
| Juan Miguel Cadena         | **Mejoras en el Modelo de Excepciones y Modificaciones en los Modelos de Datos**<br>- Revisar y mejorar la estructura de las excepciones utilizadas en el proyecto.<br>- Asegurar que las excepciones sean adecuadamente lanzadas y manejadas según las buenas prácticas aprendidas.<br>- Revisar los modelos de datos actuales y añadir setters y getters según las necesidades del proyecto, asegurando coherencia y cumplimiento de los estándares definidos. |
| Juan Manuel Velásquez      | **Implementación de Persistencia en Repositorios**<br>- Implementar la persistencia utilizando lo aprendido en la clase de persistencia.<br>- Utilizar Spring Data JPA en las interfaces ya creadas para gestionar las operaciones de persistencia de datos. |
| Juan Esteban Obando        | **Definición de Métodos de Servicio**<br>- Definir los métodos a utilizar en las interfaces de servicio.<br>- Implementar dichos métodos asegurando que realicen las operaciones correspondientes utilizando los repositorios y modelos adecuados.<br>- Incluir lógica de negocio y manejo de excepciones apropiado. |
| Daniela Ramirez            | **Definición de Métodos de Servicio**<br>- Colaborar en la definición de métodos en las interfaces de servicio.<br>- Implementar los métodos definidos, asegurando su correcta funcionalidad y manejo adecuado de excepciones y lógica de negocio. |
| Carlos Andrés Zuluaga      | **Pruebas de Implementación del Servicio**<br>- Generar pruebas para los métodos del servicio implementado utilizando JUnit y Mockito, garantizando la calidad y funcionalidad del código. |
| Yeferson Salcedo           | **Implementación de Métodos de API en el Controlador**<br>- Generar los métodos necesarios para el consumo del API.<br>- Asegurar que los métodos respondan adecuadamente a las solicitudes HTTP, siguiendo las mejores prácticas y estándares definidos. |

## Licenciamiento

Este proyecto está licenciado bajo la Apache License 2.0. Para más detalles, consulta el archivo [LICENSE](LICENSE).

