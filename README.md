Este proyecto busca facilitar herramientas interactivas para comprender conceptos básicos de estadística. El lenguaje de programación es [python](https://www.python.org/). Mediante la plataforma [anaconda](https://www.anaconda.com/) se crean los gráficos con [matplotlib](https://matplotlib.org/), controlados por [ipywidgets](https://github.com/jupyter-widgets/ipywidgets) en [jupyter](https://jupyter.org/) notebooks y visualizados con [Voilà](https://github.com/voila-dashboards/voila). [BinderHub](https://binderhub.readthedocs.io/) facilita el servidor para ejecutar los aplicativos en la red, por lo que no es necesario hacer ninguna descarga ni instalación. Inicializar la máquina virtual y configurar el sistema puede tomar un poco más de un minuto si hay mucho tráfico en los servidores; cuando cargan correctamente se ve como las animaciones a continuación:

## Estadística univariada
### Distribución normal [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Yagwar/stats_interact/master?urlpath=voila%2Frender%2Fdist_normal.ipynb)

En este gráfico encontramos un histograma y la curva de la distribución para unos números generados aleatoriamente con una distribución normal. Los controles permiten ajustar el *promedio*, la *desviación estándar* y el *tamaño de la muestra*. El botón *Fijar Cero* hace que el valor cero en el eje _**x**_ sea visible para mantener un punto de referencia al momento de ver como los parámetros de media y desviación estándar cambian la distribución. El botón *Reiniciar valores* modifica todos los parámetros para visualizar una distribución normal estándar, con *promedio=0* y desviación *estandar=1*, que son los valores iniciales cuando comenzamos a utilizar los controles.

[![Dist_norm](curva_normal.gif)](https://mybinder.org/v2/gh/Yagwar/stats_interact/master?urlpath=%2Fvoila%2Frender%2Fdist_normal.ipynb)


## Estadística Bivariada
### Regresión Lineal simple - Correlación [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Yagwar/stats_interact/master?urlpath=voila%2Frender%2Fcorrelaciones.ipynb)

Es un gráfico de dispersión con números generados aleatoriamente. La pestaña de **datos** contiene los controles permiten generar los puntos en el sistema de coordenadas. Los valores en _**x**_ son generados mediante números aleatorios con una distribución normal, ajustando el *promedio*, la *desviación estándar* y el *tamaño de la muestra*. Los valores en _**y**_ son calculados a partir del modelo de regresión simple: 

<img src="https://render.githubusercontent.com/render/math?math=\hat{y}= m*x %2B \beta_{0} ( %2B \epsilon)"> 

Cada valor de _**x**_, se multiplica por la *pendiente* (_**m**_), más el *intercepto* (_**beta_0**_) y se le agrega un valor de *dispersión* ( _**epsilon**_ ) que es un número aleatorio generado con una distribución normal, de promedio cero y una desviación estándar proporcional a la desviación estándar en _**x**_.

La pestaña **gráfico** controla aspectos estéticos. El control de *Transparencia* modifica el color de los puntos, lo cual facilita diferenciar e identificar la densidad de la nube de puntos cuando el tamaño de la muestra es grande. El botón *Fijar origen* hace que el valor cero en abos ejes sea visible para mantener un punto de referencia al momento de modificar la generación de los puntos. El botón *Reiniciar valores* modifica todos los controles a sus valores iniciales.

[![regres](regresion.gif)](https://mybinder.org/v2/gh/Yagwar/stats_interact/master?urlpath=%2Fvoila%2Frender%2Fcorrelaciones.ipynb)


Hecho con : <img src="https://github.com/voila-dashboards/voila/raw/master/docs/source/voila-logo.svg?sanitize=true" width="48">
