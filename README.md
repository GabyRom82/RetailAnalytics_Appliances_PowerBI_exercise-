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

Este repositorio presenta un **dashboard interactivo desarrollado en Power BI**, creado como parte de un proyecto práctico del curso Power BI Total en 14 Días – Analista de Datos Avanzado impartido por Federico (Udemy). El objetivo del proyecto es aplicar principios fundamentales de visualización de datos, modelado y diseño de dashboards para construir un reporte analítico que facilite la comprensión del desempeño comercial de una tienda de electrodomésticos.

El dashboard integra distintos enfoques de análisis con el fin de ofrecer una visión completa del comportamiento de las ventas:

-**Dashboard explicativo(reporting dashboard):** orientado a comunicar resultados clave de forma clara y accesible, permitiendo presentar información relevante para la toma de decisiones estratégicas por parte de audiencias no técnicas.

-**Dashboard táctico:** enfocado en el análisis del desempeño comercial a nivel de categorías, subcategorías y canales de venta, proporcionando información que facilita la evaluación del rendimiento y la toma de decisiones operativas a mediano plazo.

-**Dashboard analítico:** diseñado para permitir la exploración de los datos y la identificación de patrones o tendencias, apoyando el análisis detallado del comportamiento de ventas mediante segmentaciones, comparaciones y análisis temporal.

En conjunto, este proyecto busca demostrar cómo una adecuada integración entre modelado de datos, visualización y narrativa analítica puede transformar datos transaccionales en información estratégica para la toma de decisiones basada en datos.
 
<p align="center">
<img src="https://cdn-icons-png.flaticon.com/512/1828/1828919.png" width="16"> <b>Filtros</b> &nbsp;&nbsp;&nbsp;
<img src="https://cdn-icons-png.flaticon.com/512/1828/1828919.png" width="16"> <b>Segmentación</b> &nbsp;&nbsp;&nbsp;
<img src="https://cdn-icons-png.flaticon.com/512/1828/1828919.png" width="16"> <b>Comparaciones</b>
</p>

---

## 🎯 Objetivos del Proyecto

El objetivo de este proyecto es desarrollar un dashboard analítico que permita responder **preguntas clave de negocio** relacionadas con el desempeño de ventas, facilitando la exploración de los datos y la identificación de patrones relevantes para la toma de decisiones.

En particular, el análisis busca responder a preguntas como:

- ¿Cuál es el volumen total de ventas por periodo (mes, trimestre y año), por categoría de producto y por región?

- ¿Qué categorías de productos presentan el mejor desempeño en términos de ventas o unidades comercializadas?

- ¿Cómo evolucionan las ventas a lo largo del tiempo y qué tendencias pueden identificarse?

Adicionalmente, el dashboard incorpora segmentaciones y filtros interactivos que permiten **analizar los datos desde diferentes perspectivas**, facilitando la exploración dinámica de la información.

Desde el enfoque de **data storytelling**, el proyecto busca representar visualmente el comportamiento del negocio mediante visualizaciones claras, atractivas y fáciles de interpretar, permitiendo comunicar insights relevantes a distintos tipos de usuarios. Para ello, el análisis se organiza en dos perspectivas principales:

**1. Perspectiva de desempeño general de ventas**
Se analiza el comportamiento global de las ventas, incluyendo:

- Evolución temporal de las ventas

- Distribución por canal de venta (tiendas físicas vs. online)

- Análisis geográfico para identificar las regiones o ciudades con mayor concentración de clientes

**2. Perspectiva de comparación entre categorías de productos**
Se evalúa el desempeño relativo de las diferentes categorías de productos, permitiendo comparar:

- Volumen de unidades vendidas

- Participación relativa de cada categoría

- Diferencias en el comportamiento comercial entre líneas de producto

Este enfoque permite construir una visión integral del negocio, combinando análisis temporal, segmentación comercial y exploración comparativa, elementos fundamentales en proyectos de business intelligence y analítica de datos.

---

## 🗂️ Datos

El conjunto de datos utilizado en este proyecto es **ficticio y de carácter no público**, proporcionado como material didáctico dentro del curso de Udemy. Los datos simulan la operación comercial de una cadena de tiendas de electrodomésticos, permitiendo analizar el comportamiento de las ventas desde diferentes dimensiones del negocio.

El dataset está compuesto por **cuatro tablas relacionales** que representan distintos componentes del proceso comercial:

- **Listado_Precios:** Contiene información económica de los productos, incluyendo ID_Producto (clave primaria), precio de venta y costo.

- **Categorías:** Incluye la clasificación jerárquica de los productos mediante categoría y subcategoría, junto con sus respectivos identificadores (ID_Categoría e ID_Subcategoría).
 
- **Ciudades:** Contiene información geográfica asociada a las transacciones, incluyendo ID_Ciudad, nombre de la ciudad, latitud y longitud, lo que permite realizar visualizaciones geoespaciales.

- **Transacciones:** Representa el registro de ventas e incluye información como fecha y hora de la transacción, ID_Producto, tipo de venta (canal), cantidad de unidades vendidas, ID_Ciudad, ID_Categoría e ID_Subcategoría.

## <div align="left">
  <img src="https://github.com/user-attachments/assets/ce34cd94-2edb-4945-9485-cec673571ee8" 
       width="32" height="32" alt="icono" style="vertical-align: middle;"> 
  <span style="font-size: 16px; margin-left: 8px;">Modelo de datos</span>
</div>   

 ## Modelo

Para estructurar el análisis se implementó un **modelo de datos en estrella (Star Schema)**, un enfoque ampliamente utilizado en proyectos de business intelligence y analítica de datos, que facilita el rendimiento de las consultas y la construcción de visualizaciones analíticas.

En este modelo:  

- Transacciones funciona como tabla de hechos (fact table), ya que contiene las medidas cuantitativas del negocio, como la cantidad de unidades vendidas, además de las claves foráneas que permiten relacionarla con las diferentes dimensiones.

- Listado_Precios, Ciudades y Categorías funcionan como tablas de dimensión, proporcionando el contexto descriptivo necesario para el análisis, como información de productos, ubicación geográfica y clasificación comercial.

- Las relaciones entre tablas siguen el patrón uno a muchos (1:N), donde cada dimensión se conecta con múltiples registros dentro de la tabla de hechos, permitiendo realizar análisis desde diferentes perspectivas como producto, ubicación geográfica y estructura de categorías.

Este enfoque de modelado facilita la construcción de visualizaciones dinámicas y consultas analíticas eficientes dentro del dashboard.

<p align="center">
<img src="https://github.com/user-attachments/assets/889b5ee7-702c-49fe-bd2b-69964f42d759" width="80%"> 
</p>

---

## 🛠️ Herramientas y Tecnologías

El desarrollo del proyecto involucró el uso de diversas herramientas orientadas al análisis de datos, preparación de información y visualización analítica:

**Excel**
Utilizado para realizar el análisis exploratorio de datos (EDA) y procesos iniciales de limpieza y validación del dataset, especialmente en la revisión y corrección de los datos geográficos utilizados posteriormente en las visualizaciones de mapas.

**Power BI Desktop**
Herramienta principal empleada para el modelado de datos, creación de medidas analíticas y desarrollo del dashboard interactivo, incluyendo la implementación de visualizaciones, segmentaciones y navegación analítica.

**BIPP Theme Generator**
Utilizado como apoyo para el diseño del tema visual del dashboard, permitiendo definir una paleta de colores consistente y una identidad visual coherente, con el objetivo de mejorar la legibilidad y la narrativa visual del reporte.
  
---

## ✨ Características Destacadas

Uno de los objetivos del ejercicio fue aplicar principios de diseño visual y buenas prácticas en la construcción de dashboards, apoyándose en diferentes recursos especializados para mejorar la coherencia estética, la claridad visual y la experiencia de usuario dentro del reporte.

Para ello se utilizaron diversas herramientas de apoyo en el proceso de diseño:

**BIPP Theme Generator**<sub>https://bibb.pro/apps/theme-generator/?color1=e85399&color2=060606&color3=f2dcee&color4=f89833&color5=ec75dd&color6=ef885d&color7=6c6c6c&color8=787878</sub>

Herramienta utilizada para generar temas personalizados para Power BI. Permite definir paletas de colores, estilos visuales y configuraciones de diseño mediante archivos JSON (JavaScript Object Notation). En este proyecto se utilizó para crear un tema visual personalizado, integrando un logotipo ficticio y una paleta cromática consistente, lo que permitió mantener una identidad visual uniforme en todo el dashboard.

**Flaticon** <sub>https://www.flaticon.es/</sub>

Plataforma utilizada como fuente de iconografía visual para complementar algunos elementos del dashboard. El uso de iconos facilita la interpretación visual de la información y contribuye a mejorar la claridad del diseño.

**Adobe Color** <sub>https://color.adobe.com/es/create/color-wheel<sub> 

Herramienta empleada para explorar combinaciones cromáticas y colores complementarios, permitiendo definir una paleta equilibrada que mejore la legibilidad y armonía visual del dashboard.

A partir de estos recursos se implementaron las siguientes características de diseño y funcionalidad:

- Diseño visual limpio y moderno
Uso de una paleta de colores consistente, tipografías legibles y una distribución equilibrada de los elementos visuales, con el objetivo de mejorar la claridad y la experiencia de navegación del usuario.

- Interactividad analítica
Incorporación de segmentadores, filtros y tarjetas de indicadores (KPIs) que permiten al usuario explorar los datos de forma dinámica. En particular, se implementó una tarjeta de KPI para visualizar el total de ventas, proporcionando una referencia rápida del desempeño comercial.

- Diversidad de visualizaciones
El dashboard incluye diferentes tipos de gráficos, como gráficos de barras, líneas de tendencia, mapas geográficos y gráficos de dona, lo que permite analizar la información desde múltiples perspectivas analíticas.

- Narrativa basada en datos (data storytelling)
La estructura del dashboard sigue una narrativa visual progresiva, comenzando con una visión general del desempeño de ventas y avanzando hacia análisis más detallados por categorías, canales de venta y distribución geográfica.

---

## 🚀 Cómo Usar Este Repositorio

Este repositorio tiene fines educativos y demostrativos, y fue creado para mostrar el proceso de análisis de datos, modelado y desarrollo de dashboards interactivos en Power BI.  Para explorar el proyecto se recomienda seguir los siguientes pasos:

- **Descargar** el archivo del proyecto
Descarga el archivo .pbix incluido en el repositorio.

- **Abrir** el archivo en Power BI Desktop
Para visualizar el dashboard interactivo, abre el archivo .pbix utilizando Power BI Desktop (versión 2023 o superior).

- **Explorar** las visualizaciones interactivas
Navega por las diferentes páginas del dashboard y utiliza los segmentadores, filtros y elementos interactivos para analizar los datos desde distintas perspectivas.

- **Modificar o actualizar los datos** (opcional)
Si deseas experimentar con el modelo de datos, puedes editar o actualizar las fuentes de información a través de Power Query, lo que permite transformar y preparar nuevos datos para el análisis.

---

## 📷 Vista Previa del Dashboard

# Descripción general del dashboard

Este **dashboard** constituye una plataforma de análisis táctico y exploratorio diseñada para el monitoreo del desempeño comercial de una tienda ficticia de productos electrónicos. **Integra diversas visualizaciones interactivas** que permiten analizar el comportamiento de las ventas desde múltiples dimensiones del negocio, incluyendo volumen de productos vendidos, distribución por categorías, canal de venta y evolución temporal.

El dashboard está construido sobre un **modelo analítico estructurado**, que facilita la exploración de la información y la generación de **insights*** mediante herramientas de interacción visual.

El modelo analítico permite:

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


<small>*A través de estas capacidades analíticas, el dashboard permite **transformar datos transaccionales en información estratégica** que facilita la toma de decisiones basada en datos.*<small>


<p align="center">
<img width="425" height="726" alt="image" src="https://github.com/user-attachments/assets/c79cb413-8cd4-49e0-9abc-f72580675eab" />
</p>

## Análisis de la distribución Geográfica de Ventas/Transacciones (primer hoja del Dashboard)

La primera página del dashboard presenta un **análisis geoespacial** de las transacciones comerciales, permitiendo visualizar la distribución geográfica de las ventas por ciudad mediante un mapa interactivo. Esta vista proporciona una perspectiva inicial del comportamiento comercial del negocio, facilitando la identificación de zonas con mayor concentración de actividad de ventas.

- Componentes analíticos: 

  - **Mapa geográfico de transacciones:** Visualización espacial que representa la distribución de las ventas por ciudad utilizando coordenadas geográficas (latitud y longitud), permitiendo identificar la concentración de transacciones en diferentes regiones.

  - **Indicador KPI** de volumen total de productos vendidos
Tarjeta de indicador que muestra el total de unidades comercializadas, proporcionando una referencia rápida del desempeño general del periodo analizado.

  - **Filtro temporal dinámico**
    
  - **Segmentador** de fechas que permite analizar el comportamiento de las ventas en el periodo comprendido entre 2024 y 2026, facilitando la exploración temporal del dataset.


- Objetivo analítico: El propósito de esta página es proporcionar una visión geográfica del desempeño comercial, permitiendo identificar las regiones con mayor actividad de ventas y analizar la distribución territorial de los clientes. Este enfoque facilita la generación de información relevante para apoyar decisiones relacionadas con:

   - Estrategias de expansión comercial

   - Optimización logística y de distribución

   - Planificación de campañas comerciales regionales

En conjunto, esta visualización permite comprender dónde se concentra la actividad comercial, aportando un contexto espacial clave para el análisis del negocio.

<img width="1105" height="645" alt="image" src="https://github.com/user-attachments/assets/0618e1b8-0ef4-4bc3-ad86-c1a278fcf226" />


## Desempeño por Categoría y Canal de Venta (segunda hoja del Dashboard)

La segunda página del dashboard presenta un **análisis comparativo** del desempeño comercial por categorías y subcategorías de productos, integrando además la dimensión del canal de venta. Esta vista permite evaluar cómo se distribuyen las ventas entre diferentes líneas de productos y cómo estas se comportan dentro de los distintos canales de comercialización.

A través de visualizaciones jerárquicas y comparativas, esta sección facilita la **identificación de categorías con mayor contribución** al volumen total de ventas, así como la comprensión del papel que desempeñan los canales online y tienda física en la dinámica comercial del negocio.

- Componentes analíticos:  Esta página del dashboard incorpora los siguientes elementos de análisis:

    - Distribución porcentual de ventas por categoría
     
    - Visualización que muestra la participación relativa de cada categoría de producto en el total de ventas, permitiendo identificar cuáles concentran una mayor proporción del volumen comercializado.
     
    - Comparación de ventas por canal de comercialización:  Gráfico comparativo que permite diferenciar el desempeño entre ventas online y ventas en tienda física, facilitando el análisis del comportamiento de los clientes según el canal utilizado.
     
    - Análisis jerárquico de categorías y subcategorías: Visualización estructurada que permite profundizar en el desempeño de las distintas subcategorías de productos, proporcionando una perspectiva más detallada sobre el rendimiento de cada línea dentro del portafolio.

- Objetivo analítico: El propósito de esta sección es proporcionar una visión comparativa del desempeño comercial por tipo de producto y canal de venta, facilitando la identificación de oportunidades de optimización en la estrategia comercial.

- Este análisis contribuye a respaldar decisiones relacionadas con:

   - Gestión estratégica del portafolio de productos

   - Priorización de categorías con mayor potencial comercial

   - Optimización de estrategias de venta omnicanal

En conjunto, esta página permite comprender qué productos impulsan el desempeño comercial y a través de qué canales se generan las ventas, aportando información clave para la planificación estratégica del negocio.


<img width="1103" height="648" alt="image" src="https://github.com/user-attachments/assets/9d3336b5-f450-4811-9880-b41893ce9f23" />


## Análisis de Tendencias y Evolución de Ventas

La tercera página del dashboard presenta un análisis temporal del comportamiento de las ventas, permitiendo observar la evolución del volumen de productos vendidos a lo largo del tiempo. Esta vista está orientada a identificar patrones de comportamiento en la demanda y analizar el desempeño de las diferentes categorías de productos en distintos periodos.

Mediante visualizaciones de tipo serie temporal, el dashboard permite comprender cómo evolucionan las ventas entre 2024 y 2026, facilitando la identificación de tendencias de crecimiento, variaciones estacionales o posibles disminuciones en la demanda.

- Componentes analíticos, esta sección integra los siguientes elementos de análisis:

   - **Serie temporal de ventas**: Visualización de línea que representa la evolución del volumen de ventas a lo largo del tiempo, permitiendo analizar cambios en el comportamiento de la demanda.

   - **Evolución del volumen de ventas (2024–2026)**: Análisis temporal que muestra la dinámica del volumen de productos vendidos durante el periodo disponible en el dataset.

   - **Segmentación por categoría de producto**: Desagregación de la serie temporal por categorías, lo que permite comparar el desempeño de las distintas líneas de productos y detectar variaciones específicas en cada una.

- Objetivo analítico: El propósito de esta página es proporcionar una perspectiva longitudinal del desempeño comercial, facilitando el análisis de la evolución de las ventas en el tiempo y la identificación de patrones relevantes para la planificación estratégica. Este análisis permite a los responsables comerciales:

   - Detectar tendencias de crecimiento o disminución en categorías específicas

   - Identificar posibles patrones estacionales de consumo

   - Anticipar necesidades de inventario y abastecimiento

En conjunto, esta sección permite comprender cómo evoluciona la demanda a lo largo del tiempo, aportando información valiosa para la planificación operativa y la toma de decisiones comerciales basadas en datos. Anticipar necesidades de inventario y abastecimiento

<img width="1100" height="627" alt="image" src="https://github.com/user-attachments/assets/0e18f02e-849d-4d88-8927-e2bb848fef7d" />

---
## <div align="left">
  <img src="https://github.com/user-attachments/assets/e50e0ae2-1f8b-4b32-8316-f2ebefaa2dce" 
       width="32" height="32" alt="icono" style="vertical-align: middle;"> 
  <span style="font-size: 16px; margin-left: 8px;">Insights obtenidos del análisis</span>
</div>  

## Insights obtenidos del análisis

A partir de la exploración del dashboard y del análisis de las diferentes dimensiones del dataset (categoría de producto, canal de venta, geografía y evolución temporal), se identifican algunos hallazgos relevantes sobre el comportamiento comercial del negocio:

- **Concentración geográfica de la demanda**
El análisis geoespacial revela una marcada concentración de transacciones en la región de Tokio, seguida por Yokohama y Nagoya. Estas tres ciudades acumulan la mayor parte del volumen de ventas, lo que indica la existencia de mercados regionales con alta actividad comercial.

  - *Implicaciones estratégicas:*

    - Expansión y capacidad logística: Priorizar inversiones en infraestructura de almacenamiento y distribución en estas zonas para garantizar disponibilidad de producto y reducir tiempos de entrega.

    - Estrategias comerciales focalizadas: Diseñar campañas de marketing y promociones específicas para estos mercados, aprovechando su alta densidad de clientes.

Optimización de recursos: Evaluar la posibilidad de reducir la presencia física en regiones de baja demanda y redirigir esfuerzos hacia los clústeres de mayor potencial.

 - **Desempeño diferenciado entre categorías de productos**

   - *Implicaciones estratégicas:*

     - Priorización del portafolio: Asignar mayor presupuesto de inventario y marketing a la categoría TV y Sonido, asegurando surtido y novedades constantes.

     - Estrategias de cross-selling: Aprovechar la alta rotación de esta categoría para promocionar productos complementarios (accesorios, cables, garantías extendidas).

     - Negociación con proveedores: Reforzar alianzas estratégicas con los principales fabricantes de TV y audio para obtener mejores condiciones y exclusividades.

- **Importancia relativa de los canales de venta**
El canal online supera significativamente a la tienda física en volumen de ventas durante todo el período analizado. Esta tendencia sugiere un cambio en las preferencias de compra de los consumidores hacia lo digital.

  - *Implicaciones estratégicas:*

    - Reasignación de recursos: Evaluar la posibilidad de reducir la superficie de venta física o transformar algunas tiendas en puntos de experiencia o showrooms, disminuyendo costos fijos (alquiler, servicios, personal).

    - Fortalecimiento del canal digital: Invertir en mejoras de la plataforma de e-commerce, logística de última milla y atención al cliente online.

    - Estrategia omnicanal: Desarrollar iniciativas que integren ambos canales, como la compra online con recogida en tienda (click & collect), para aprovechar sinergias y ofrecer una experiencia unificada.
     
- **Evolución temporal y patrones de demanda**

El análisis de series temporales muestra un comportamiento diferenciado por categoría:

  - Electrodomésticos y computadoras: Demanda estable y constante a lo largo del año, sin picos estacionales marcados. Esto indica una necesidad de reposición continua y productos de uso cotidiano.

  - Cámaras fotográficas: Experimentaron un crecimiento significativo durante el primer año, seguido de una caída sostenida en los dos años posteriores. Esta tendencia podría deberse a la saturación del mercado, cambios tecnológicos o la entrada de nuevos competidores.

    - *Implicaciones estratégicas:*

      - Planificación de inventario: Para categorías estables, mantener niveles de stock predecibles y optimizar la cadena de suministro con reposiciones programadas.

      - Investigación de mercado: Realizar un análisis más profundo sobre la caída en ventas de cámaras para identificar causas (¿cambio en preferencias del consumidor? ¿obsolescencia por smartphones?) y definir acciones correctivas (liquidación de inventario, reposicionamiento, descuentos).

      - Previsión de demanda: Incorporar estos patrones en modelos predictivos para ajustar compras y promociones de forma dinámica.



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
