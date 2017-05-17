# linkRappi

Para añadir el link de rappi a tu página web debes seguir estos pasos:

1. Crear un div con un id llamado 'linkRappi' donde quieras que aparezca el link.

```
<div id="linkRappi"></div>
```

2. Agregar este script antes de finalizar el 'body':

```
<script src="https://s3-us-west-2.amazonaws.com/rappi-images-01-prod/web/linkRappi.min.js"></script>
```

3. Para ejecutar el plugin solo debes añadir estas linea despues de donde se agrego el script anterior:

```
  <script>
    (function() {
      addLinkRappi();
    })();
  </script>
```

esta función recibe 2 parametros:
  
* tipo de botón 'shadow radius big'

  shadow = agrega una sombra 
  
  radius = deja las esquinas redondeadas
  
  big    = es un poco mas grande el botón
  
  white  = Color blanco
  
  red    = color rojo

* Url donde va direccionar, tener en cuenta que si se ingresa un nombre con espacios se reemplazara con guiones(-),
  ejemplo: 'mi restaurante' = mi-restaurante



## Ejemplo configuración

```
  <script>
    (function() {
      addLinkRappi('radius shadow big', 'mi restaurante');
    })();
  </script>
```

si desea dejar el boton por defecto y solo agregar la url del restaurante:

```
  <script>
    (function() {
      addLinkRappi('', 'mi restaurante');
    })();
  </script>
```

## Ejemplo botones:

1. Por defecto:
```
  <script>
    (function() {
      addLinkRappi('', 'mi restaurante');
    })();
  </script>
```
![alt text](https://github.com/esteban-vera/linkRappi/blob/master/images/button-default.png?raw=true)

2. Por defecto con sombra:
```
  <script>
    (function() {
      addLinkRappi('shadow', 'mi restaurante');
    })();
  </script>
```
![alt text](https://github.com/esteban-vera/linkRappi/blob/master/images/button-default-shadow.png?raw=true)

3. Con bordes redondeados:
```
  <script>
    (function() {
      addLinkRappi('radius', 'mi restaurante');
    })();
  </script>
```
![alt text](https://github.com/esteban-vera/linkRappi/blob/master/images/button-radius.png?raw=true)

4. Con bordes redondeados y sombra:

```
  <script>
    (function() {
      addLinkRappi('radius shadow', 'mi restaurante');
    })();
  </script>
```
![alt text](https://github.com/esteban-vera/linkRappi/blob/master/images/button-radius-shadow.png?raw=true)

5. Con fondo blanco:

```
  <script>
    (function() {
      addLinkRappi('white', 'mi restaurante');
    })();
  </script>
```
![alt text](https://github.com/esteban-vera/linkRappi/blob/master/images/button-white.png?raw=true)


6. Con fondo naranja:

```
  <script>
    (function() {
      addLinkRappi('red', 'mi restaurante');
    })();
  </script>
```
![alt text](https://github.com/esteban-vera/linkRappi/blob/master/images/button-red.png?raw=true)


Si desea el boton mas grande agregar la palabra 'big', ejemplo: 

```
  <script>
    (function() {
      addLinkRappi('radius shadow big', 'mi restaurante');
    })();
  </script>
