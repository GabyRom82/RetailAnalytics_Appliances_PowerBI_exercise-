markdown
#  Dashboard RetailAnalytics_Appliances_PowerBI_exercise-
Dashboard preview

<div align="center">

<table>
<tr>
<td style="border:6px solid #4B0082; border-radius:18px; padding:6px;">

<img src="https://github.com/user-attachments/assets/646c016b-6833-46f7-bfc4-a7c9754ff131" width="700">

</td>
</tr>
</table>

</div>


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

Uno de los principales objetivos del ejercicio, es usar paginas y documentaicón de apoyo en la parte de diseño visual, algunos recursos usados son:
 **BIPP (https://bibb.pro/apps/theme-generator/?color1=e85399&color2=060606&color3=f2dcee&color4=f89833&color5=ec75dd&color6=ef885d&color7=6c6c6c&color8=787878)**:

Te ayuda a generar diferentes temas, para la construcción del Dashboard, puedes utilizar temas ya construidos, o personalizarlo. Para el caso del ejercicio se subio la imagen del logo (ficticio), y se genero un tema personalizado en un archivo JSON (JavaScript Object Notation), para la construccion del dashboard con un diseño coherente y atractivo.

**Flaticon(https://www.flaticon.es/resultados?word=puntos)**: 
Es un recurso en línea, que tiene una gran cantidad de íconos para poder insertar en tu dasboard.

**Rueda de colores (https://color.adobe.com/es/create/color-wheel)**:
Es otra página para generar temas, en el caso de este ejercicio, se utilizo para conocer colores complementarios, y darle equilibrio al Dashboard.

- **Diseño limpio y moderno**: Uso de paleta de colores coherente, tipografías legibles y disposición equilibrada de los elementos.
- **Interactividad**: Filtros básicos, segmentadores y tarjetas  de datos (en este caso se uso el KPI ventas totales).
- **Gráficos variados**: Barras, líneas de tendencia, mapas ygráfico de dona para porcentajes,.
- **Narrativa guiada**: El dashboard cuenta una historia, desde el panorama general hasta el detalle por departamento.

---

## 🚀 Cómo Usar Este Repositorio

1.Este repositorio solo es con fines descriptivos, y demostrativo de manejo de análisis de dtos, y manejo de Power BI.

2.Para poder ver el el uso de los filtros, los segmentadores, y la tarjeta de KPI abre el archivo `.pbix` con Power BI Desktop (versión 2023 o superior).

3.Explora las diferentes páginas del dashboard y prueba los filtros interactivos.
   
4.Si deseas modificar los datos, puedes editar las fuentes en Power Query.

---

## 📷 Vista Previa del Dashboard

# Descripción general del dashboard

Este dashboard constituye una plataforma de **análisis táctico y exploratorio** para el monitoreo del desempeño comercial de una tienda ficticia de productos electrónicos. Integra visualizaciones interactivas que permiten analizar el comportamiento de ventas desde múltiples dimensiones, incluyendo volumen de productos vendidos, distribución por categoría, canal de venta y evolución temporal.

El modelo analítico facilita:

<p align="center">

<img src="https://github.com/user-attachments/assets/f1475669-9717-40f7-827f-f31b6e1447c8" width="14"> 
<b>Monitoreo de KPIs comerciales (cantidad de productos vendidos).</b>
<br><br>

<img src="https://github.com/user-attachments/assets/f1475669-9717-40f7-827f-f31b6e1447c8" width="14"> 
<b>Segmentación por categorías y subcategorías de productos.</b>
<br><br>

<img src="https://github.com/user-attachments/assets/f1475669-9717-40f7-827f-f31b6e1447c8" width="14"> 
<b>Comparación de desempeño entre canales de venta (online vs tienda física).</b>
<br><br>

<img src="https://github.com/user-attachments/assets/f1475669-9717-40f7-827f-f31b6e1447c8" width="14"> 
<b>Análisis de tendencias temporales para detectar patrones de demanda.</b>
<br><br>

<img src="https://github.com/user-attachments/assets/f1475669-9717-40f7-827f-f31b6e1447c8" width="14"> 
<b>Exploración geográfica de transacciones por ciudad.</b>

</p>

El dashboard está diseñado para apoyar decisiones tácticas de negocio, priorización de categorías y evaluación de estrategias de venta multicanal.

<p align="center">
<img width="425" height="726" alt="image" src="https://github.com/user-attachments/assets/c79cb413-8cd4-49e0-9abc-f72580675eab" />
</p>

## Análisis de la distribución Geográfica de Ventas/Transacciones (primer hoja del Dashboard)

En esta primer parte del dashboard se presenta un análisis espacial de las transacciones comerciales, permitiendo visualizar la distribución de ventas por ciudad mediante un mapa interactivo.

*Componentes analíticos:*

 - Mapa geográfico de transacciones que identifica la concentración de ventas por ubicación.
 
 - Indicador KPI de volumen total de productos vendidos.
 
 - Filtro temporal dinámico que permite analizar el comportamiento de ventas entre 2024 y 2026.

*Objetivo táctico:*  Facilitar la identificación de mercados regionales con mayor actividad comercial, permitiendo orientar decisiones relacionadas con las Estrategias de expansión, la Logística y distribución, así como tomar desiciones para Campañas comerciales regionales.


<img width="1105" height="645" alt="image" src="https://github.com/user-attachments/assets/0618e1b8-0ef4-4bc3-ad86-c1a278fcf226" />


## Desempeño por Categoría y Canal de Venta (segunda hoja del Dashboard)

En esta segunda sección del dashboard se proporciona una visión comparativa del desempeño de ventas por categorías y subcategorías de productos, así como su relación con los canales de comercialización.

*Componentes analíticos*

- Distribución porcentual de ventas por categoría

- Permite identificar qué categorías concentran mayor participación en el volumen total.

- Comparación de ventas por canal

- Diferenciación entre ventas online y ventas en tienda física.

- Análisis jerárquico de categorías y subcategorías

- Permite profundizar en el rendimiento específico de cada línea de productos.

*Objetivo táctico: Se relaciona principalmente en apoyar decisiones relacionadas con:*

- Gestión del portafolio de productos
- Priorización de categorías estratégicas
- Optimización de estrategias omnicanal



<img width="1103" height="648" alt="image" src="https://github.com/user-attachments/assets/9d3336b5-f450-4811-9880-b41893ce9f23" />


## Análisis de Tendencias y Evolución de Ventas
En la última parte del reporte del Dashboard se presenta un análisis longitudinal del comportamiento de ventas, mostrando la evolución de la demanda por categoría a lo largo del tiempo.

*Componentes analíticos:*

- Serie temporal de ventas.

- Evolución del volumen de ventas entre 2024 y 2026.

- Segmentación por categoría.

- Permite identificar patrones de crecimiento, estacionalidad o declive en cada línea de producto.


Esta parte fue diseñada para permitir a los responsables comerciales a:

 - Detectar tendencias de crecimiento o disminución en categorías específicas
 - Identificar patrones estacionales de consumo
 - Anticipar necesidades de inventario y abastecimiento

<img width="1100" height="627" alt="image" src="https://github.com/user-attachments/assets/0e18f02e-849d-4d88-8927-e2bb848fef7d" />

---

## 📚 Créditos

Este proyecto fue desarrollado como parte del curso **"Power BI – Análisis de Datos y Business Intelligence"** en Udemy. Los datos son proporcionados por el curso y tienen fines exclusivamente educativos.

Lo realiza:

<p align="center">
  <img src="https://github.com/user-attachments/assets/c21439cd-4209-4573-8575-4f068c5086fd" width="500">
</p>


<div align="center">
<p align="justify" style="max-width:800px;">
Analista de datos con 5 años de experiencia en análisis estadístico, visualización y gestión de bases de datos en los sectores educativo, de investigación y administrativo. Transformo datos en información estratégica que impulsa decisiones inteligentes. Conocimientos básicos de programación en Python y R; nivel intermedio de Excel y SQL; diseño de dashboards en Tableau y Power BI para facilitar la comprensión y el storytelling basado en datos. Con una maestría en Ciencias, aplico pensamiento analítico, crítico e innovador a cada proyecto, integrando narrativas de datos claras y efectivas. Soy una profesional motivada, adaptable y orientada al aprendizaje continuo. Como analista busco generar análisis que aporten valor, perspectiva estratégica y una visión única para mejorar el rendimiento organizacional y la optimización de decisiones estratégicas basadas en datos.
</p>
</div>


---

## 📬 Contacto

Si tienes preguntas, sugerencias o simplemente quieres conectar, ¡estaré encantado de recibir tu mensaje!

- **LinkedIn**: [https://www.linkedin.com/in/gabriela-romero-b4a11414b/)
- **Correo**: gabriela.e.romero.moreno.romero@gmail.com
