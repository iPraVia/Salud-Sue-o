El siguiente es el proceso de análisis de un dataset el cual contiene datos relacionados a la ocupación del usuario, información de su actividad física como también información relacionada a su conducta de sueño y su condición física, a lo largo del informe se realizaran varias visualizaciones. El data set cuenta con un total de 13 variables o columnas y un total de 374 filas.

##### Ocupacion y probabilidad de tener un desorden del sueño

![ocupacion - desorden sueño](https://github.com/iPraVia/Salud-Sue-o/blob/415b5593e21b06c756faba72c90114331cf92705/graficos/bar_ocupacion_trastorno_sueno_porcentaje.png)

Observando el set de datos tomamos la decision de analizar que porsentaje de la muestra puede sufrir algun tipo de desorden en el sueño dependiendo de la ocupacion que realiza, este analisis arrojo que los representantes de ventas tienen un 100% de probabilidad de sufrir algun tipo de desorden del sueño, el problema con la muestra es que solo contiene dos personas con ese cargo y al ser una cantidad tan reducida puede no representar correctamente la realidad de la poblacion. Lo mismo ocurre con la ocupacion Manager que solo contiene 1 dato dentro de la muestra y nos dice que el 0% de los Manager poseen desorden del sueño.

Dos ocupaciones del area de la medicina, enfermera y doctor poseen registros suficientes en la muestra para realizar un analisis que podria reflejar un poco mas acertadamente lo que ocurre con la poblacion. Los resultados indicaron que el 87% de las enfermeras poseen algun tipo de desorden del sueño un porcentaje bastante alto comparado con el porcentaje de doctores que posee algun desorden del sueño donde la cifra es solo un 9.8%.

##### Analisis de la ocupacion: Nurse(enfermera/o)

Para determinar si las variables estan correlacionadas entre si se realizo un proceso de escalamiento de datos y agrupacion para graficarlo en un biplot, los datos que se tomaron fueron las horas que duerme una persona, junto con el nivel que le daria a su calidad del sueño, tambien se analizara la cantidad de pasos que da una persona por dia junto con el nivel de actividad fisica que realiza.

![biplot](https://github.com/iPraVia/Salud-Sue-o/blob/2a3aca480edba1b00f240c1cbb046e2fd1ae722f/graficos/biplot_nurse.png)

En el grafico anterior podemos ver como se relacionan las variables entre si, en este caso el nivel de actividad fisica estan altamente ligados a la cantidad de pasos diarios que da una persona, como tambien la calidad del sueño con la duracion del mismo. Tambien podemos apreciar que mientras la edad aumenta el nivel de actividad fisica comienza a disminuir, pero no asi la calidad del sueño que pareciera aumentar conforme lo hace la edad.

##### Correlacion estres

Para continuar con el analisis se realizo un regresion lineal entre la variable estre y otras variables asociadas al sueño y otras asociadas a la actividad fisica.

![regresiones lineales](https://github.com/iPraVia/Salud-Sue-o/blob/2a3aca480edba1b00f240c1cbb046e2fd1ae722f/graficos/regplot_nurse_estres_varios.png)

Al parecer las variables de estudio se comportan de manera similar. La duracion del sueño junto con la calidad de este al aumentar disminuye el estres, no asi las variables asociadas a la actividad fisica, que nos indican que ha mayor actividad fisica mayor es el nivel de estres que puede persivir una persona

Al analizar una de las ocupaciones con mas usuarios encuestados pudimos determinar que la calidad y cantidad de horas de sueño que tiene una persona afectan positivamente la sensacion de estres percibida por el usuario, y que el nivel de actividad fisica tiene un impacto negativo en el nivel de estres percibido por una persona.

Siguiendo con el analisis exploratorio de los datos realizaremos visualizaciones en busca de algun otro factor que pueda estar asociado con el padecimiento de algun tipo de desorden del sueño.

##### Probabilidad de tener algun tipo de desorden del sueño segun IMC

![IMC - desorden sueño](https://github.com/iPraVia/Salud-Sue-o/blob/2a3aca480edba1b00f240c1cbb046e2fd1ae722f/graficos/trastorno_sueno_BMI.png)

Al analizar que tan probable es que una persona posea algun tipo de desorden del sueño basandoce en el IMC que posee, nos podemos dar cuenta que existe una alta probabilidad en caso de estar dentro de la categoria de 'Sobrepeso' y en la categoria 'Normal'.

Ya que al parecer el sobrepeso podria estar asociado con el padecimiento de algun tipo de desorden del sueño lo siguiente sera realizar un analisis entre el IMC y la ocupación.
##### Analisis IMC y ocupacion

![IMC -ocupacion](https://github.com/iPraVia/Salud-Sue-o/blob/2a3aca480edba1b00f240c1cbb046e2fd1ae722f/graficos/ocupacion_BMI.png)

En el grafico anterior hemos agrupado los datos por ocupacion y por nivel de IMC, de esta manera podemos identificar cual de las ocupaciones puede tener usuarios con altos indices de IMC e identificar si esto tiene alguna relacion con el padecimiento de desordenes del sueño, a simple vista podemos ver que la ocupacion Nurse enfermera tiene una alta cantidad de usuarios en la categoria sobrepeso.

Lo siguiente sera determinar que porcentaje de las enfermeras en la categoria de sobrepeso poseen algun tipo de desorden del sueño.

##### IMC 'sobrepeso' -  desorden del sueño 

![IMC sobrepeso - desorden sueño](https://github.com/iPraVia/Salud-Sue-o/blob/2a3aca480edba1b00f240c1cbb046e2fd1ae722f/graficos/sobrepeso_desorden_sueno.png)

En el grafico anterior podemos visualizar el porcetaje de enfermeras que estan dentro de la categoria sobrepeso del IMC que poseen algun tipo de desorden del sueño.

Despues de los analisis anteriores podemos concluir de que tanto la calidad del sueño, el tener un estilo de vida activo o tener un IMC ligeramente elevado podrian influir significativamente en el nivel de estres de una persona. Si bien este no es un nivel alto dentro de lo que son las categorias de IMC el entorno podria ser bastante influyente ya que esta podria alterar su propia percepción de IMC y afectar negativamente su nivel de estres.

En un entorno de trabajo demandante el buen descanso puede ayudar de manera favorable a disminuir el estres, por el contrario el nivel de pasos de una persona nos puede indicar que fue un trabajo o turno movido, lo que estaria relacionado a la alta cantidad de estres percibida por el usuario, ya que de los datos obtenidos pudimos rescatar que una alta cantidad de pasos diarios o actividad fisica esta relacionado con un alto nivel de estres, dentro de lo que viene siendo la ocupacion enfermera. 
