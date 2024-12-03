# Dashboard y Análisis en Google Sheets

## Objetivo del proyecto

Realizar un análisis exploratorio de un conjunto de datos de elección propia y elaborar un dashboard en Google Sheets.

## Requisitos 

- Transformación y limpieza de los datos.
- Análisis descriptivo de los datos.
- Dashboard.
- Informe explicativo del análisis.

## Requisitos del Github

Tu repositorio tiene que constar, al menos, de los siguientes archivos/carpetas:

- Archivo README.md, que recoja los pasos seguidos durante el proyecto y el informe de tú análisis.
- Si usas Google Sheets, la url de acceso a esa hoja de cálculo compartida para cualquier persona con el enlace en modo lectura.
- Un archivo que contenga los datos originales con los que se va a trabajar: un csv, un excel o una url a un Google Sheets. Y el origen de los mismos si fuera necesario ( la url a través de la cual has llegado a los datos ).


## Origen de los datos

Hemos obtenido los datos des de https://www.kaggle.com/, en particular hemos elegido los datos sobre Remote Work & Mental Health (https://www.kaggle.com/datasets/waqi786/remote-work-and-mental-health)

## Objetivo del conjunto de datos

Estos datos tratan de analizar el bienestar mental en la era del trabajo a distancia, es decir, como afecta el teletrabajo a los niveles de estrés, el equilibrio entre la vida laboral y personal (work-life balance) y las condiciones de salud mental (ansiedad, depresión, etc.) en diferentes industrias y regiones. 

### Columnas/Campos del conjunto de datos y tamaño

Nuestro conjunto de datos inicial está formado por 5000 filas y 20 columnas

A continuación vamos a describir que representan cada una de estas columnas:

- **Employee_ID**: Identificador único de cada empleado.
- **Age**: Edad del empleado.
- **Gender**: Género del empleado (puede ser masculino, femenenino, no binario, prefiere no decirlo).
- **Job_Role**: Rol actual del empleado.
- **Industry**: Industria en la que trabajan.
- **Years_of_Experience**: Años de experiencia del empleado en este rol. 
- **Work_Location**: Modalidad de trabajo (remoto, híbrido, presencial).
- **Hours_Worked_Per_Week**: Horas semanales trabajadas.
- **Number_of_Virtual_Meetings**: Número de reuniones online.
- **Work_Life_Balance_Rating**: Puntuación autoevaluada del equilibrio entre la vida personal y laboral (1 al 5).
- **Stress_Level**: Nivel de estrés autoevaluado por el empleado (bajo, medio, alto).
- **Mental_Health_Condition**: Condición de salud mental reportada (ansiedad, depresión, burnout, ninguna).
- **Access_to_Mental_Health_Resources**: Indica si el empleado tiene o no acceso a recursos de salud mental.
- **Productivity_Change**: Cambios en la productividad laboral (incrementa, disminuye, no cambia). 
- **Social_Isolation_Rating**: Puntuación autoevaluada (1 al 5) sobre qué tan aislado se siente el empleado.
- **Satisfaction_with_Remote_Work**: Nivel de satisfacción con las condiciones de trabajo remoto 
    (satisfecho, neutral,insatisfecho).
- **Company_Support_for_Remote_Work**: Puntuación autoevaluada (1 al 5) sobre la ayuda que recibe el empleado de su empresa para el facilitar el teletrabajo.
- **Physical_Activity**: Frecuenacia con que el empleado practica actividad física (semanal, diaria, ninguna).
- **Sleep_Quality**: Calidad del sueño (mala, buena, promedio)
- **Region**: Región a la que pertenece (Europa, África, Asia, Norteamérica, Sudamérica, Oceanía)

Clasificamos las diferentes columnas en alfanuméricas, numéricas, categóricas, categóricas ordinales y booleanas:

- **Alfanuméricas**: Employee_ID. (1)
- **Numéricas**: Age, Years_of_Experience, Hours_Worked_Per_Week, Number_of_Virtual_Meetings. (4)
- **Categóricas**: Gender, Job_Role, Industry, Work_Location, Stress_Level, Mental_Health_Condition, 
                   Productivity_Change, Satisfaction_With_Remote_Work, Physical_Activity, Sleep_Quality,
                   Region.(11)
- **Categóricas ordinales**: Work_Life_Balance_Rating, Social_Isolation_Rating, Company_Support_for_Remote_Work. (3)
- **Booleanas**: Access_to_Mental_Health_Resources.(1)

Hemos incluido como columnas categóricas ordinales aquellas que representan una autoevaluación realizada por el empleado donde la respuesta puede ser un valor entero del rango (1,5), es decir,  1-2-3-4-5 en el cual el valor 1 representa el valor más bajo y el 5 el más alto. 