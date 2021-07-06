# Datascience_test

El presente trabajo busca poder estimar el tiempo total de entrega de una gran cantidad de pedidos de la app Cornershop. Par poder lograr estas estimaciones se utilizan distintos modelos matemáticos de Machine Learning. Como inputs se utilizan 4 archivos que se describen a continuación junto a los atributos que trae cada uno:

**order_products.csv:**
- order_id: ID of the order
- product_id: ID of the product
- quantity: The quantity ordered of this product
- buy_unit: The unit of the product (KG/UN)

***orders.csv:***
- order_id: ID of the order
- lat: The latitude of the delivery location
- lng: The longitude of the delivery location
- promised_time: The delivery time promised to the user
- on_demand: If true, the order was promised to be delivered in less than X minutes
- shopper_id: ID representing the shopper completed the order.
- store_branch_id: ID of the store branch
- total_minutes: The total minutes it took to complete the order (label)

***shopper.csv***
- shopper_id: ID of the shopper
- seniority: The experience level of the shopper.
- found_rate: Percentage of products found by shopper historical.
- picking_speed: Historical picking speed, products pr minutes.
- accepted_rate: Percentage of orders historically accepted by shopper
- rating: client rating of shopper
- 
- ***storebranch.csv:***
- store_branch_id: ID of the store branch
- store: ID representing the store
- lat: Latitude of the branch location
- lng: Longitude of the branch location

En el trabajo se realizan varios procesos que comienzan con unificar las bases en un solo dataset, posteriormente se imputo data, se generaron dummies y se crearon nuevas variables para lograr enriquecer la data y predecir de mejor forma. Luego  se realiza un análisis exploratorio para entender la distribución de las variables y conocer la relación existentes entre ellas, principalmente como influyen en la variable que se busca predecir. Luego se ajustaron dos modelos de ML que fueron una regresión lineal multiple y un random forest.

En el repositorio se encuentra el archivo principal que es DS Cornershop test.ipynb donde se encuentra detalladamente paso a paso el proceso utilizado para llegar a  predecir el tiempo total de las ordenes. Además, se encuentra una carpeta llamada data 1 donde se encuentran las bases de datos inciales entregadas por el equipo reclutador y las predicciones logradas por el mejor modelo obtenido.




