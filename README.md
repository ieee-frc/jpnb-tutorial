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
comnado se instalaran las herramientas restantes. 

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

### Creacion de entornos virtuales 

* `virtualenv <dir>`
    
    Por ejemplo, puede ser util tener una carpeta en $HOME con nombre <virtual_env>
    y tener los diferentes entornos virtuales dentro de ese directorio : 

* `virtualenv ~/virtual_env/python2`
    
    Una vez creado el entornor virtual, para activarlo : 

* `source  ~/virtual_env/python2/bin/activate`
    
    Y para instalar paquetes dentro de este entorno virtual : 

* `pip install <nombre paquete> `
    
    Para desactivar el entorno, solamente : 

* `deactivate`


### Creacion de Kernels de entornos virtuales 
    
Instalar ipykernel. Esto se puede hacer con el entorno virtual activado o en con el 
    entorno virtual desactivado, instalando este paquete en nuestro sistema. Si lo hacemos dentro del entorno
    tendremos que instalar este paquete dentro de cada entorno que querramos usar como kernel de jpnb. 
    Y además, tendremos que, luego de instalar desactivar y volverlo a activar el entorno. 

* `pip install ipykernel`
    
Crear el kernel con el nombre del entorno virtual. Es recomendable darle el mismo nombre que al directorio donde creamos ese 
    entorno virtual. En el caso del ejemplo superior, <python2> 

* `ipython kernel install --user --name=<name>`
    

Abrir jpnb y seleccionar el kernel 


Para desinstalar un kernel 


* `jupyter kernelspec uninstall <name>`


Para listar los kernels 

* `jupyter kernelspec list`
    
    
