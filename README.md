# proyecto-Dataxperience

## Análisis de datos para la identificación y predicción de amenazas de ciberseguridad

![Imagen del proyecto](https://images.unsplash.com/photo-1498050108023-c5249f4df085)

## Integrantes

- Derly Benitez
- Juan Vergara Ramirez
- Lina Vargas Lasso


## Resumen

Este proyecto aplica ciencia de datos para analizar el tráfico de red, identificar patrones asociados a ataques informáticos y construir un modelo predictivo sencillo que clasifique el tráfico como normal o malicioso. Se desarrolla en tres etapas: limpieza de datos, estadística descriptiva y visualización con modelo predictivo.

**Pregunta central:** ¿cómo podemos usar la ciencia de datos para identificar patrones de comportamiento asociados a ataques informáticos y anticipar posibles amenazas?

## Dataset

Se utilizó **UNSW-NB15 (conjunto de entrenamiento)**, creado por el Cyber Range Lab de UNSW Canberra. Contiene tráfico de red normal y ataques simulados.

- Copia usada en el proyecto: [UNSW_NB15_training-set.csv](https://raw.githubusercontent.com/stijnhuysman/DissertationData/main/UNSW_NB15_training-set.csv)
- Variable objetivo: `label` (0 = tráfico normal, 1 = ataque)

## Tabla de contenido

| Datos | [Dataset UNSW-NB15](https://raw.githubusercontent.com/stijnhuysman/DissertationData/main/UNSW_NB15_training-set.csv) |            
| Cuaderno (Colab) | [Abrir el cuaderno](Copia_de_Proyecto_Ciberseguridad_UNSW_NB15.ipynb) |          
| Presentación | [Ver presentación](Ciberseguridad%20con%20UNSW-NB15%20detectar%20ataques%20con%20ciencia%20de%20datos.pdf) |        
| Video | [Ver video](https://youtu.be/sFslDpxoPHk?si=We61sW6nRwIGreaP) |       


## Conclusión

El análisis del dataset UNSW-NB15 mostró que el tráfico malicioso se diferencia del normal en variables clave como sttl, rate, ct_dst_src_ltm y | ct_state_ttl. Mientras que la regresión logística alcanzó un accuracy del 83% y un recall del 89% en la clase ataque, el modelo Random Forest superó este |  desempeño logrando un 97% de accuracy y un 95% de recall, detectando 95 de cada 100 ataques reales. Este enfoque funciona como un filtro inicial de | alertas para que el equipo de seguridad (SOC) priorice el tráfico sospechoso y reduzca el riesgo de amenazas no detectadas. 


