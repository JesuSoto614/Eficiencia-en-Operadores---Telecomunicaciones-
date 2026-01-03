# 📊 EFICIENCIA EN OPERADORES - Telecomunicaciones 

## 📌 Resumen
Implemente metricas para la categorizar la eficiencia en operadores, en distintas actividades, luego desarrolle una formula para etiquetar el desempeño de los trabajadores de forma general logrando evaluar el desempeño del 93.5% de los operadores, empleando pandas, matplot, numpy, seaborn y scipy.

## 🎯 Objeto de Estudio   
EL proposito de este proyecto es estableer metricas para la distincion de operadores segun su eficiencia. Para ello es neesario consultar KPIs (Indicadores Clave de Desempeño por sus siglas en ingles) empleadas en las empresas del rubro, las cuales despues de una investigacion externa encontramos las siguientes:

- Tiempo Promedio de Operación (Average Handle Time - AHT) Es el tiempo total invertido en una interacción, desde que se contesta hasta que se cierran las notas administrativas. Es el indicador primario de la agilidad del operador.

- Referencia: "El AHT es fundamental para dimensionar la fuerza laboral y asegurar que los costos operativos se mantengan dentro de los márgenes previstos" (Gartner, 2022).
    Tiempo Medio de Respuesta (Average Speed of Answer - ASA) NUEVA MÉTRICA: Mide cuánto tiempo espera un cliente en la cola antes de ser atendido por un operador. Refleja si el equipo de operadores es suficiente para el volumen de llamadas.

- Referencia: El Customer Service Institute of America (2024) establece que el ASA es el principal predictor del abandono de llamadas; a mayor tiempo de espera, mayor es la tasa de deserción.
    Resolución en la Primera Llamada (First Call Resolution - FCR) Mide la eficiencia cualitativa. Si un operador es rápido pero no resuelve, el costo operativo se duplica cuando el cliente vuelve a llamar.

- Referencia: Según Dixon et al. (2010) en Harvard Business Review, reducir el esfuerzo del cliente mediante la resolución inmediata es el factor que más impacta en la lealtad en servicios de telecomunicaciones.
    Llamadas Realizadas por Hora (Outbound Calls per Hour) Mide la productividad proactiva de un operador. En proyectos de retención o cobranza de telecomunicaciones, determina el ritmo de trabajo del agente en campañas de salida.

    Cita: "La eficiencia en campañas outbound no solo se mide por el volumen, sino por la relación entre llamadas realizadas y contactos efectivos alcanzados" (IFC, 2023).
    Llamadas No Atendidas por el Agente (Agent No Answer - ANA) Mide la cantidad de veces que una llamada suena en la extensión de un operador y, tras un tiempo determinado (ej. 15 segundos), el sistema la retira porque el operador no contestó.

    Cita: "El RONA es una métrica de fuga de eficiencia pura; cada llamada no contestada por un agente disponible incrementa el tiempo de espera del cliente en al menos un 30% adicional al reingresar a la cola" (Gartner, 2022).
    Cada uno de estos indicadores seran la base para el calculo de la eficiencia, pero puede ser modificados a la nesecidad y la informacion disponible del proyecto. Las formulas se presentaran en cada uno de los pasos.

## 📂 Dataset
Datos simulados / proporcionados con fines academicos que representan metricas operativas del sector telecomunicaciones.      

## 🧠 Metodologia 
- Limpieza de datos:
    1. Imprimiremos una muestra de los datos
    2. Buscaremos errores en el formato de la informacion
    3. Cambiaremos el formato y limpiaremos los datos
- Exploracion de datos:
    1. Analizaremos los datos contenidos en cada columna para determinar si existen outlier o valores atipicos, asdi como prevenir cualquier inconveniente
Medicion de KPIs:
Para cada indicador desglosaremos en un cuadro de texto la formula y las columnas a utilizar
Tendremos un apartado de exploracion donde:
    1. Observaremos los promedios, percentiles y otras metricas.
    2. Designaremos las metricas de un operador eficiente y uno que no
    3. Comprobaremos las diferiencias
    4. Etiquetaremos o filtraremos los operadores segun los parametros establesidos
    5. Observaremos resultados, daremos concluciones y recomendaciones.

## 📈 Resultados
/image.png
Despues de limpiar y dar formato a los datos, pudimos calcular los indicadores de eficiencia de los cuales determinamos que la mayor area de oportunidad que tiene la empresa en el indicador Llamadas por Hora - OCH, ya que representa el kpi con el porcentaje de datos aceptables mas bajos con un 26 % de operadores con metricas Normales y 21% Con metricas eficientes. Al contrario que Tiempo Promedio de Operacion con un 79% de eficiencia y un 20% de operadores normales. Encuanto al resto de indicadores Llamadas no Respondidas -ANA ocupa el segundo lugar en el top de indicadores con mas eficiencia, con un porcentaje de 72% de operadores eficientes y 13% de operadores normales sumando un 86 % de operadores con una Taza de llamadas perdida aceptable, seguido por Tiempo Promedio de respuesta - ASA con colaboradores que responden eficientemente un 49% y normalmente 19%, y por ultimo Resolucion a la primera llamada FCR con 62% de operadores aceptables de los cuales solo el 36% actuan de manera Eficiente.

**Ponderacion general**
Una ves ponderados los operadores con Indicadores individuales, se promediaron las puntuaciones y se re-etiqueto llegando al siguente resultado:

- Operadores Eficientes: 24.77%
- Operadores Normales: 48.44%
- Operadores Deficientes: 16.15%
- Operadores Muy Deficientes: 4.13%
- Datos insufucientes: 6.33%
- Sin datos: 0.18%.

## ✅ Conclusiones

Con los datos obtenidos del etiquetado general podemos concluir que:

La empresa cuenta con un 73.21% de trabajadores con desempeño aceptable de los cuales el 24.77% son Eficases.
- Solo un 4.13% cuenta con metricas que requieren de mucho trabajo
- Hay margen de error del 6.51 % que no permitio evaluar a los trabajadores correctamente
**Recomendaciones**
- Prestar atencion a los outliers de la duracion de llamada y contador de llamdas, ya que puede haber un error en la captura o una manipulacion
- Atender principales areas de oportunidad como lo son el numero de llamadas realizadas por los operadores ya que es el kpi con peores resultados (hay pocas llamadas realizadas y el tiempo promedio de llamada es aceptable por lo que el tiempo en llamada no es una limitante).
- Implementar otras metricas de evaluacion como 'Calificacion del Usuario'.
- Detallar si los operadores se encuentran en areas diferentes o desempeñen funcinciones distintas (Esto permitiria evaluar por area, lo que seria una evaluacion mas eficiente).

## 🛠️ Herramientas Utilizadas 
- Python 3.12
- Pandas
- SciPy
- Matplotlib
- Seaborn 

## ▶️ Cómo Ejecutar el Proyecto**
1. Clonar el repositorio.
2. Crear el entorno virtual
    - Instalar el archivo requirements.txt 
    - Activar el entorno virtual 
3. Ejecutar el Notebook.