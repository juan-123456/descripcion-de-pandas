# descripcion-de-pandas

import pandas as pd: importa las librerias 
url = 'https://raw.githubusercontent.com/justmarkham/DAT8/master/data/chipotle.tsv' importa desde la url donde tengamos la tabla de datos o los datos
tarea = pd.read_csv(url, sep = '\t' lo que hace es que el pd como libreria lo usa con el read para buscar la ruta mas rapida o exacta donde esta nuestro archivo desde la url que nosotros agregamos antes y despues haga un espacio en blanco que lo demas este en blanco
tarea me muestra todo lo que hemos creado o exportado.
tarea.head(10) el numero que poganmos es desde el 0 hasta el numero que mostrara lo que haya en la tabla.
