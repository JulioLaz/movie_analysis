# Proyecto de Análisis de Películas
## Ver presentación:
https://juliolazarte.my.canva.site/movie-analysis
## Descripción General
Este proyecto tiene como objetivo analizar datos de películas y series de televisión utilizando Python, centrándose en conjuntos de datos de IMDb y TMDb. El análisis incluye preprocesamiento de datos, análisis exploratorio de datos (EDA) y visualización de varios aspectos de la industria del entretenimiento.

## Configuración

### Entorno
- Utiliza Google Colaboratory o tu editor de Python preferido
- Asegúrate de tener Python 3.x instalado

### Bibliotecas Requeridas
- pandas
- matplotlib
- seaborn
- plotly (para algunas visualizaciones)

Puedes instalar las bibliotecas requeridas usando:

```
pip install pandas matplotlib seaborn plotly
```

### Conjuntos de Datos
El proyecto utiliza los siguientes conjuntos de datos:
1. IMDb Title Basics
2. IMDb Title Ratings
3. TMDb Movie Dataset

## Estructura del Proyecto

1. **Carga y Preprocesamiento de Datos**
   - Cargar archivos TSV/CSV en dataframes
   - Limpiar y preprocesar datos
   - Manejar valores faltantes y duplicados

2. **Análisis Exploratorio de Datos (EDA)**
   - Analizar distribuciones de datos
   - Explorar relaciones entre variables

3. **Visualizaciones**
   - Crear varios gráficos para ilustrar insights:
     - Distribución de tipos de películas
     - Calificaciones promedio a lo largo del tiempo
     - Análisis de géneros
     - Análisis de ROI por género
     - Análisis de países de producción

4. **Análisis Específicos**
   - Pregunta 1: Análisis de tipos de títulos y calificaciones promedio
   - Pregunta 2: Popularidad de géneros y calificaciones promedio
   - Pregunta 3: Top 10 géneros por ROI
   - Pregunta 4: Análisis de países de producción

## Cómo Ejecutar

1. Clona este repositorio
2. Configura tu entorno Python con las bibliotecas requeridas
3. Ejecuta los notebooks de Jupyter o scripts de Python en el orden especificado en la estructura del proyecto

## Resultados

### Pregunta 1: Análisis de tipos de títulos y calificaciones promedio

![image](https://github.com/user-attachments/assets/83d8cd51-1880-404c-a96a-2eeae8b9053e)

### Insights Basados en la Relación entre el Tipo de Título (Movies vs. TV Series) y el Average Rating (1990-2024):

1. **Dominio de Movies en el Conjunto de Datos:**
   - La relación de tipos de título muestra que las películas representan el 84.3% del total, mientras que las series de televisión representan el 15.7%. Esto indica un predominio claro de las películas en el conjunto de datos.

2. **Tendencias de Ratings en Movies:**
   - Las películas han mostrado una tendencia general de incremento en las calificaciones promedio a lo largo del tiempo. Desde 1990, donde el rating promedio era de aproximadamente 5.965, ha habido un aumento gradual, alcanzando un promedio de 6.796 en 2024.
   - El aumento es relativamente lento, con algunas fluctuaciones menores, pero la tendencia general es positiva.

3. **Tendencias de Ratings en TV Series:**
   - Las series de televisión también han experimentado un aumento en los ratings promedio. En 1990, el promedio era de 7.017, y en 2024, ha aumentado a 7.101.
   - Comparado con las películas, las series de televisión tienen una calificación promedio consistentemente más alta durante todo el período analizado.

4. **Comparación de Calificaciones entre Movies y TV Series:**
   - A lo largo del período de 1990 a 2024, las series de televisión han mantenido calificaciones promedio más altas que las películas.
   - La diferencia en calificaciones indica que las series de televisión podrían estar mejor valoradas por los espectadores en comparación con las películas.

5. **Aceleración en el Aumento de Calificaciones en los Años Recientes:**
   - En los años más recientes (especialmente desde 2020), se observa una aceleración en el aumento de las calificaciones promedio para ambas películas y series de televisión. Este patrón podría estar relacionado con la mejora en la calidad de producción y la disponibilidad de contenido a través de plataformas de streaming.

### Insights Estratégicos:

1. **Enfoque en Producción de Series de Televisión:**
   - Dado que las series de televisión tienen calificaciones promedio más altas, la plataforma de streaming podría beneficiarse al invertir más en la producción y adquisición de contenido de series de televisión.
   
2. **Optimización de Algoritmos de Recomendación:**
   - La plataforma puede mejorar su algoritmo de recomendación para priorizar las series de televisión, dado que tienen calificaciones más altas y podrían atraer más a los usuarios.

3. **Segmentación de Mercados:**
   - Las diferencias en las calificaciones entre películas y series de televisión pueden ser útiles para segmentar el mercado y personalizar el contenido para diferentes grupos demográficos. Por ejemplo, promover series de televisión a usuarios que buscan contenido de alta calidad.

4. **Marketing y Promociones:**
   - Utilizar las calificaciones más altas de las series de televisión como un punto de venta en campañas de marketing para atraer nuevos suscriptores y retener a los existentes.

5. **Producción de Contenido Original:**
   - Dado el incremento en la calificación promedio tanto de películas como de series en años recientes, la plataforma puede centrarse en producir contenido original de alta calidad para continuar esta tendencia positiva y diferenciarse en un mercado competitivo.

Estas estrategias pueden ayudar a la plataforma de streaming a capitalizar los datos de tendencias del sector y mejorar su rendimiento general.

### Pregunta 2: Popularidad de géneros y calificaciones promedio
![image](https://github.com/user-attachments/assets/2b53e18b-1114-4f79-a438-c69449d470ea)

### Insights Basados en el Género de las Películas y su Calificación Promedio:

1. **Documentales como el Género Mejor Calificado:**
   - Los documentales tienen la calificación promedio más alta (7.235) entre todos los géneros, lo que sugiere que este tipo de contenido es muy valorado por los espectadores.

2. **Alta Calidad en Cortometrajes:**
   - Los cortometrajes también tienen una calificación promedio alta (7.102), aunque el número de películas en este género es significativamente menor (558). Esto indica que, aunque no son tan comunes, los cortometrajes tienden a recibir altas calificaciones.

3. **Géneros Populares con Calificaciones Moderadas:**
   - Los géneros con la mayor cantidad de películas, como Drama (144,290 películas) y Comedia (87,220 películas), tienen calificaciones promedio de 6.328 y 6.083, respectivamente. Estos géneros son populares pero no necesariamente los más valorados en términos de calidad promedio.

4. **Calificaciones Bajas para Géneros de Horror y Ciencia Ficción:**
   - El género de Horror tiene una de las calificaciones promedio más bajas (5.016), a pesar de tener un número significativo de películas (22,201).
   - La Ciencia Ficción también tiene una calificación baja (5.521) con 7,989 películas, indicando que estos géneros podrían necesitar una mejora en la calidad del contenido para aumentar su valoración.

5. **Calificaciones Relativamente Altas en Géneros Históricos y Biográficos:**
   - Los géneros de Historia (6.896) y Biografía (6.978) tienen calificaciones promedio altas, lo que sugiere un buen nivel de calidad percibida en estas categorías.

6. **Buen Desempeño de Películas de Animación y Familia:**
   - La Animación (6.689) y las películas de Familia (6.433) tienen calificaciones promedio relativamente altas, lo que indica que son bien recibidas por el público.

### Insights Estratégicos:

1. **Promoción de Documentales y Cortometrajes:**
   - Dado que estos géneros tienen las calificaciones más altas, la plataforma de streaming debería enfocarse en promocionarlos y agregar más contenido de alta calidad en estas categorías.

2. **Mejorar la Calidad en Géneros de Horror y Ciencia Ficción:**
   - Invertir en mejorar la calidad de las producciones de Horror y Ciencia Ficción para aumentar sus calificaciones promedio y atraer a más espectadores.

3. **Expandir la Oferta en Géneros Históricos y Biográficos:**
   - Dado que estos géneros tienen calificaciones altas, la plataforma debería considerar la producción y adquisición de más contenido en Historia y Biografía para satisfacer a los espectadores que buscan contenido de alta calidad en estas áreas.

4. **Fortalecer el Contenido de Animación y Familia:**
   - Mantener y expandir la biblioteca de contenido de Animación y Familia para capitalizar en sus calificaciones altas y atraer a familias y audiencias más jóvenes.

5. **Diferenciarse con Contenido Especializado:**
   - Utilizar los géneros de alto rating como Documentales y Cortometrajes para diferenciarse de la competencia y atraer a una audiencia que busca contenido más profundo y de alta calidad.

6. **Analizar y Mejorar Géneros Populares:**
   - Aunque los géneros como Drama y Comedia son populares, sus calificaciones promedio son moderadas. La plataforma debería analizar los factores que contribuyen a estas calificaciones y trabajar en mejorar la calidad general del contenido en estos géneros.

Estas estrategias pueden ayudar a la plataforma de streaming a utilizar los datos de tendencias de género de manera estratégica para mejorar su rendimiento y atraer a una audiencia más amplia y satisfecha.

### Pregunta 3: Top 10 géneros por ROI
![image](https://github.com/user-attachments/assets/0d05443c-cc42-4755-aa6c-330d16725ad6)

### Insights Basados en ROI, Ingresos, Presupuestos y Ganancias por Género:

1. **Géneros con Mayor Retorno de Inversión (ROI):**
   - **Science Fiction (Ciencia Ficción)** tiene el ROI más alto (1.631), seguido por **Fantasy (Fantasía)** (1.565) y **Adventure (Aventura)** (1.532). Esto indica que estos géneros generan un retorno significativo en relación con su inversión, haciendo que sean opciones rentables para la producción.
   - **Action (Acción)** y **Family (Familia)** también presentan ROIs altos (1.500 y 1.481 respectivamente), sugiriendo que son géneros con buenas posibilidades de obtener beneficios sustanciales.

2. **Géneros con Mayor Ingreso Total:**
   - **Action (Acción)** tiene el mayor ingreso total (50,548 millones), seguida por **Adventure (Aventura)** (41,520 millones) y **Drama** (41,843 millones). Estos géneros generan grandes cantidades de ingresos, aunque no siempre tienen el ROI más alto.
   - **Fantasy (Fantasía)** y **Science Fiction (Ciencia Ficción)** también generan ingresos significativos (23,525 millones y 27,488 millones respectivamente).

3. **Géneros con Mayores Presupuestos:**
   - **Action (Acción)** y **Adventure (Aventura)** tienen los presupuestos más altos (33,573 millones y 29,210 millones respectivamente), lo cual está alineado con sus altos ingresos. Sin embargo, también implica un mayor riesgo financiero.
   - **Science Fiction (Ciencia Ficción)** y **Fantasy (Fantasía)** también tienen presupuestos altos (18,590 millones y 15,416 millones respectivamente).

4. **Géneros con Mayor Ganancia Absoluta:**
   - **Action (Acción)** tiene la mayor ganancia absoluta (16,975 millones), seguida por **Adventure (Aventura)** (12,310 millones) y **Drama** (15,152 millones). Estos géneros no solo generan ingresos altos, sino que también dejan grandes ganancias después de cubrir sus costos.
   - **Science Fiction (Ciencia Ficción)** y **Fantasy (Fantasía)** también tienen ganancias altas (8,898 millones y 8,109 millones respectivamente).

5. **Géneros con Presupuestos y Ganancias Relativamente Pequeñas:**
   - **Western (Western)** y **War (Guerra)** tienen presupuestos más pequeños (846 millones y 2,838 millones respectivamente) y ganancias absolutas menores (120 millones y 1,483 millones), pero siguen siendo rentables con ROIs de 1.428 y 1.408 respectivamente.
   - **Mystery (Misterio)** también tiene un presupuesto más bajo (6,253 millones) y una ganancia de 3,326 millones, con un ROI de 1.270.

### Insights Estratégicos:

1. **Invertir en Géneros con Alto ROI:**
   - Dado que los géneros de **Science Fiction**, **Fantasy**, y **Adventure** tienen altos ROIs, invertir en estos géneros puede proporcionar un buen retorno sobre la inversión. La plataforma debería enfocarse en producir o adquirir más contenido en estas categorías.

2. **Capitalizar en Géneros con Ingresos Altos:**
   - Los géneros de **Action**, **Adventure**, y **Drama** generan los ingresos totales más altos. La plataforma debería mantener una oferta robusta en estos géneros para asegurar un flujo de ingresos constante y significativo.

3. **Gestionar el Riesgo en Producciones de Alto Presupuesto:**
   - Aunque **Action** y **Adventure** tienen altos ingresos y ganancias, también implican mayores riesgos debido a sus altos presupuestos. Es crucial gestionar estos riesgos cuidadosamente y evaluar las oportunidades de financiación y aseguramiento de ingresos.

4. **Diversificar con Géneros de Presupuesto Moderado:**
   - Géneros como **Mystery**, **Family**, y **Animation** presentan una oportunidad para diversificación con un riesgo financiero menor debido a sus presupuestos más moderados, pero aún ofrecen buenas ganancias y retornos.

5. **Explorar Géneros de Nicho Rentables:**
   - **Western** y **War** a pesar de sus presupuestos y ganancias menores, ofrecen un ROI razonable. La plataforma podría explorar más contenido en estos géneros de nicho que tienen seguidores leales y constantes.

6. **Optimizar Estrategias de Marketing y Distribución:**
   - Maximizar el alcance y la rentabilidad de los géneros más rentables a través de estrategias de marketing y distribución bien planificadas puede aumentar aún más los beneficios y asegurar el éxito financiero de las producciones.

Estos insights pueden ayudar a la plataforma de streaming a tomar decisiones informadas sobre dónde invertir y cómo optimizar su contenido para maximizar ingresos y rentabilidad.
### Pregunta 4: Análisis de países de producción
![image](https://github.com/user-attachments/assets/16a21620-ce08-4beb-9227-a44ed5ac5d8a)
![image](https://github.com/user-attachments/assets/e8e7a804-fe93-40a4-8db4-ef7bdf220fb8)

### Insights Basados en ROI, Cantidad de Películas y Ingresos por País de Producción:

1. **Países con Mayor Retorno de Inversión (ROI):**
   - **India** tiene el ROI más alto (1.781), seguido por **South Korea (Corea del Sur)** (1.666) y **China** (1.342). Estos países generan un retorno significativo en relación con su inversión, haciendo que sean opciones rentables para la producción.
   - **United States of America (Estados Unidos)** también presenta un ROI alto (1.428), indicando un buen equilibrio entre inversión y retorno.

2. **Países con Mayor Ingreso Total:**
   - **United States of America (Estados Unidos)** tiene, con diferencia, el mayor ingreso total (311,067 millones), seguido por **United Kingdom (Reino Unido)** (45,614 millones) y **Germany (Alemania)** (22,144 millones). Estos países generan grandes cantidades de ingresos, aunque no siempre tienen el ROI más alto.
   - **France (Francia)** y **China** también generan ingresos significativos (21,483 millones y 11,016 millones respectivamente).

3. **Cantidad de Películas Producidas por País:**
   - **United States of America (Estados Unidos)** produce la mayor cantidad de películas (6,355), seguido por **United Kingdom (Reino Unido)** (1,063) y **France (Francia)** (753). Esto sugiere una gran industria cinematográfica en estos países.
   - **India** y **Germany (Alemania)** también tienen una cantidad considerable de producciones (602 y 494 respectivamente).

4. **Países con ROI Relativamente Bajo:**
   - **Belgium (Bélgica)** tiene un ROI muy bajo (0.138), lo que indica que las producciones en este país no están generando un retorno significativo.
   - **Italy (Italia)** y **Russia (Rusia)** también tienen ROIs bajos (0.384 y 0.584 respectivamente), lo que sugiere que las inversiones en estos países no están resultando en altos retornos.

5. **Ingresos Moderados y ROIs Medios:**
   - **Japan (Japón)** y **Hong Kong** tienen ingresos moderados (9,530 millones y 7,110 millones respectivamente) y ROIs medios (1.166 y 1.312 respectivamente), sugiriendo que son mercados estables y rentables.
   - **Australia** y **Canada (Canadá)** también presentan ingresos moderados (7,182 millones y 19,231 millones respectivamente) con ROIs medios a bajos (0.925 y 0.875 respectivamente).

### Insights Estratégicos:

1. **Enfocar Inversiones en Países con Alto ROI:**
   - **India**, **South Korea (Corea del Sur)** y **China** ofrecen altos retornos de inversión, por lo que invertir en producciones en estos países puede ser muy rentable. La plataforma debería considerar ampliar su presencia y producción en estos mercados.

2. **Capitalizar en Países con Altos Ingresos:**
   - **United States of America (Estados Unidos)** y **United Kingdom (Reino Unido)** generan los ingresos totales más altos. La plataforma debería mantener una oferta robusta de contenido de estos países para asegurar un flujo de ingresos constante y significativo.

3. **Diversificación y Gestión del Riesgo:**
   - Diversificar inversiones en países como **Japan (Japón)** y **Hong Kong**, que tienen ingresos moderados y ROIs razonables, puede proporcionar estabilidad y reducir el riesgo asociado con concentrar inversiones en un solo país.
   - Evaluar estrategias para mejorar el ROI en países con retornos bajos, como **Belgium (Bélgica)** y **Italy (Italia)**, podría abrir nuevas oportunidades de crecimiento.

4. **Explorar Nuevos Mercados:**
   - **Australia** y **Canada (Canadá)** presentan oportunidades con ingresos moderados y deberían ser explorados para aumentar la variedad de contenido disponible en la plataforma.
   - Invertir en marketing y distribución en estos países puede ayudar a aumentar la visibilidad y el consumo del contenido producido.

5. **Optimización de Estrategias de Producción:**
   - Evaluar y optimizar las estrategias de producción en **Germany (Alemania)** y **France (Francia)**, que tienen altos ingresos pero ROIs relativamente bajos, podría ayudar a mejorar la eficiencia y rentabilidad de las inversiones en estos mercados.

Estos insights pueden ayudar a la plataforma de streaming a tomar decisiones informadas sobre dónde invertir y cómo optimizar su contenido para maximizar ingresos y rentabilidad, considerando tanto los retornos de inversión como los ingresos totales y la cantidad de producciones por país.

## Others Insights:
![image](https://github.com/user-attachments/assets/6b2b2490-6797-448a-ab15-9fea67dfe635)
![image](https://github.com/user-attachments/assets/f9b4ed36-3d81-4111-bda5-718b482ebe47)
![image](https://github.com/user-attachments/assets/1a2f89a7-ea2e-4dc5-9d7f-3b4e4fe03d8c)
![image](https://github.com/user-attachments/assets/428c71d2-b8ac-49b2-80cd-7da8b84e2e8f)

### Navega en el proyecto y verás mucho más!!!

## Contribuir

Siéntete libre de hacer un fork de este proyecto y enviar pull requests con mejoras o análisis adicionales.

## Licencia

[Especifica aquí la licencia elegida]
