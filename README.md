# Tutorial de Jupyter Notebook 
<p align="center">
<img src="https://github.com/ieee-frc/jpnb-tutorial/blob/master/Slides/img/main-logo.png" width="200" height="200" />
</p>

[Slides](#)

## Instrucciones instalacion 

### Windows 

Si bien se puede instalar solo Jupyter Notebook, lo recomendado es instalar un 
entorno, Anaconda, que contiene este interprete, IDEs, herramientas de desarrollo 
y visualizacion, administrador de paquetes, etc. 

Se puede instalar solo Jupyter Notebook si ya tiene instalado Python (y el gestor de 
paquetes `pip` que generalmente se instala con Pyhton). Los pasos a seguir se 
pueden encontrar en la web de [Jupyter Notebook](https://jupyter.org/install)


Para instalar *Anaconda* se puede descargar el instalador desde su 
[pagina web](https://www.anaconda.com/products/distribution). Una vez instalado, se puede 
lanzar este programa y desde abrir jupyter notebook. 


### Linux 

En Linux tambien podemos instalar Anacoda, pero si queremos manejar nosotros mismos
entornos virtuales, paquetes, etc, es recomendable intalar la herramienta por separado. 

Para instalar Jupyter Notebook simplemente: 

* `sudo apt update`

* `sudo apt install jupyter-notebook`

Es recomendable instalar otras herramientas de jupyter como `kernelspecs`, para poder 
adminisitrar kernels. Para ello, cambiar el comando por: 

* `sudo apt install jupyter`

Si ya habian lanzado el comando anterior instalando solo notebook, al lanzar este 
comnado se instalaran las herramientas restanteces. 

 Tambien podemos instalarlo haciendo: 

* Instalamos pip3 y dependencias para Jupyter Notebook: 
`sudo apt install python3-pip python3-dev`

* Instalamos jupyter notebook usando pip: 
`pip3 install jupyter-notebook`. 


## Entornos virtuales 

### Instalacion 
Para instalar *virtualenv*, la herramienta para crear entornor virtuales: 

* `sudo apt update`

* `sudo apt install virtualenv`

En windows, con el mismo anaconda se pueden crear entornos virtuales. Revisar su 
pagina web para ver las instrucciones. 


### Creacion de Kernels de entornos virtuales 


