# Preprocesador Less
http://lesscss.org/

## Comparación


### LESS
* Mejor prestaciones para sitios webs
* Nomenclatura más sencilla (más similar a CSS)
* Curva de aprendizaje menor
* Pocas dependencias
* Funciona bajo Javascript


### SASS
* Mejor prestaciones para aplicaciones webs
* Mucho más potente
* Ideal para grandes hojas de estilo
* Mejor compilación
* Funciona bajo Ruby

# ¿Qué es Less?

LESS CSS es una ampliación a las famosas hojas de estilo CSS, pero a diferencia de estas funciona como un lenguaje de programación, permitiendo el uso de variables, funciones, operaciones aritméticas, entre otras, para acelerar y enriquecer los estilos en un sitio web. No reemplaza a CSS, de hecho el resultado final es una hoja de estilos css completamente funcional y compatible, simplemente ofrece mejoras en el área de desarrollo, por lo que usarlo se vuelve recomendable si quieres ahorrar tiempo de desarrollo, utilizar características avanzadas de estilos y para ahorrarte trabajo —de allí su nombre: less css (menos css).
¿Qué funcionalidades aporta? ¿puedo usar funciones o variables?
Less tiene muchas características pero se va a mencionar unas más relevantes

## Variables
Las variables en less funcionan de forma similar a las constantes en los lenguajes de programación, permitiendo definir valores que podrán ser reutilizados en cualquier parte de la hoja de estilo, e incluso entre otras hojas de estilo.
```
@variable: valor;
``` 
 
 
 
 
## Mixins
Los mixins funcionan de forma similar a las clases CSS pero con características de funciones de programación. Es decir que pueden ser llamadas desde otras clases para obtener su valor y además permiten parámetros, aunque no es necesario utilizarlos. Esta característica  hace posible definir una clase dando flexibilidad para variar algunos estilos como el color o tamaño del elemento. Su sintaxis, en el caso de que usemos parámetros,  es la siguiente:
```
.mi_mixin(color: valordefecto){
 font-size:2em;
  color:@color;
  margin:0.2em;
}
```
## Funciones de color

Las funciones de color son funciones pre-definidas de Less CSS que permiten alterar un color, para hacerlo más claro, oscuro, saturado, desaturado, cambiarle la tonalidad, etc.
* “lighten” para aclarar un color.
* “darken” para oscurecerlo.
* “saturate” para saturar, o «aumentar el color».
* “desaturate” para reducir la saturación, o «reducir el color».
* “fadein” para resaltar quitándole transparencia.
* “fadeout” para disimular usando transparencia.
* “fade” para cambiar la transparencia al 50%.
* “spin” para cambiar el tono de color.
* “mix” para mezclar dos colores.

Su sintaxis sería:    
```
   lighten(@color, 30%);  
   darken(@color, 30%);
```

## @import
Se usa para importar los archivos en el código. Difunde el código LESS en diferentes archivos y permite mantener la estructura del código fácilmente. Puede poner las declaraciones @import en cualquier lugar del código.

Ejemplo:
```
   @import "button";
```
Este se importa desde un archivo **button.less** hacia el archivo **styles.less**.

## Frameworks o librerías
Less soporta gran cantidad de frameworks pero vamos a mencionar algunos de estos

#### UI/Theme Frameworks y Componentes 
* **1pxdeep:** Es un tema plano de Bootstrap que proporciona potentes controles de combinación de colores.
* **Bootflat:** Es un framework de código abierto basado en Bootstrap.
* **BootPress:** Es un framework PHP basado en CMS de archivo plano
* **Bootstrap:** Es un potente framework de front-end móvil para un desarrollo web más rápido y sencillo.
* **Bootswatch:** Es un theme de código abierto que proporciona temas gratuitos para Bootstrap.
* **Cardinal:** Es un framework CSS para dispositivos móviles que permite mantener CSS para sitios web, interfaces de usuario y aplicaciones receptivos.

referencias: https://www.tutorialspoint.com/less/less_frameworks.htm


## Tutorial de instalación
https://www.youtube.com/watch?v=vPFbW3utUuU 

### Less en Mac:
```
sudo npm install -g less
```
### Instalar Less en el Visual Code:

- Colocamos esto en el head del HTML:
```
   <link rel="stylesheet/less" type="text/css" href="styles.less"/>
```
- Colocamos esto en el final del body
```
   <script src="//cdn.jsdelivr.net/npm/less@3.13"></script>
```
### Instalar Less con Bash:
```
npm install less -g
```
### Usar Less de forma global:
```
npm i less --save-dev
```
### Verificar la versión de Less:
```
lessc -v
lessc --version
```

## Easy LESS

Una vez instalado el LESS dentro del Visual Code, buscamos un plugin llamado ** Easy ** Less para instalarlo. Esto nos ayudará mientras estemos trabajando con LESS.
Si el archivo de styles.css se borra accidentalmente el plugin creará uno inmediatamente luego de guardar nuestro proceso en el archivo de styles.less con Ctrl + S en windows o Command S en MAC.
Además, compila errores integrados con los errores estándar y lista de advertencias. 
Es configurable, según sea necesario: 
- Soporte de archivos principal 
- archivo de salida alternativo
- supresión de salida -compresión 
- https: //github.com/postcss/autoprefixer Plugin incluido que es  un complemento PostCSS para analizar CSS y agregar prefijos de proveedores a las reglas de CSS utilizando valores de Can I Use (https://caniuse.com/). Es recomendado por Google y utilizado en Twitter y Alibaba.



#### referencias
 - https://www.genbeta.com/desarrollo/less-el-lenguaje-de-hojas-de-estilo-dinamico
 - https://ivanmendoza.net/desarrollo-web/introduccion-less-css

#### Documento y presentación

- https://docs.google.com/document/d/19SzptLeLK6Vd3yasJr4Holqf9MqjkpbtDn-nzsXbJRQ/edit
- https://www.powtoon.com/s/fHQ51InB9Jf/1/m
