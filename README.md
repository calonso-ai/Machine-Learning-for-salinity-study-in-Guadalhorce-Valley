# Técnicas de aprendizaje automático para el análisis de la salinidad de aguas en el valle del Guadalhorce

La necesidad principal del trabajo surge de la inquietud de la Junta de Andalucía por conocer lo que muestran los datos recogidos, y en particular, los datos sobre la salinidad de la presa Guadalhorce y como influye en el resto de presas.

En la actualidad de se mezcla el agua de las tres presas, dependiendo de su capacidad, para obtener agua para consumo, regadío, ganadería, etc.

Lo que se pretende es aplicar métodos de aprendizaje automático para conocer que parámetros influyen en la salinidad de la mezcla y cual es la mezcla óptima de las tres presas de cara a sesgar agua para consumo, regadío y ganadería.

Utilizar la menor cantidad de agua dulce, proveniente de Guadalteba y Conde de Guadalhorce, para que la mezcla fuera utilizable. 

Como influyen parámetros, como la altura, lluvia, etc, en la salinidad del agua de la presa Guadalhorce.

Relacionar la salinidad de la presa Guadalhorce la salinidad que se obtiene de la mezcla.

Se tomarán los datos proporcionados por la Junta de Andalucía, que recogen diferente información acerca de las presas, se preprocesarán, se analizarán y se visualizarán para extraer un análisis pormenirizado.

Una vez se han consolidado los 8 ficheros csv que pueden encontrarse en la carpeta dataset, que un dataframe con 2894 registros y 73 variables. Entre estas 73 variables se encuentra la variable etiquetada, que será Salinidad_mezcla, que toma los valores:

  •	Mezcla de aguas no salina: 0 ≤  Salinidad_mezcla ≤ 900 --> Salinidad_mezcla = 0 

  •	Mezcla de aguas salina: Salinidad_mezcla > 900 --> Salinidad_mezcla = 1 

Esta variable contiene un gran número de missing values por lo que se estudiarán distintas metodologías de imputación. 

(Nota de ejecución: Para cada ejecución completa del script utilizar únicamente un método de imputación y el resto de métodos dejarlos comentados)

Una vez se completa la fase de preprocesado, se aplican los métodos; Arboles de decisión, Random Forest, SVM, AdaBoost y ANN para hallar un clasificador o predictor óptimo de la variable Salinidad_mezcla.

Para finalizar, se realizan varias predicciones de la variable Salinidad_mezcla con conjuntos nuevos de datos, para ver como varían distintas variables de interés.

(Nota de ejecución: En el apartado 5.)
