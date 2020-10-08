# Arquitecturas software para la nube

## Ejercicio 1
## Buscar una aplicación de ejemplo, preferiblemente propia, y deducir qué patrón es el que usa. ¿Qué habría que hacer para evolucionar a un patrón tipo microservicios?

Como ejemplo, voy a usar mi propia pagina web personal, la cual esta alojada en este [enlace](https://www.roldanzafra.com). La página es un tipo de portfolio/curriculum virtual y en la cual se pueden añadir post, proyectos y diferentes secciones instalables a través de plugins. Esta aplicación presenta una arquitectura de microkernel ya que todos estos plugins se ejecutan sobre un núcleo central.

Para evolucionar este tipo de aplicación a un patron de microservicios se podrían desarrollar las paginas en html/css/php y dividir las funcionalidades en diferentes microservicios. Ejemplos de estos microservicios podrían ser el login, la base de datos que almacena las paginas o los datos de los usuarios (en el caso de mi pagina personal mis datos, aunque también se podrían desarrollar varios perfiles de forma similar).

## En la aplicación que se ha usado como ejemplo en el ejercicio anterior, ¿podría usar diferentes lenguajes? ¿Qué almacenes de datos serían los más convenientes?

Si, se podrían utilizar lenguajes diferentes a los que se utilizan, actualmente la pagina esta escrita en go y javascript y se podría utilizar php html y css.
En cuanto a los almacenes de datos, dado que las diferentes secciones del sitio web se organizan en paginas seria interesante un almacén de datos de tipo documental y noSQL como mongodb, por ejemplo.
