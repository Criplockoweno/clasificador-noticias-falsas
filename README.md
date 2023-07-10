# Clasificador de noticias falsas
## Descripcion
Este proyecto es un reto propuesto por el Club de Machine Learning de la Universidad de Tennessee, Knoxville hace aproximadamente 5 años en la plataforma de Kaggle. El objetivo del mismo es crear un programa que sea capáz de identificar un posible artículo con noticias falsas. El enlace con la información de este reto es el siguiente: https://www.kaggle.com/competitions/fake-news/overview

Este es un problema inusual de regresión, es decir, que es un problema de aprendizaje supervisado. Cada valor del Dataset tiene 4 etiquetas: id, autor, texto y etiqueta, esta última para definir si una noticia es falsa o no. En base a esto se pueden entrenar clasificadores que van a decidir si una noticia es falsa o no, basado solamente en las 3 primeras características . Sin embargo, hacer esto no es tan sencillo como pasar estos 3 features sin preprocesar a un clasificador ya que es demasiada información que no es útil  y tomaría mucho tiempo y poder computacional en entrenar ese clasificador, por no hablar de una optimización de parámetros. 

Para solucionar este problema primero se tiene que realizar un preprocesamiento de los datos y guardar la información resultante en Google Drive para no tener que procesar toda la información cada vez que se quiera ejecutar el proyecto desde cero. Con esta información procesada ya se pueden entrenar los modelos y lo que se va a hacer es concatenar toda la información en un solo campo y usar este campo para entrenar los modelos.
## Importancia

Este proyecto nos llamó la atención debido a que resuelve un problema que poco se está haciendo más prevalente, la desinformación en base a noticias falsas. Con herramientas como Quillbot o EssayGenius, solo se necesitan unos pocos detalles para poder escribir un artículo qe aparente ser una noticia real solo para ser una noticia falsa. 

Sin embargo, de la misma manera que la Inteligencia Artificial amenaza con la credibilidad de las noticias, también puede ayudarnos a descifrar si una noticia es falsa o no y ese es el propósito del proyecto. Si bien para testear los modelos se va a usar un split 80-20 para revisar la precisión de los clasificadores entrenados, si se usara un DataSet que solo contenga noticias en un idioma, donde no haya ninguna incertidumbre de si una noticia es falsa o no, podría crearse un modelo donde se le introduce las 3 etiquetas de información explicadas anteriormente para que nos devuelva si se trata de una noticia verdadera o falsa. 
