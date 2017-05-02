# linkRappi

Para añadir el link de rappi a tu página web debes seguir estos pasos:

1. Crear un div con un id llamado 'linkRappi' donde quieras que aparezca el link.

```
<div id="linkRappi"></div>
```

2. Agregar este script antes de finalizar el 'body':

```
<script src="http://amp-ejemplo-tomalo.epizy.com/linkRappi.min.js"></script>
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

* Url donde va direccionar, tener en cuenta que si se ingresa un nombre con espacios se reemplazara con guiones(-),
  ejemplo: 'mi restaurante' = mi-restaurante



## Ejemplo con configuración

```
  <script>
    (function() {
      addLinkRappi('radius shadow big', 'mi restaurante');
    })();
  </script>
```
