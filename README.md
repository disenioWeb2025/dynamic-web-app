# Aplicación Web Dinámica

## Descripción

Este repositorio contiene una aplicación web dinámica diseñada para mostrar prácticas y tecnologías de desarrollo web heredadas. La aplicación está construida con Java y utiliza servlets para generar contenido web interactivo.

## Características

- Páginas web interactivas usando servlets de Java
- Generación dinámica de contenido basado en la entrada del usuario
- Configuración segura mediante variables de entorno para el acceso a la base de datos
- Interfaz simple e intuitiva

## Requisitos Previos

Asegúrate de tener lo siguiente instalado en tu máquina:

- Java Development Kit (JDK) 17 o superior
- Apache Tomcat 10 o superior
- Servidor de base de datos MySQL

## Configuración de Variables de Entorno

Para mejorar la seguridad y la flexibilidad, las credenciales de la base de datos se gestionan mediante variables de entorno. Define las siguientes variables en tu sistema:

### Linux/macOS

```bash
export MYSQL_JDBC_URL="jdbc:mysql://localhost:3306/fbank"
export MYSQL_JDBC_USER="root"
export MYSQL_JDBC_PASSWORD="tupassword"
```

### Windows CMD

```cmd
set MYSQL_JDBC_URL=jdbc:mysql://localhost:3306/fbank
set MYSQL_JDBC_USER=root
set MYSQL_JDBC_PASSWORD=tupassword
```

### IntelliJ IDEA (Configuración de entorno)

```properties
MYSQL_JDBC_URL=jdbc:mysql://localhost:3306/fbank;
MYSQL_JDBC_USER=root;
MYSQL_JDBC_PASSWORD=tupassword;
```

## Instalación

Clona el repositorio:

```bash
git clone https://github.com/ferneybaron/dynamic-web-app.git
```

Abre el proyecto en tu IDE favorito (IntelliJ IDEA, Eclipse, etc.).

Configura el proyecto para usar el JDK 17+ y un servidor Tomcat compatible.

## Configuración de la Base de Datos

Antes de ejecutar la aplicación, configura la base de datos:

1. Ve al directorio `src/main/resources`.
2. Ubica el archivo `script.sql`.
3. Ejecuta el script en tu gestor de base de datos. Por ejemplo, con MySQL:

```bash
mysql -u root -p fbank < script.sql
```

## Uso

1. Compila el proyecto desde tu IDE.
2. Inicia el servidor Tomcat.
3. Accede en tu navegador a:

```
http://localhost:8080
```

4. Deberías ver el mensaje de bienvenida y un enlace al servlet principal.

## Contribuciones

Toda contribución es bienvenida. Haz un fork del repositorio, crea tu rama, realiza los cambios y abre un pull request.

## Licencia

El código fuente está bajo licencia MIT.  
Los recursos gráficos están licenciados bajo la  
[Creative Commons Atribución 3.0 Unported](https://creativecommons.org/licenses/by/3.0/).

