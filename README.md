# Gustos

Unos amigos se están por abrir un bilichito y nos pidieron un sistema para determinar qué cosas le gustan a las personas. Toda la documentación se encuentra en [este documento](doc/objetosGustos.md).

Por suerte para nosotros, alguien ya implementó lo pedido. Pero nos dieron la tarea de revisar su trabajo.

## Code Review

Revisar que lo que esté hecho funciona correctamente. Para ello se cuenta con algunos tests que prueban la funcionalidad de algunos objetos. Correrlos y ver que todo esté correcto y sin errores.

**En el caso de encontrar errores deberán arreglarlos** teniendo la documentación otorgada como _fuente de la verdad_.

## Más cosas

Agregar al modelo estos objetos:

- un _arito_ celeste de cobre, que pesa 180 gramos.
- un _banquito_ de madera que pesa 1700 gramos. 
  Al principio es naranja, pero puede cambiar de color. 
  El naranja es un color fuerte.
- una _cajita_ roja, que tiene un objeto adentro. Puede ser de cualquier material. 
  Este objeto puede ser cualquiera de los definidos previamente, y puede cambiar.
  El peso de la cajita es de 400 gramos más el peso de lo que tiene adentro.
    
Y tener tests que prueben los siguientes casos:
- Un bolichito con un banquito en mostrador y una cajita de cobre con una pelota dentro en vidriera no está desequilibrado y tiene algo naranja.
- El caso anterior pero si en vez de la pelota hay un arito dentro de la cajita, entonces sí está desequilibrado.
- El caso anterior pero si se le cambia el color del banquito por verde, entonces deja de tener algo naranja.


## Se hizo la luz

- Ahora también queremos saber si **el bolichito tiene luz** que se cumple cuando alguno de los dos objetos está hecho de un material que conduce la electricidad. De los amteriales que tenemos por ahora, solo el cobre conduce la electricidad.

- Agregar como material al plomo que puede estar en uno de sus tres estados: _natural_, _cromado_ u _oxidado_.
  - Cuando está al natural, el material brilla pero no conduce la electricidad.
  - Cuando está cromado, el material brilla y conduce la electricidad.
  - Cuando está oxidado, el material no brilla ni conduce la electricidad.
  El material comienza al natural pero puede ser cromado u oxidado cuando se desee.

- Testear los siguientes casos de prueba:
  - Un bolichito con un muñeco de 500 gramos en mostrador y una cajita de plomo con un arito dentro es brillante pero no tiene luz.
  - La misma situación pero con una cajita de plomo cromado, entonces el bolichito es brillante y tiene luz.
  - La misma situación pero con una cajita de plomo oxidado, entonces el bolichito no es brillante ni tiene luz.
