# **📚 Proyecto: Base de Datos de Recetas con MongoDB**

Este repositorio contiene la exportación de una colección de documentos de MongoDB, creada como parte de una tarea para aplicar los conceptos de modelado de datos NoSQL y consultas con filtros.

## **🎯 Objetivo del Proyecto**

1. Crear una base de datos (mi\_db\_recetas) en MongoDB.  
2. Modelar una colección (recetas) e insertar documentos coherentes (mínimo 3).  
3. Realizar consultas filtradas para extraer subconjuntos de datos específicos.  
4. Exportar la colección completa en formato JSON.  
5. Compartir el resultado en un repositorio de GitHub.

## **💾 Estructura de la Base de Datos**

El archivo principal es recetas\_export.json, que contiene la colección exportada.

**Colección:** recetas

Estructura de Documento (Ejemplo):  
Cada receta incluye campos clave para la consulta:  
{  
  "nombre": "String",  
  "tiempo\_preparacion\_minutos": "Number",  
  "ingredientes\_principales": \["Array", "de", "Strings"\],  
  "dificultad": "String", // Ej: "Baja", "Media", "Alta"  
  "es\_vegetariana": "Boolean"  
}

## **🔍 Consulta con Filtro**

Para demostrar la aplicación del filtrado, se ejecutó una consulta que busca todas las recetas cuyo tiempo de preparación es mayor a 60 minutos:

**Filtro Utilizado en MongoCompass:**

{  
  "tiempo\_preparacion\_minutos": { $gt: 60 }  
}

### **🖼️ Evidencia del Filtrado**

A continuación, se adjunta la captura de pantalla que muestra el filtro aplicado en MongoCompass y el resultado obtenido (la receta que cumple con la condición):

\!\[Captura de Pantalla del Filtro en MongoCompass\](filtro\_mongodb.png)

*Desarrollado para la clase de \[Base de Datos 2\].*