# Hoja de Ruta de The Native Pond

![flatbreadlist_background](/background/es/FBL-docs-bg-es.png)

> [!WARNING]
> 1. Todo el contenido de esta lista son castillos en el aire — no representa la presentación final ni la implementación real.
> 2. Parte del contenido de esta lista no se ha debatido en las reuniones del equipo de desarrollo.
> 3. Parte del contenido de esta lista no ha pasado por un estudio de viabilidad.
> 4. Esta lista puede servir de guía orientativa para creaciones secundarias y obras derivadas.
> 5. El equipo de desarrollo se reserva todos los derechos para tomar medidas posteriores sobre esta lista, así como la interpretación final de la misma.

---

## 🎮 Sistema de control

Un movimiento fluido y una buena cámara son fundamentales para que el juego tenga jugabilidad. **¡El personaje tiene que poder moverse!**

### 🚶 Formas de moverse

- El jugador controla al personaje para moverse por el **mapa** y, en lugares especiales (como la plataforma de pesca), al pulsar una tecla o al llegar a un pequeño rango de coordenadas del lugar especial, se **activa** la animación de entrada en ese **lugar especial**.
- El jugador **interactúa** con el juego mediante botones táctiles (móvil), teclado (escritorio) y mando, y las teclas se pueden personalizar.

### 🎥 Cámara

- En las zonas no especiales del mapa se usa una vista en **tercera persona**.
- En las zonas especiales del mapa (como la plataforma de pesca) se usa una vista en **primera persona**, mostrando el interior de esa zona especial (si lo tiene).
- El mapa se **mueve** siguiendo la cámara.

---

## 🗺️ Sistema de mapa

¡Siéntate a hacer un **mapa** sobre la mesa, que en el mapa hay de todo!

### 🧭 Zoom y orientación

- El mapa no **gira** con la cámara.
- El mapa se puede **ampliar y reducir**.
- El mapa sigue la lógica de "**norte arriba, sur abajo, oeste a la izquierda, este a la derecha**".

### 🚧 Límites

- El mapa del juego tiene **límites**, es decir, el jugador no puede atravesar el **borde del mapa**.
- Cuando el jugador intenta cruzar el límite, el juego le **arrastra de vuelta** y muestra el mensaje "* Una sensación familiar te invade — parece que oyes: '¡Exploremos la zona de delante más tarde!' Aunque sabes que nunca podrás explorarla, aun así quieres intentarlo."
- Los límites pueden ser **obstáculos naturales** evidentes (como montañas grandes) o **vallas artificiales** (como los muros de la arquitectura estilo Huizhou).

### ⛅ Clima

- Los **tipos** de clima son los siguientes:
	- Soleado.
	- Lluvia.
	- Tormenta.
	- Nieve.
- El **cambio** de clima puede decidirse según:
	1. El ajuste manual del jugador.
	2. La similitud con las características climáticas de una determinada región.
	3. Una probabilidad completamente aleatoria.

### 🍂 Estaciones

- Las estaciones cambian cada **90 horas**.
- Los **tipos** de estación son los siguientes:
	- Primavera.
	- Verano.
	- Otoño.
	- Invierno.

### 📷 Cámara de fotos

- El jugador puede **hacer fotos** en cualquier lugar (excepto en las interfaces de la GUI) pulsando una tecla, haciendo clic en un botón o pulsando un botón del mando.
- Al **hacer una foto**, el juego mostrará un **destello blanco** a pantalla completa para representar la foto. Puede ser necesario añadir una pantalla de aviso de **epilepsia fotosensible** en la pantalla de inicio del juego.
- Al **hacer una foto**, el juego **captura** automáticamente todos los elementos de la pantalla (excepto los elementos de la GUI) y les añade un **marco**.
- El juego **guardará** las fotos en una **carpeta específica** para poder compartirlas.

### 🌍 Biomas

- La mayoría de los elementos del mapa se distribuyen en distintos **biomas**.
- Hay los siguientes biomas:
	- Llanuras
	- Selva
	- Playa
	- Tierras de cultivo
	- Campos de flores
	- Estanque
	- Arroyos
	- Aldea

### 🐟 El estanque de pesca

- El estanque de pesca es la zona especial más importante del juego, e incluye la **plataforma de pesca**, el **estanque** y la **barca**.

#### Plataforma de pesca

- Está en el extremo más al **sur** del estanque, en el bioma de playa.
- Cuando el jugador **entra** en esta zona especial, la cámara se acerca automáticamente y cambia a la vista en primera persona, el personaje se sienta y se muestra la interfaz visual de esa zona especial.
- La plataforma de pesca sirve para **pescar**.

#### Estanque

- Está en el extremo más al **norte** del mapa, en el bioma del estanque.
- Cuando el jugador **entra** en esta zona especial, el personaje pasa a estar en estado de **natación**.

#### Barca

- Puede estar en **cualquier lugar** del estanque (dependerá de dónde la dejara aparcada el jugador la última vez).
- Cuando el jugador **entra** en esta zona especial, el personaje pasa a estar en estado de **conducción** y se muestra la interfaz visual de esa zona especial.
- El jugador puede conducir la barca para navegar por el **estanque**.

### ⛺ Tienda

- Está al **suroeste**, más o menos en el centro del mapa, en el bioma de llanuras.
- Cuando el jugador **entra** en esta zona especial, la cámara se acerca automáticamente y cambia a la vista en primera persona, mostrando la interfaz visual de esa zona especial.
- La tienda es el corazón del **campamento**.
- El **interior** y el **tamaño** de la tienda pueden inspirarse en el diseño de la tienda de *Robinson Crusoe*.

### 🌾 Campo

- El campo está al **sureste** de la tienda, en el bioma de tierras de cultivo.
- Cuando el jugador **entra** en esta zona especial, la cámara se acerca automáticamente y cambia a la vista en primera persona, mostrando la interfaz visual de esa zona especial.
- El campo sirve para **cultivar**.

### 🏪 Mercado

- El mercado está en la parte **sur** del mapa, en el bioma de la aldea.
- Cuando el jugador **entra** en esta zona especial, la cámara se acerca automáticamente y cambia a la vista en primera persona, mostrando la interfaz visual de esa zona especial.
- El mercado sirve para **comerciar**.

### 🌳 Árbol antiguo

- Está al **sureste** de la tienda, en el bioma de llanuras.
- Cuando el jugador **entra** en esta zona especial, la cámara se acerca automáticamente y cambia a la vista en primera persona, y el personaje se sienta.
- En el árbol antiguo a veces (por ejemplo en otoño) aparecen **manzanas**. El jugador puede derribarlas con un **palo largo** y **recogerlas**.
- Cuando el jugador permanece un rato bajo el **árbol antiguo** (unos 1 minutos), el juego muestra un botón flotante "Mantén [W] para meditar"; al pulsar W, hacer clic en el botón o pulsar un botón del mando, se entra en **meditación**. Mientras el jugador **medita**, el juego muestra **efectos visuales** a pantalla completa (varias fórmulas físicas) y hay probabilidad de que le golpee una **manzana**.
- El árbol antiguo puede florecer con **flores antiguas** (nombre provisional); las flores antiguas caen flotando de las ramas. El jugador puede recoger una flor antigua y **chupar el néctar**, con un 50 % de probabilidad de obtener un **néctar dulcísimo**.

### 🔥 Hoguera

- Está a poca distancia al **este** de la tienda, en el bioma de llanuras.
- Cuando el jugador **entra** en esta zona especial, la cámara se acerca automáticamente y cambia a la vista en primera persona, mostrando la interfaz visual de esa zona especial.
- La hoguera puede **encenderse** y proporcionar luz.
- La hoguera sirve para **cocinar**.

### 📮 Buzón

- Está al **sur** de la tienda, en el bioma de la aldea.
- Cuando el jugador **entra** en esta zona especial, la cámara se acerca automáticamente y cambia a la vista en primera persona, mostrando la interfaz visual de esa zona especial.
- El buzón sirve para **enviar y recibir correo**.

### 🐚 Caracola mágica

- El jugador puede recoger la **caracola mágica** en la **playa** junto al agua.
- Cuando el jugador **recoge** la caracola mágica, el personaje pasa a estar en estado de tocar la caracola y la cámara se acerca automáticamente. El jugador no puede moverse. Al mismo tiempo se muestra la interfaz visual de ese objeto especial.
- La caracola mágica tiene 7 **tonos** que el jugador puede tocar.
- La caracola mágica tiene varias **variantes**, y cada variante tiene un **timbre** distinto.

### 🍄 Setas

- Las setas se encuentran en el bioma de la **selva** y se dividen en **setas venenosas** y **setas no venenosas**.
- Las setas se reproducen con el clima de **lluvia** y **tormenta**.
- El jugador puede dar palmaditas a las setas para ayudar a que se reproduzcan; cada seta solo puede ayudar a la reproducción una vez, pero se le pueden dar palmaditas todas las veces que se quiera.
- Cuando el jugador interactúa con una seta (dándole palmaditas), la seta emite un **efecto de sonido** agradable; cada seta tiene un tono distinto.
- El jugador puede **mover de sitio** las setas.
- Mediante combinaciones y disposiciones, el jugador puede fabricar **instrumentos** con las setas.

### ✨ Luciérnagas

- Las luciérnagas aparecen durante la **noche** en el bioma de la selva.
- Las luciérnagas brillan por sí solas y vuelan aleatoriamente por el bioma de la selva y los biomas cercanos.
- El jugador puede meter luciérnagas en una **botella a la deriva** para que le proporcionen luz.
- La luz de la botella de luciérnagas solo dura 3 días.

---

## 🎣 Sistema de pesca

En la **plataforma de pesca**, el jugador puede pescar con la **caña**.

### 🐠 Especies

- El **estanque de pesca** del juego permite pescar tanto **especies marinas** como **especies de agua dulce**. Además de peces, también se pueden pescar **coleccionables**.
	1. Puede decidirse según la **plataforma de pesca** que elija el jugador (por ejemplo, una plataforma junto al mar solo permite pescar especies marinas, y una plataforma junto a un lago solo especies de agua dulce).
	2. Puede decidirse según la **probabilidad** de cada especie (es decir, en la misma plataforma junto al mar se pueden pescar a la vez especies marinas y de agua dulce según la probabilidad).
- La **probabilidad** de pescar cada especie depende de:
	1. La probabilidad real de pescar cada especie. Puede ser un rango de valores que se ajusta según varios factores (como el clima o la estación), y no es fijo.
	2. Una probabilidad completamente **aleatoria**.
- La **probabilidad** de pescar coleccionables depende de:
	1. La **tasa de mordida** histórica del jugador.
	2. Una **probabilidad** aleatoria dentro de un rango fijo.
	3. Una probabilidad completamente **aleatoria**.

### 🎯 Tasa de mordida

Cabe señalar que la tasa de mordida se refiere a la probabilidad de que el pez **muerda el anzuelo**, no a la probabilidad de acabar pescándolo.

- La **tasa de mordida** del juego se decide en conjunto según los siguientes factores:
	- Si el anzuelo del jugador tiene cebo o no.
	- Si el jugador ha cebado el puesto de pesca o no.
	- El tipo de cebo del anzuelo.
	- La hora del juego (por ejemplo, de día o de noche).
	- Si la lámpara frontal está encendida de noche.
	- El clima del juego.
	- La estación del juego.
- La tasa de mordida del juego también puede decidirse según:
	1. La tasa de mordida histórica del jugador.
	2. Una probabilidad completamente aleatoria.

### 🪝 Tasa de captura

Como su nombre indica, la tasa de captura se refiere a la probabilidad de acabar pescando el pez.

- La **tasa de captura** del juego se decide en conjunto según los siguientes factores:
	- Si el pez ha mordido el anzuelo.
	- El momento en que el jugador levanta la caña (ni demasiado pronto ni demasiado tarde).
	- La tasa de rotura del sedal.
	- El tamaño del anzuelo.

### 🎣 La caña

- La caña se compone de la **vara**, el **flotador**, el **anzuelo** y el **sedal**.
- Todas las partes de la caña tienen **durabilidad**; cuanto menor es la durabilidad, mayor es la probabilidad de que la caña se estropee. Cuando la caña se estropea, hay que **reemplazar** la parte dañada.

#### Vara

- La **vara** es una parte de la **caña**.
- El jugador puede comprar varas con el **sistema de comercio**, por ejemplo varas de 2,7 metros y de 3,6 metros.
- Las varas de distinta longitud tienen tiempos de lanzamiento y de levante distintos.

#### Flotador

- El **flotador** es una parte de la **caña**; el jugador puede decidir si levanta la caña según el **movimiento del flotador**.
- El jugador puede comprar flotadores con el **sistema de comercio**, por ejemplo flotadores normales y flotadores luminosos.
- El movimiento del flotador al morder el anzuelo es distinto para cada especie, tomando como referencia el movimiento real del flotador cuando los peces muerden el anzuelo.
- El flotador se puede **ajustar en "puntos"** (es decir, ajustando el peso del plomo) para facilitar la observación.

#### Anzuelo

- El **anzuelo** es una parte de la **caña** y la base para pescar.
- El jugador puede comprar anzuelos con el **sistema de comercio**, por ejemplo anzuelos pequeños y anzuelos grandes.
- El tamaño del anzuelo es el factor decisivo para pescar peces grandes o pequeños.
- Al anzuelo se le puede poner **cebo**.

#### Sedal

- El **sedal** es una parte de la **caña**.
- El jugador puede comprar sedales con el **sistema de comercio**, por ejemplo sedales normales del 0.8 y sedales de calidad del 2.0.
- Los distintos sedales tienen una **tasa de rotura** distinta, que puede decidirse según estos factores:
	- La calidad del sedal.
	- El tiempo de uso o la durabilidad del sedal.

### 🪱 Cebo

- El jugador puede comprar cebo con el **sistema de comercio**, por ejemplo cebo normal y lombrices rojas.
- Si compra cebo en polvo, antes habrá que prepararlo mezclándolo con agua y amasándolo para obtener el cebo.
- Los distintos cebos tienen una **tasa de mordida** distinta.
- Como consumible, cuando el jugador se queda sin cebo y no tiene suficientes conchas (incluidas las obtenidas al vender la pesca) para comprar un paquete, el juego repondrá cebo gratis en el **buzón** al día siguiente.

### 🥣 Cebado

- El jugador puede comprar cebado con el **sistema de comercio**, por ejemplo bagazo de soja fermentado y maíz viejo macerado en vino.
- Los distintos cebados tienen una **tasa de mordida** distinta.
- El cebado puede aumentar muchísimo la tasa de mordida.

### 🔦 Lámpara frontal

- El jugador puede comprar lámparas frontales con el **sistema de comercio**, por ejemplo una lámpara normal y una lámpara de luz azul para pescar de noche.
- Las distintas lámparas frontales tienen una **tasa de mordida** distinta y efectos visuales distintos.
- De noche, la lámpara frontal permite ver la superficie del agua y el flotador.
- De noche, la lámpara frontal puede asustar a los peces y hacer bajar la tasa de mordida.

### 🏺 Coleccionables

- Los coleccionables se dividen principalmente en **botellas a la deriva**, **recuerdos** y **fragmentos de historia**.
- El jugador puede **obtener** coleccionables de las siguientes formas:
	- Pescar.
	- Regalos de Cat.

#### Botella a la deriva

- Las botellas a la deriva contienen **papeles de carta**.
- La mayoría de los papeles de carta son **mensajes reconfortantes** para animar al jugador.

#### Recuerdos

- Algunos recuerdos se pueden **colocar** en la **tienda**.

#### Fragmentos de historia

- Los fragmentos de historia sirven para guiar al jugador y que conozca las historias de los **aldeanos**.
- Cuando se han recogido todos los fragmentos de historia, el jugador puede desbloquear una historia larga para conocer completa y detalladamente las historias de los **aldeanos**.

---

## 🍳 Sistema de cocina

¡Prepara **comida** y prueba a comértela!

### 🍳 Utensilios de cocina

- Los utensilios de cocina se componen de tres partes: el **fogón**, la **tabla de cortar** y los **utensilios culinarios**.

#### Fogón

- El fogón sirve para **calentar** la comida.
- El fogón puede **estar**:
	1. Dentro de la tienda.
	2. Fuera de la tienda, pero cerca de ella.
- El fogón permite colocar algunos **utensilios culinarios** (como la sartén).
- Antes de usar el fogón hay que añadirle **combustible**.
- El jugador debe **controlar el fuego** para asegurarse de que la comida preparada sea comestible.

#### Tabla de cortar

- La tabla de cortar sirve para **trocear** la comida.
- La tabla de cortar permite colocar algunos **ingredientes** (como la col china) y **alimentos semielaborados**.
- El jugador puede usar algunos **utensilios culinarios** (como el cuchillo) para cortar sobre la tabla.

#### Utensilios culinarios

- Los utensilios culinarios permiten **manipular** los ingredientes con comodidad.
- Los utensilios culinarios incluyen:
	- La olla grande.
	- La sartén.
	- La vaporera.
	- El cuenco de porcelana.
	- El cuchillo.
	- El rodillo.

### 📜 Recetas

- El jugador puede preparar comida siguiendo las **recetas**. En general, si se sigue la receta, la comida sale bien.
- El jugador también puede **no seguir** la receta y dejarse llevar.

### 🍲 Alimentos

- Cuando el jugador completa todo el **proceso de elaboración de un alimento**, obtiene ese **alimento**.
- El jugador puede preparar los siguientes alimentos:
	- Fideos simples (obtenidos en todo el proceso: de la harina, el amasado, cortar las tiras y hervirlas).
	- Bollos al vapor (obtenidos en todo el proceso: de la harina, el amasado, estirar la masa, preparar el relleno, dar forma y cocerlos al vapor).
	- Huevo frito (obtenido en todo el proceso: cascar el huevo, encender el fuego y darle la vuelta).
	- Pescado a la brasa (obtenido asándolo en la hoguera).
	- Objeto indescriptible (obtenido al fracasar en la preparación de comida).
	- Carbón (obtenido al fracasar preparando comida sin seguir la receta).

### 🍽️ Comer

- Cuando el jugador ha **preparado** un alimento, puede probar a comérselo.
- Al comer, el jugador puede hacer clic en el **alimento** o en las **partes del alimento** para comerlas.
- Cuando el jugador come un **alimento**, sonará un **efecto de sonido** agradable, aparecerá un **texto** reconfortante y el alimento o sus partes **desaparecerán** con una animación para representar que se ha comido.
- En particular, cuando el jugador come un **objeto indescriptible**, hay probabilidad de que ocurra alguna de estas cosas:
	1. El personaje se desmaya y despierta al cabo de un rato.
	2. El personaje tiene náuseas visuales durante un rato.
	3. No ocurre nada.

---

## ⛺️ Sistema de campamento

¡Solo la **tienda** da sensación de seguridad!

### 📦 Almacenamiento

- En la **tienda**, el jugador puede ver los **objetos** que posee.
- Los objetos que **posee** el jugador incluyen:
	- Peces.
	- Coleccionables.
	- Utensilios de pesca.
	- Cultivos.
- Algunos objetos (como algunos coleccionables) se pueden **colocar**.

### 🏆 Logros

- El jugador puede desbloquear logros **cumpliendo** ciertas **condiciones**.
- Los logros no dan al jugador **recompensas materiales**, pero hay un **sonido al completarlos** que elogia al jugador.
- Los logros pueden ser ocultos; los logros ocultos no se pueden ver en la página de logros antes de completarlos.
- En la **tienda**, el jugador puede ver los **logros** obtenidos.

### 📍 Hitos

- El jugador puede desbloquear hitos **haciendo clic** en la página de hitos.
- Los hitos no tienen nada que ver con el juego; existen para que las experiencias del jugador en el **mundo real** encuentren su reflejo en el juego.
- Los hitos se pueden alcanzar sin ninguna condición **dentro del juego**.
- Desbloquear hitos depende de la **credibilidad** del propio jugador; solo los hitos realmente cumplidos en el mundo real tienen sentido.

### 🛏️ Cama

- Al **atardecer** y **de noche**, el jugador puede hacer clic en la cama para **dormir** y saltarse la noche.
- El jugador se despertará con la **salida del sol** o por la **mañana** del día siguiente; también puede elegir **seguir durmiendo un poco**.

### 🗑️ Contenedor de reciclaje de emociones

- Este contenedor, parecido a un cubo de reciclaje, permite al jugador escribir las cosas desagradables que le han pasado en la **vida real**, hacer una bola con el papel y ¡tirarla al contenedor de reciclaje de emociones!

### 📓 Diario

- El jugador puede escribir en el **diario** las cosas que le ocurren cada día (tanto del juego como de la vida real).
- El diario debe admitir formato de texto enriquecido (sintaxis Markdown) y poder mostrar imágenes.
- Las imágenes que se muestran en el diario solo pueden provenir de los **dibujos** y las **capturas de pantalla del juego** del jugador.
- El juego permite **exportar** páginas concretas del **diario** a una **carpeta específica** para poder compartirlas.
- El papel del diario se puede **arrancar** y tirar al **contenedor de reciclaje de emociones**.

### 🖼️ Álbum

- El álbum mostrará todas las **obras** que el jugador ha dibujado en el **papel de dibujo**.
- El álbum se puede exportar entero como un único archivo a una **carpeta específica** para poder compartirlo.

---

## 🐚 Sistema de comercio

¿Está madura esta sandía?

### 🛒 Comprar

- El jugador puede comprar productos en el **mercado**.
- En el mercado, el jugador puede hablar con los **aldeanos** de distintas profesiones.
- Al **hablar** con un aldeano, hay probabilidad de **desencadenar una misión especial**; al completarla, se obtiene un **descuento**.
- El jugador puede comprar en el mercado los siguientes **tipos** de productos:
	- Utensilios de pesca (como cañas).
	- Semillas de cultivos (como semillas de trigo).
	- Cultivos procesados (como harina).
	- Verduras (como col china).
	- Combustible (como carbón).
	- Condimentos (como sal).
	- Papel de dibujo (como papel 1:1).
	- Sellos.

### 💰 Vender

- El jugador puede vender productos en el **mercado**.
- El jugador puede vender en el mercado los siguientes **tipos** de productos:
	- Peces.
	- Algunos coleccionables.
- Al vender peces, el precio seguirá el **precio del día**.
- El **precio del día** tiene dos modalidades: **pescado fresco** y **pescado en stock**; ningún precio es fijo, y el precio del día puede decidirse según estos factores:
	- El clima del juego.
	- La estación del juego.
	- Un valor aleatorio dentro de un rango fijo.

### 🪙 Moneda

- El juego usa **conchas** como moneda.
- El jugador puede **obtener** conchas de las siguientes formas:
	- Comerciando.
	- Pesándolas.
	- Regalos de Cat.

---

## 🌽 Sistema de cultivos

**Planta cultivos**, **riega y abona**, y **cosecha**.

### 🌱 Plantar

- Para plantar cultivos es necesario tener **semillas de cultivos**.
- El **proceso** de plantación es el siguiente: allanar la tierra, sembrar las semillas, cubrirlas con tierra, regar y abonar.
- Condiciones para que germinen las semillas: **la humedad adecuada**, **la temperatura adecuada** y **el oxígeno suficiente**.
- Al plantar, el jugador debe **tener en cuenta**:
	- El clima del juego.
	- La estación del juego.

### 🌿 Crecimiento

- Durante el crecimiento de los cultivos, el jugador debe mantener el **riego** y el **abonado** sin interrupciones.
- Los cultivos **cambian** de **estado de crecimiento** cada cierto tiempo (unas 90 horas aproximadamente).

### 🧺 Cosecha

- Cuando los cultivos están **completamente maduros**, el jugador puede cosechar los **cultivos** y las **semillas**.

---

## 🐱 CatGPT

**Charla** con el gatito o **acarícialo** ฅ՞•ﻌ•՞ฅ.

### 💬 Chatear

- El jugador puede **enviar mensajes** a Cat.
- Cat **responderá** al jugador según ciertos pesos, que pueden decidirse según:
	1. El número de caracteres que envía el jugador.
	2. Una probabilidad completamente aleatoria.
- Cat responderá "**Meow**" con varios tonos y timbres para aportar valor emocional al jugador.

### 🐾 Acariciar

- El jugador puede acariciar a Cat tocándole la **cabeza**.
- Al acariciarlo, saldrán de Cat mensajes flotantes con la palabra "**Meow**", acompañados de "**Meow**" en varios tonos y timbres para aportar valor emocional al jugador.

### 🎁 Regalos

- Cat puede dar un **regalo** al jugador cuando este se despierta a la mañana siguiente.
- Si Cat da o no un **regalo** puede decidirse según:
	1. Las veces que el jugador habló con Cat o lo acarició ayer.
	2. Las veces que el jugador ha hablado con Cat o lo ha acariciado en total.
	3. Una probabilidad completamente aleatoria.
- Los **tipos** de regalos pueden incluir:
	- Peces.
	- Conchas.
	- Algunos coleccionables (probabilidad muy baja).

### ❓ Y también puede ser...

- Además de Cat, el jugador puede elegir **otros objetos** con los que hablar o a los que acariciar. Estos **otros objetos** pueden ser **miembros del equipo de desarrollo** que aparecen en la **historia introductoria**.

---

## 🖌️ Sistema de dibujo

**Dibuja** con papel y pinturas de lo más reales, y guarda tu obra.

### 📄 Papel de dibujo

- El papel de dibujo es igual que el papel real: permite **difuminar**, **volver a colorear** y **mezclar colores**.
- El jugador puede comprar papel de dibujo con el **sistema de comercio**, por ejemplo papel 1:1 y papel 3:4.

### 🎨 Paleta de colores

- Por defecto se ofrecen 8 colores básicos; el jugador puede mojar el **pincel** en la pintura y mezclar colores en la **paleta**.
- La técnica de mezcla puede ser **acuarela** o **gouache**.
- Al mezclar, las pinturas de dos colores se combinan con el **pincel**; la pintura no mezclada conserva su color original, y el color mezclado depende del grado de mezcla del jugador.

### 🖌️ Pincel

- El pincel sirve para **aplicar** pintura o agua sobre el papel de dibujo.

### 💾 Guardar

- Los dibujos del jugador se **guardarán** en el **diario**.
- El jugador puede **exportar** sus obras a una **carpeta específica** para poder compartirlas.

---

## 📬 Sistema de buzón

Enviar y recibir **correo**.

### 📥 Recibir

- El jugador puede **recibir** los siguientes correos:
	- Cartas que se ha enviado a sí mismo.
	- Reposición gratuita de cebo.
	- Felicitaciones de festividades.
	- Felicitaciones de cumpleaños.

### 📤 Enviar

- El jugador puede **enviar** los siguientes correos:
	- Cartas para su yo del futuro.
- Al enviar, el correo debe llevar **sello**.

---

## 🧩 Extender el juego

Una forma importante de mejorar la jugabilidad es extender el juego con contenido nuevo, por ejemplo **haciendo MODs** y **haciendo paquetes de recursos**.

### 🔧 Sistema de MODs

- Desde su diseño inicial, el juego admite la importación de **paquetes de MOD de terceros** para enriquecer el contenido del juego.
- Los MODs deben poder añadir/modificar/eliminar lo siguiente:
	- Biomas
	- Flujo de tiempo
	- Objetos
	- Logros
	- Hitos
	- Tipos de comercio
	- Métodos de cultivo
	- Interfaces de GUI (incluidos los controles)
	- Texto
	- Texturas
	- Audio
- El juego debe ofrecer casi todas las **interfaces** disponibles y la documentación de soporte correspondiente, así como diseñar un conjunto de **normas**; por ejemplo, ciertos componentes deben invocarse con un método concreto.
- El juego **no debe** admitir paquetes de MOD que no sigan las normas.
- No se restringe el contenido de los paquetes de MOD, sin importar si viola los valores.
- El juego debe ofrecer una **página** específica para ayudar al jugador a activar o configurar los paquetes de MOD.

### 🗂️ Paquetes de recursos

- Los paquetes de recursos pueden modificar el **texto**, las **texturas** y el **audio** del juego.
- Los paquetes de recursos no ofrecen, ni se **les permite** ofrecer, funciones nuevas al juego.
- El juego debe ofrecer una **página** específica para ayudar al jugador a activar o configurar los paquetes de recursos.

---

## 📺 Interfaz visual

Una **animación no lineal** fluida siempre da al jugador una buena experiencia visual.

### 🎛️ Controles

- Los controles pueden **activar** comportamientos y eventos de interacción.
- Los controles deben mantener el mismo estilo de diseño que *Today@PolarBay*.
- Al **pulsar** un control, debe encogerse al instante tomando el centro de la interfaz como centro de escala, y luego rebotar de forma no lineal.
- Los controles pueden **posicionarse** y **redimensionarse** a gusto.

### 🃏 Tarjetas

- Las tarjetas no son **interactivas**.
- Las tarjetas deben mantener el mismo estilo de diseño que *Today@PolarBay*.
- Las tarjetas sirven para mostrar fondos relativamente **limpios**, como la interfaz de la mochila.

### 🟢 Pantalla verde protectora de ojos

- Como el jugador debe **mirar fijamente** el **flotador** durante **mucho tiempo** al **pescar**, se ha diseñado especialmente una **pantalla verde protectora de ojos**.
- La pantalla verde protectora de ojos **cubre la pantalla** de vez en cuando para obligar al jugador a **descansar**.
- El **intervalo** y la **duración** de la pantalla verde protectora de ojos se pueden ajustar o desactivar en los ajustes.
- La pantalla verde protectora de ojos mostrará el contenido de los **papeles de carta** de las **botellas a la deriva** que el jugador haya recogido.

### 🌗 Esquemas de color

- El juego puede incluir **dos esquemas** de color: el tema blanco y el tema negro.
- El tema blanco y el tema negro pueden **alternarse** según las siguientes condiciones:
	1. El ciclo de día y noche de la vida real.
	2. El ciclo de día y noche del juego.
	3. El ajuste manual del jugador en la pantalla de ajustes.

### 🎆 Efectos de partículas

- Los efectos de partículas los producen **eventos especiales**, como la barca navegando por la superficie del agua.
- La cantidad y el activado/desactivado de los efectos de partículas se pueden **ajustar** en los **ajustes**, para evitar problemas de rendimiento.

### 💎 Materiales avanzados

- Los materiales avanzados son el material **acrílico**.
- El jugador puede activar o desactivar los materiales avanzados en los **ajustes**.
- Con los materiales avanzados activados, las **zonas vacías** de la GUI (controles, tarjetas, etc.) se vuelven un material translúcido y difuminado.

---

## 🕒 Sistema de tiempo

El **tiempo** siempre pasa volando, hasta el punto de que nos perdemos muchas cosas.

### ⏱️ Conversión de tiempo

- **Un día** del juego equivale a **una hora** real.
- La proporción entre el tiempo del juego y el tiempo real es de **1:24**.

### 🕐 Franjas horarias

- Tanto el **día** como la **noche** del juego duran **30 minutos**.
- En **un día** (60 minutos), las franjas horarias del juego se dividen así:
	- Amanecer: minutos 1-2.
	- Mañana: minutos 2-10.
	- Mediodía: minutos 11-20.
	- Tarde: minutos 21-28.
	- Atardecer: minutos 29-30.
	- Noche: minutos 31-60.

---

## 💾 Sistema de guardado

**Guarda** el **progreso actual** del juego para que nuestros peces y nuestra sal estén a salvo.

### 🗃️ Guardar

- En la página de **guardado**, el jugador puede hacer clic en el botón **obtener partida** para **guardar** el progreso actual.
- En la página de **guardado**, el jugador puede hacer clic en el botón **cargar partida** para **cargar** una partida guardada.
