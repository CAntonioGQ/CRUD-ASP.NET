# CRUD Básico con ASP.NET MVC, C# y SQL Server

Este proyecto es un ejemplo de una aplicación CRUD desarrollada con ASP.NET MVC, utilizando C# como lenguaje de programación y SQL Server como base de datos. El objetivo principal es mostrar cómo realizar operaciones básicas de creación, lectura, actualización y eliminación de datos.

## Requisitos Previos
- Visual Studio instalado.
- SQL Server instalado.
- Conexión a Internet para instalar paquetes NuGet y herramientas adicionales.
- Instalar Entity Framework (core y SQL)

## Configuración del Proyecto
1. Abre el Proyecto en tu Visual Studio 2022.
2. Coloca `entity.HasKey(e => e.Id).HasName("localhost");` en la linea 29 de `Mvccrudcontext.cs`.
3. Abre el proyecto en SQL SERVER o ejecuta estos Queries:

```sql
CREATE DATABASE MVCCRUD
USE MVCCRUD

CREATE TABLE Usuarios(
    id int identity(1,1) primary key,
    Nombre varchar(50),
    Fecha date,
    Clase varchar(50)
)
Si quieres ver la tabla utiliza el Query:
sql
Copy code
SELECT * FROM Usuarios
Pulsa RUN

#Contribuciones
Si encuentras problemas o tienes sugerencias para mejorar este proyecto, no dudes en abrir un problema o enviar una solicitud de extracción.

¡Esperamos que este ejemplo te sirva como punto de partida para tu propio desarrollo con ASP.NET MVC, C# y SQL Server!
