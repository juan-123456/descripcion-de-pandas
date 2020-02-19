# descripcion-de-pandas

+ import pandas as pd: importa las librerias

+ url = 'https://raw.githubusercontent.com/justmarkham/DAT8/master/data/chipotle.tsv' importa desde la url donde tengamos la
tabla de datos o los datos


+ tarea = pd.read_csv(url, sep = '\t' lo que hace es que el pd como libreria lo usa con el read para buscar la ruta mas rapida o exacta donde esta nuestro archivo desde la url que nosotros agregamos antes y despues haga un espacio en blanco que lo demas este en blanco
+ tarea me muestra todo lo que hemos creado o exportado.
+ tarea.head(10) el numero que poganmos es desde el 0 hasta el numero que mostrara lo que haya en la tabla.
+ tarea.shape [0] lo que hace es leer la parte vertical osea muestra la primera columna de forma vertical desde el inicio al final
+ tarea.shape [1] hace lo mismo de con 0 pero de forma horizontal
+ tarea.info() nuestra informacion sobre los numeros de datos, lo tipos, las columnas, el orden, etc
+ tarea.columns por lo que entendi simplemente te muestra lo que esta en horizontal osea las columnas de arriba que lo separan de su descripcion
+ tarea.index por lo que entendi es el total de todos los datos que contiene 
c = chipo.groupby('item_name')
c = c.sum()
c = c.sort_values(['quantity'], ascending=False)
c.head(1): este codigo por lo que entendi es que los datos que estan repeditos en esa columna se suman y se muestran como tabla.

+ c = chipo.groupby('choice_description').sum()
c = c.sort_values(['quantity'], ascending=False)
c.head(1):  aqui hace la misma funcion nada mas que de otras columnas 

+ total_items_orders = chipo.quantity.sum()
+ total_items_orders: es el total de datos que hay.


+ chipo.item_price.dtype: lo que entendi es que muestra los dtype que tenga en esa columna

+ tarea.item_price.str.slice(1) muestra del 0 a la 1 todas esas columnas desde horizontal y vertical

+ tarea.item_price.dtype muestra el tipo de dato

+ orders = tarea.order_id.value_counts().count()
orders: son los datos totales pero de esa columna en espesifico
tarea['item_price'].sum(): la suma de los resultados de esa tabla


+ chipo.item_price.dtype: el tipo de dato que es

+ revenue = (chipo['quantity']* chipo['item_price']).sum()
print('Revenue was: $' + str(np.round(revenue,2))) : por lo que entendi es que lo supa pero de forma total de toda la columna

+ chipo['revenue'] = chipo['quantity'] * chipo['item_price']
order_grouped = chipo.groupby(by=['order_id']).sum()
order_grouped.mean()['revenue'] muestra de la columna que se ponga el monto promedio que a habido por ingresos

+ chipo.groupby(by=['order_id']).sum().mean()['revenue'] : y esta es la segunda forma de hacerlo.

+ chipo.item_name.value_counts().count(): esta parte muestra los diferentes datos que se tiene agregados

