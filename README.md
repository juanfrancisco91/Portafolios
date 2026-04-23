# Analisis y Predicciones de Data Set Titanic
## Resumen del Proyecto
### El Titanic, una de las embarcaciones mas impresionante y famosas que a visto la humanidad y en este esta basasdo su Data Set. El Data Set consta de 11 Columnas de diferentes tipos como age(edad), fare(precio del boleto) Pclass(Clase dentro del barco) etc. El objetivo principal de las predicciones era lograr mas de un 80% en la metrica accuracy y utilizando el modelo Random Forest lo cual fue logrado con exito. 

## Analisis Exploratorio
<img width="831" height="528" alt="image" src="https://github.com/user-attachments/assets/cc1cee7e-2816-401f-890e-10ebdb25b535" />
  
  ### En este Grafico Observamos que la ubicacion de cada clase dentro del barco fue crucial para la supervivencia porque dependiendo la clase del boleto la posicion variaba.
 
<img width="831" height="528" alt="image" src="https://github.com/user-attachments/assets/9125c239-5d36-4eb6-8f52-2f4a99f0743b" />
  
  ### Aqui vemos la historia completa, ya que si solo nos llevamos de la imagen anterior pensariamos que la Tercera Clase fue de la que mas se salvaron pero comparando el total de personas que habian fue la que mas perdio.
  ### La que tuvo el mejor balance fue la Primera Clase ubicada de manera mas centrica lo que permitio su evacuacion inmediata.
  ### La Clase Media se mantiene en un punto intermedio ya que estaban mas distribuidos dentro del barco que otras claese
  ### El porcentaje Total de Sobrevivientes al Titanic fue del 38.38%.
  
  	
<img width="1015" height="463" alt="image" src="https://github.com/user-attachments/assets/84dfb4f2-774c-49cb-a776-768fead1da67" />

  ### Obsevamos estos porcentajes de mejor manera en este grafico de pastel, divido por cada clase entre Sobrevivientes y Fallecidos.

<img width="831" height="528" alt="image" src="https://github.com/user-attachments/assets/ff71c00f-5afa-458b-b038-765bfefe68ec" />

  ### Este grafico nos muestra la verdad absoluta que siempre se mencionaba en las historias, mujere y niños primeros habiendo una diferencias bastante considerable frente a los hombres.

<img width="1085" height="477" alt="image" src="https://github.com/user-attachments/assets/eeddc23d-155b-4561-8f6a-02ae512d4dfc" />

## Mapa de Calor
<img width="838" height="528" alt="image" src="https://github.com/user-attachments/assets/01c25739-be68-4ea6-bd8d-03adf348e031" />
  
  ### Podemos ver variables como Parch y Sibsp con mas de un 0.40 una de las mas cercanas a 1, lo que nos indica que cuando suben una tiende a subir la otra.

## Importancia De Variables 
<img width="1189" height="590" alt="image" src="https://github.com/user-attachments/assets/dfac674a-c651-4acc-9995-3ed54d20826c" />
  
  ### Este Grafico es uno de los mas importantes principalmente para el ajuste del modelo, nos muestra cual es la importancia de las variables dentro del modelo. Se utiliza La Reduccion de Impureza de Gini que mide como estan mezcladas las clases en un nodo y cuanta mas cerca el valor a 0 significa que esta mas libre de Impureza, en este caso utilizamos la funcion "features_importances" que viene en la libreria de Scikit-Learn y que nos calcula que tanta impureza logro reducir cada variable en promedio. Las variables que limpian mejor los datos, ganan los puntajes mas altos.

  ### En este caso observamos algo curioso y es una distribucion Heterogenea en las importancias de las variables en el modelo, con un claro ganador por diferencia como es la variables "Sex". Este grafico nos ayuda a visualizar con las que nos covendria quedarnos en caso de un nuevo entrenamiento unicamente filtrando las que cumplan un minimo de importancia.

## Prediccion del Modelo

<img width="831" height="528" alt="image" src="https://github.com/user-attachments/assets/9bdf205a-1e66-4a37-bc6b-97887d2a3ab6" />


## Metricas De Evaluacion

<img width="1501" height="512" alt="image" src="https://github.com/user-attachments/assets/ccef2c65-199b-4488-a3b3-f099103065e4" />
  
  ### Utilizamos 3 metricas para evaluar el modelo accuracy, recall y precision.
  Con unos resultados bastantes solidos con mas de un 80% de accuracy lo que nos dice que el modelo clasifica bien entre las clases a predecir.
  El Recall nos cuenta la cantidad de Falsos negativos que captura el modelo con mas de un 80%
  Precision con mas de un 70% captura los Falsos positivos que captura el modelo,

