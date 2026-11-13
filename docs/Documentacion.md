```
    @author: 
    @version:
    @date: 
```
# Sistema Gestor de Rutas Turísticas y Conexiones de Transporte para Tegucigalpa

## Análisis de Proyecto

La pagina está dirigida por un presidente de transporte que se dedica a analizar adecuadamente las rutas turísticas y de transporte, y generar horarios alternos evitando colisiones entre dos o más rutas. 

Este proyecto se basa en el diseño de 4 horarios turísticos en la ciudad de Tegucigalpa, donde cada uno de los horarios consta de la **ruta de transporte, los destinos y el tipo de transporte**, elementos los cuales son afectados por los horarios de salida, tiempo de visita, guías turísticos, estaciones terminales, líneas de transporte, etc.

En la página web se mostrará toda la información sobre los horarios, rutas, destinos y demás elementos que existe en la base de conocimiento, así como estadísticas que se crearás en base a las reglas de los hechos. Esta información será mostrada por **Java Script**, que sería el **FrontEnd** de nuestro sistema, con el uso de módulos como el *DOM*, *Cambios de tema*, *creación de tablas* y demás elementos vistos en la clase impartida por el Ingeniero José Inestroza. 

La información de los módulos y de los demás archivos de Java Script será extraída de las APIs escritas en el lenguaje de programación, PHP. Las APIs contendrán los componentes PHP en el FrontEnd que hablaran con los componentes PHP en el BackEnd. Estos elementos del BackEnd harán la conexión con la base de conocimiento. 

## Servicios

El sistema debe ser capaz de:
- \[PL] Generar horarios de acuerdo a los hechos de la base de conocimiento. 
- \[PL] Mostrar estadísticas relacionadas con los hechos.
- \[PL] Mostrar las 4 rutas turísticas alternativas.
	- Generando reglas, así como vimos en la clase impartida por el Ingeniero José Inestroza (aplica para los tres servicios anteriores).
- \[JS] Mostrar toda la información de la base de conocimiento.
	- PL -> PY -> PHP -> JS.
- \[JS] Botón de **Acerca de** (muestra la documentación explicativa de cada función).
	- Generar una ventana modal con los módulos de Java Script, así como vimos en la clase impartida por el Ingeniero José Inestroza. 
- \[PH] Botón de **Borrar** (genera un archivo con toda la información de la base de conocimiento)
	- Renombrar el archivo con el formato dado en la documentación de proyecto o crear el archivo y copiar toda la información antes de borrarlo.
- \[JS] Manejar un cambio de tema por medio de un JSON.

## Prolog

*En prolog vamos a crear la base de conocimientos que nos permita generar los horarios turísticos, mediante los hechos y reglas que nos permite el lenguaje de programación.*

### Hechos de la base de conocimiento

- turista (nombre)
- grupo de turista

- Horario
	- Destino1
	- Destino 2
	- Destino 3
	- Hora de salida (hora)
	- Guía turístico (nombre)
	- Línea de transporte (Carrizal, Cerro Grande, La Sosa, …).
	- Tipo de transporte (bus, taxi, carro alquilado, taxi vip, …).
	- Estaciones terminales (Terminales de buses, puntos de taxis, puntos de alquiler de automóviles, calle).
	- Perfil de turista (tipo, nombre).
	- turista(nombre)

- Destino 
	- Tiempo límite de visita (50 minutos)
	- Numero máximo de turistas (número)
	- Nombre del destino (nombre)
	- Tipo de destino (montañoso, urbano, rural, selvático)

- Ruta 
	- Lugar de partida
	- Destino1
	- Destino 2
	- Destino 3
	- distancia


%%## Actores 

- Rutas de transporte
- Destinos (con su numero máximo de turistas)
- Tipos de transporte

**Fijos**
- Horarios de salida
- Tiempo de visita
- Guías turísticos
- Estaciones terminales
- Líneas de transporte

*Van a ser varios turistas (15) que se moverán entre destinos según sus horarios respectivos y en cada destino se armarán grupos, siempre menores al numero máximo de turistas permitidos.*
%%

