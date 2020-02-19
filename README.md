# descripcion-de-pandas

+ import pandas as pd: import libraries

+ url = 'https://raw.githubusercontent.com/justmarkham/DAT8/master/data/chipotle.tsv' matter from the url where we have the data table or data

+ tarea = pd.read_csv(url, sep = '\t' what is does is that the pd as a library uses it with the read to find the fastest or exact route where our file is from the url that we added before and then make a blank space that the rest is blank
+ tarea is shows me everything we have created or exported
+ tarea.head(10) the number we give is from 0 to the number that will show what is in the table
+ tarea.shape [0] what it does is read the vertical part bone shows the first column vertically from the beginning to the end

+ tarea.shape [1] it does the same with 0 but horizontally

+ tarea.info() our information on data numbers, types, columns, order , etc

+ tarea.columns from what i understood, it simply shows you what is horizontal, the upper columns that separate ir from its description

+ tarea.index from what i understood is the total of call the data it contains

c = chipo.groupby('item_name')
c = c.sum()
c = c.sort_values(['quantity'], ascending=False)
c.head(1): this code from what i understood is that the data that is reprinted in that column is added and shown as a table

+ c = chipo.groupby('choice_description').sum()
c = c.sort_values(['quantity'], ascending=False)
c.head(1):  here it does the dame function nothing more than other columns

+ total_items_orders = chipo.quantity.sum()
+ total_items_orders: is the total data that there is


+ chipo.item_price.dtype: what i understood is that it showsthe dtype that i have in that column
+ tarea.item_price.str.slice(1) show from 0 to 1 all those columns from horizontal and vertical
+ tarea.item_price.dtype show the type of data

+ orders = tarea.order_id.value_counts().count()
orders: son los datos totales pero de esa columna en espesifico
tarea['item_price'].sum(): the sum od the results of that table


+ chipo.item_price.dtype: the type od data that is

+ revenue = (chipo['quantity']* chipo['item_price']).sum()
print('Revenue was: $' + str(np.round(revenue,2))) : from what i understood is that i knew it but in a total way of the whole column

+ chipo['revenue'] = chipo['quantity'] * chipo['item_price']
order_grouped = chipo.groupby(by=['order_id']).sum()
order_grouped.mean()['revenue'] sample of the column that puts the average amount that has been for income

+ chipo.groupby(by=['order_id']).sum().mean()['revenue'] : And this is the second way to do it.

+ chipo.item_name.value_counts().count(): this part shows the different data that has been added
