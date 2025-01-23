# SerenityAIModelScraping
 This script uses web scraping and database management techniques to interact with the Serenity Star API, process data, and store it in a SQL database. Its main purpose is to automate the flow of data from an API to a structured storage, facilitating its subsequent analysis.

# Documentación técnica del guión
Propósito del guión

Este script utiliza técnicas de web scraping y gestión de bases de datos para interactuar con la API de Serenity Star, procesar datos y almacenarlos en una base de datos SQL. Su objetivo principal es automatizar el flujo de datos desde una API a un almacén estructurado, facilitando su posterior análisis.

# Estructura del guión

El script utiliza las siguientes bibliotecas:

solicitudes: Para realizar solicitudes HTTP.
pandas: Para manipulación de datos.
sqlalchemy y sqlite3: para la gestión de bases de datos
registro: Sistema de registro para almacenar registros en un archivo y mostrarlos en la consola.
json: trabajar con datos en formato JSON
Funciones principales:

scrape_and_send_to_serenity: envía datos a la API de Serenity Star y procesa la respuesta.
create_database y create_table: configura una base de datos SQLite para almacenar datos procesados.
insert_or_update_data: Inserta o actualiza datos en la base de datos SQLite según el modelo.
main: Función principal que organiza el flujo del programa, solicitando al usuario datos de entrada y ejecutando las funciones anteriores.
Envía una solicitud a la API con los parámetros necesarios.
Recibir y verificar la respuesta, asegurándose de que no esté vacía y que contenga datos válidos.
Procesa y limpia los datos JSON obtenidos de la respuesta.
Almacene datos en una base de datos SQLite, ya sea insertando nuevos registros o actualizando los existentes.
Registra cada paso del proceso para facilitar la depuración y la supervisión. (Explotación florestal)

# Manual de usuario
Requisitos:
Python 3.x
Paquetes:
json
hermosasoup4
sqlite3
Accede a la API de Serenity Star, con la URL, claves de acceso y datos necesarios.
Instrucciones de ejecución
Instalación de dependencias: ejecute los siguientes comandos para instalar las dependencias necesarias:

!pip solicita la instalación de beautifulsoup4 panda

# Ejecución

1. Configurar el entorno: asegúrese de instalar las bibliotecas necesarias
2. Ejecutar el script
3. Ingresa el modelo que deseas analizar
4. Ingresa las URL que deseas extraer, separadas por comas
5. Serenity limpiará la información y extraerá las variables necesarias.
6. Se guardará automáticamente en la base de datos "serenity_data.db"
7. El registro de inicio de sesión se registra en scrape_and_store.log
