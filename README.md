# Proyecto-Retencion-Clientes
Estudiar al detalle cómo se comportan los usuarios y las usuarias de servicios en una cadena de gimnasios

---

CONTEXTUALIZACIÓN

La cadena de gimnasios Model Fitness está desarrollando una estrategia de interacción con clientes basada en datos analíticos.

Uno de los problemas más comunes que enfrentan los gimnasios y otros servicios es la pérdida de clientes. ¿Cómo descubres si un/a cliente ya no está contigo? 

En el caso de un gimnasio, tiene sentido decir que un/a cliente se ha ido si no viene durante un mes. Pueden ocurrir excepciones, pero por lo general, si un/a cliente se une, viene varias veces y luego desaparece, es poco probable que regrese.

El objetivo principal es analizar los datos del gimnasio y elaborar una estrategia de retención de clientes.

--- 
Para desarrollar el proyecto se siguieron las siguientes etapas:
#### ETAPAS DEL PROYECTO 
* Etapa 1: Lectura de datos.
* Etapa 2: Análisis exploratorio de datos y preprocesamiento.
* Etapa 3: Construir un modelo para predecir la cancelación de usuarios.
* Etapa 4: Crear clusteres de usuarios. 
* Etapa 5: Recomendaciones y Conclusiones.

---
ALGUNAS CONCLUSIONES

### Conclusiones Generales del Análisis Estadístico:

* Los usuarios que tienen contratos cortos (1 mes) o poco tiempo de vida como clientes (Lifetime) son más propensos a cancelar.
* Baja frecuencia de visitas, tanto en términos de promedio general como en el mes actual, está fuertemente correlacionada con la cancelación. Los usuarios que no participan regularmente tienden a abandonar.
* La participación en visitas grupales parece estar relacionada con una mayor retención. Los clientes que asisten a clases grupales tienen mayor tendencia a quedarse, posiblemente porque disfrutan más de la experiencia social.
* Las personas que gastan más dinero en servicios adicionales (cafetería, productos deportivos, etc.) suelen ser clientes más leales.
* Los usuarios que se inscribieron a través de una oferta con amigos o que trabajan para empresas asociadas también muestran menor tendencia a cancelar.

### Conclusiones Modelo de Predicción de Cancelación de Clientes:

* El modelo de Bosque Aleatorio ha mostrado consistentemente mejores resultados en métricas clave (accuracy, precision, y recall). Por lo tanto, parece ser más adecuado para predecir la cancelación de clientes.

### Conclusiones Segmentación de Clientes:

* Los clusters obtenidos muestran diferencias notables en el comportamiento. Algunos grupos de clientes tienen una alta tasa de cancelación, mientras que otros son más leales.
* Usuarios con contratos de 1 mes y aquellos con baja frecuencia de visitas forman clusters con una mayor probabilidad de cancelación.
* Usuarios jóvenes con poca antigüedad en el gimnasio tienden a abandonar con mayor frecuencia.
* Clientes de empresas asociadas, o aquellos que viven cerca del gimnasio, tienen tasas de retención más altas.
* El cluster 0 es el más leal (solo 2% desertan), algunas de sus características son: 95% de ellos viven o trabajan cerca del gimnasio y el 78% trabajan en una empresa asociada. Más de la mitad de ellos ingresaron al programa a través de un amigo, además son los que más visitas registran y sus contratos son más largos. 
* El cluster con mayor tasa de cancelación corresponde al número 3 (51,4% desertan) algunas de sus características son: Si bien viven o trabajan cerca del gimnasio, solamente el 35% pertenece a una empresa asociada. Un 25% ingresa a través de una promo de amigos y su característica más importante es que los contratos que realizan son cortos y las visitas registradas semanales y mensuales son muy pocas. 

Con base en las características de los clústeres es posible identificar a los usuarios más propensos a cancelar y diseñar estrategias específicas para retenerlos:

### Recomendaciones para Reducir la Cancelación:

* Fomentar la Participación en Clases Grupales:Los usuarios que asisten a clases grupales tienden a permanecer más tiempo en el gimnasio. Una estrategia efectiva sería promover más las actividades grupales, como clases de yoga, spinning, o crossfit, especialmente para aquellos clientes que no participan actualmente.
* Ofrecer Incentivos para Contratos de Mayor Duración: Los contratos de un mes están asociados con una mayor tasa de cancelación. Se puede diseñar un esquema de descuentos o beneficios adicionales para clientes que opten por contratos más largos (3, 6 o 12 meses), incentivando su permanencia.
* Monitorear Clientes con Baja Frecuencia de Visitas: Implementar un sistema de alertas que detecte a clientes que han reducido su frecuencia de visitas. Ofrecerles recordatorios personalizados, promociones especiales o sesiones de entrenamiento gratuitas para incentivar su regreso.
* Programas de Fidelización y Gastos Adicionales: Dado que los clientes que gastan más en servicios adicionales tienden a ser más leales, se pueden crear programas de fidelización que premien el uso de estos servicios, como descuentos en cafetería o masajes después de un cierto número de visitas.
* Segmentación y Marketing Personalizado: Usar los clusters de clientes para aplicar marketing personalizado. Por ejemplo, los clientes jóvenes y nuevos, que tienden a cancelar más rápidamente, podrían recibir una atención especial, con seguimiento personalizado y comunicaciones que destaquen los beneficios de permanecer a largo plazo.
*Programas de Referidos con Amigos: Dado que los clientes que se inscriben a través de una promoción con amigos tienden a quedarse más tiempo, se podría expandir este tipo de promociones para captar más clientes leales.
* Mejorar la Experiencia del Cliente Cerca del Fin del Contrato: Los clientes que están cerca del fin de su contrato deben ser incentivados a renovarlo con campañas especiales, como descuentos por renovación temprana o beneficios adicionales.

