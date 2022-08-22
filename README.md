**PROYECTO W2-PANDAS-PROJECT**

El proyecto se ha dividido en 3 partes:

**a) planteamiento del problema**
Se tiene un dataset que contiene registros de ataques de tiburones con unas 2500 filas y 24 columnas. El objetivo final es analizar dichos datos y para ello primero se debe preseleccionar las columnas que se quiere analizar (para trabajar de manera eficiente) y limpiar la información teniéndolas en cuenta.

**b) limpieza del dataset**
Una vez que se ha seleccionado las columnas que posteriormente someteremos a estudio, se va a proceder a limpiar el dataset. Para ello, inicialmente se corrige el nombre de las columnas y se busca las filas duplicadas haciendo uso del comando drop_duplicates(). Esto nos permitirá trabajar con un menor número de datos y de manera más cómoda y eficiente. A continuación, se hace la limpieza de las columnas que se quieren analizar (case__number, date, year, fatal_(y/n), activity, species, type, sex, country, area). Este paso se ha subdividido en 2 partes: la primera de ellas se corresponde con un tratado general de estos datos, mientras que la segunda es una limpieza individual de cada ellas. El primer proceso consiste en borrar todas aquelas filas que carezcan de algún dato en las columnas previamente mencionadas. El segundo se trata de de modificar los datos, para intentar agruparlos y cambiar su tipo (object) a uno más coherente para su posterior análisis.
Después, se procede a la limpieza de las columnas indeseadas, sustituyendo sus valores por 'unknowns' o '0', según corresponda. 
Para finalizar, se resetean los indices y se guarda el dataset de los datos limpios (datttacks.csv) para su posterior análisis.

**c) análisis y conclusiones**

Tras la limpieza, se grafican los resultados de las columnas seleccionadas. El análisis comienza con una figura, donde aparecen representado el número de ataques, incluyendo si son fatales o no, en función del año en que tuvieron lugar. Mediante su visualización, se pueden intuir que durante el siglo XIX y principios del XX no se tomaban muchos registros o no se producián tantos ataques, como empieza a ocurrir a principios de los 70. Esta falta de datos se puede deber a que no se tenían los medios suficientes para tomar dichos registros, o que simplemente el contexto histórico relevara la importancia de este estudio. Otro factor a tener en cuenta en el comportamiento de dicha figura es que la proporción de ataqus fatales va en detrimento, hecho que se puede deber a un avance tecnológico que permitió unos mejores equipos de rescate o sanidad.
Por los motivos que se han expusto previamente, a partir de ahora el análisis se centrará en los registros de los últimos 40 años (1978-2018). Mediante la representación de la informacion del dataset limpio, se llega a varias conclusiones, como que el país donde más ataques hay es USA, seguido de Australia y Sudáfrica. Tmabién se ha podido concluir que el tiburón blanco es el que más ataques ha realizado, y con mayor ''efectividad''.

Si se desea consultar las figuras, consulte el excel con las tablas dinámicas, o en su defecto, el PTT. 

