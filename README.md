markdown
#  Dashboard RetailAnalytics_Appliances_PowerBI_exercise-
Dashboard preview
<p align="center">
  <img src="https://github.com/user-attachments/assets/646c016b-6833-46f7-bfc4-a7c9754ff131" width="70%">
</p>


## 📌 Descripción General

Este repositorio contiene mi primer dashboard interactivo desarrollado en **Power BI**, como parte de un curso práctico en Udemy: Power BI TOTAL en 14 Días - Analista de Datos Avanzado, profesor Federico.
El objetivo es aplicar conceptos de visualización de datos, modelado y diseño para crear un reporte que combine:

- **Dashboard Explicativo (o de reporte)**: Diseñado para **contar una historia con los datos** mostrando resultados claros y accesibles para una audiencia no técnica, y presentar informaicón importante para la toma de desiciones del negocio.
- **Dashboard Táctico**: Orientado en proporciona información detallada por **categoría y áreas** para facilitar el análisis a medio plazo, y la toma de decisiones operativas y desisivas para su crecimieto.
- **Dashboard analítico**: Nos permite explorar datos y encontrar patrones para esta toma de decisiones.Algunas características analíticas:
 
<p align="center">
<img src="https://cdn-icons-png.flaticon.com/512/1828/1828919.png" width="16"> <b>Filtros</b> &nbsp;&nbsp;&nbsp;
<img src="https://cdn-icons-png.flaticon.com/512/1828/1828919.png" width="16"> <b>Segmentación</b> &nbsp;&nbsp;&nbsp;
<img src="https://cdn-icons-png.flaticon.com/512/1828/1828919.png" width="16"> <b>Comparaciones</b>
</p>


Este ejercicio pone especial énfasis la **estética visual**, la claridad de los indicadores y la usabilidad, logrando un equilibrio entre funcionalidad analítica y presentación profesional.

---

## 🎯 Objetivos del Proyecto

El objetivo general de este ejercicio, es responder preguntas clave de negocio, tales como:
  - ¿Cuáles son las **ventas totales** por período (mes,trimestre y año), por categorías y por región?
  - ¿Qué **categoría** tienen mejor desempeño?
  - ¿Cómo evolucionan las ventas a lo largo del tiempo?

Así como proporcionar una vista táctica que permita diversoso filtros, que permitan responder diferentes preguntas. Parte fundamental del poder de las visualizaciones en el  StoryTelling, es narrar de forma interesante el comportamiento del negocio mediante visualizaciones atractivas y fáciles de interpretar.
En este caso se ha pedido mostrar, cómo han ido evolucionando las ventas, separando las perspectivas:

 1. Por un lado le interesa ver las ventas totales, y su tendencia a lo largo del tiempo, así como su distribución en los canales de venta (tiendas físicas u online), y conocer geográficamente, dónde se concentran sus clientes.

 2. Por otro lado, le interesa ver cómo se comparan las diferentes categorías de productos entre sí, respecto a la cantidad de unidades vendidas. 

---

## 🗂️ Datos

Los datos utilizados son **ficticios** y **no-publicos**, proporcionados en el curso de Udemy, y constan de **4 tablas relacionales** que simulan la operación de una cadena de tiendas de electrodomésticos:

- **Listado_precios**: Contiene id_producto (PRIMARY KEY), Precio y Costo.
- **Categorías**: Contiene Categoría, id_categoría,Subcategoría, id_subcategoria.
- **Ciudades**: Contiene ID_ciudad, Ciudad, Latitud y Longitud.
- **Transacciones**: Contiene Transacciones, fecha y hora, Id_producto, tipo de venta, Cantidad Id_ciudad, id_categoria, Id_subcategoría.

Se realizó un **modelo de datos en estrella** para relacionar las tablas, la relación es 1 (dimensión) a N (hechos), típica del esquema:

*La tabla Transacciones actúa como tabla de hechos (fact table): contiene medidas (como Cantidad) y claves foráneas que la conectan con las dimensiones.
*Las tablas Listado_Precios, Ciudades1 y Categorías son tablas de dimensión: cada una tiene una clave primaria (ID_Producto, ID_Ciudad, ID_Categoría/ID_Subcategoría) que es referenciada desde Transacciones.


<p align="center">
<img src="https://github.com/user-attachments/assets/889b5ee7-702c-49fe-bd2b-69964f42d759" width="80%"> 
</p>

---

## 🛠️ Herramientas y Tecnologías

- **EXCEL**: análisis exploratoriod e daots(DEA), y limpieza de la base de datos, principalmente en los datos geográficos.
- **Power BI Desktop**: Desarrollo del dashboard, modelado y visualizaciones.
- **Generador de temas BIPP**: Apoyo para el diseño del tema de Dashboard
  
---

## ✨ Características Destacadas

Uno de los principales objetivos del ejercicio, es usar paginas y documentaicón de apouo en la parte de diseño visual, algunos recursos usadosson:
 BIPP: te ayuda a generar diferentes temas, para la construcción del Dashboard, puedes utilizar temas ya construidos, o personalizarlo. Para el caso del ejercicio se subio la imagen del logo (ficticio), y se genero un tema personalizado en un archivo JSON (JavaScript Object Notation), para la construccion del dashboard con un diseño coherente y atractivo.


- **Diseño limpio y moderno**: Uso de paleta de colores coherente, tipografías legibles y disposición equilibrada de los elementos.
- **Interactividad**: Filtros básicos, segmentadores y tarjetas  de datos (en este caso se uso el KPI ventas totales).
- **Gráficos variados**: Barras, líneas de tendencia, mapas ygráfico de dona para porcentajes,.
- **Narrativa guiada**: El dashboard cuenta una historia, desde el panorama general hasta el detalle por departamento.

---

## 🚀 Cómo Usar Este Repositorio

1. Clona o descarga el repositorio.
2. Abre el archivo `.pbix` con Power BI Desktop (versión 2023 o superior).
3. Explora las diferentes páginas del dashboard y prueba los filtros interactivos.
4. Si deseas modificar los datos, puedes editar las fuentes en Power Query.

---

## 📷 Vista Previa del Dashboard

*(Incluye aquí una o varias capturas de pantalla para mostrar el resultado final)*

---

## 📚 Créditos

Este proyecto fue desarrollado como parte del curso **"Power BI – Análisis de Datos y Business Intelligence"** en Udemy. Los datos son proporcionados por el curso y tienen fines exclusivamente educativos.

---

## 📬 Contacto

Si tienes preguntas, sugerencias o simplemente quieres conectar, ¡estaré encantado de recibir tu mensaje!

- **LinkedIn**: [tu-perfil](https://linkedin.com/in/tu-usuario)
- **Correo**: tu-email@ejemplo.com
