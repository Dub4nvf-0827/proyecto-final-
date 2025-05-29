# proyecto-final- [pensamiento algoritmico]
## 👥 Integrantes del grupo
- Angel Cortes (Angel7952)
- Duban Vargas (Dub4nvf-0827)
-### Proyecto: Sistema de Parqueadero Inteligente (Python CLI)
- Simulación de mapa de parqueadero con matriz 8x8.
- Registro automático de entrada y salida de vehículos.
- Cálculo dinámico del tiempo de permanencia y tarifa.
- # Sistema de Parqueadero (Python CLI)
- ## 🚗 Funcionalidades
- mostrar la vista del parqueadero de forma una (matriz visual).
- ingresar los vehiculos al paqueadero.
-  Calcular tiempo de permanencia y tarifa al salir
- calcula la tarifa 1000 por minuto (tiempo rela).
- Control de disponibilidad de espacios.
## 📌 Desarrollos innovadores
### 1. Representación visual tipo mapa
¿Para qué se implementó?
para que el usuario pueda ver visualmente grafica para ver la disponibilidad del parqueadero.
¿Por qué se consideró necesario?
Hace más intuitiva la gestión, permitiendo ver claramente las zonas de entrada, salida, vía, lugar libre (`L`) y ocupado (`X`).
¿Cómo se implementó?
- Se usa una matriz de 8x8.
- 'E' marca la entrada, 'S' la salida.
- 'L' representa lugares libres, 'X' los ocupados.
- Se usa una función para imprimir la matriz al usuario.
### 2. Registro de tiempo con `datetime`
¿Para qué se implementó?
para cobrar de manera precisa por el tiempo de uso del parqueadero
¿Por qué se consideró necesario?
brinda realismo y permite automatizar el cobro del parqueadero
¿Cómo se implementó?
- Se guarda la hora de entrada usando `datetime.now()` se le nombro como una funcion de llamada.
- al salir, se calcula cuanto tiempo estuvo en el parqueadero, se calcula por minuto.
- - Se calcula la tarifa multiplicando por $1000 por hora (proporcionalmente).

# 🎮 Juego RPG de Pokémon en C++
Este proyecto es un juego de rol (RPG) sencillo basado en Pokémon, desarrollado en C++ para jugar en la línea de comandos (CLI). El juego permite al jugador enfrentarse a un poderoso Mewtwo usando un equipo de Pokémon con habilidades y efectos de estado, ofreciendo una experiencia de combate estratégica y gestionable.
## ✨ Funcionalidades Clave
* **Combate por Turnos:** Permite que dos Pokémon se enfrenten alternando turnos para atacar.
* **Menú de Interacción:** Un menú textual para que el jugador realice acciones.
* **Sistema de Ataques:** Cada Pokémon tiene al menos dos ataques distintos.
* **Sistema de Victoria:** El combate finaliza cuando un Pokémon queda sin puntos de vida, anunciando al ganador.
## 📌 Innovaciones y Desarrollos Destacados
### 1. Sistema de Energía por Puntos (PP)
* **¿Para qué se implementó?**
  Para añadir una capa estratégica al combate, obligando al jugador a gestionar los recursos de sus Pokémon, ya que cada ataque consume una cantidad específica de puntos de energía (PP).
* **¿Por qué se consideró necesario?**
  Brinda mayor profundidad al juego, haciendo que las decisiones de ataque no sean triviales y que el jugador deba planificar el uso de sus habilidades más poderosas. Evita el "spam" de un solo ataque fuerte.
* **¿Cómo se implementó?**
    * Cada habilidad de Pokémon tiene un valor de costo de PP.
    * Los Pokémon tienen un contador de PP que disminuye al usar habilidades.
    * Si los PP son insuficientes, la habilidad no puede ser utilizada.
### 2. Capacidad de Cambio entre Múltiples Pokémon
* **¿Para qué se implementó?**
    Para permitir al jugador una mayor flexibilidad y estrategia durante el combate, pudiendo adaptar su equipo a la situación actual.
* **¿Por qué se consideró necesario?**
    Aumenta las opciones tácticas del jugador, permitiéndole cambiar a un Pokémon con ventaja de tipo, más salud o con PPs disponibles cuando su Pokémon actual está en desventaja o agotado.
* **¿Cómo se implementó?**
    * El jugador comienza con un equipo de tres Pokémon predefinidos.
    * Existe una opción en el menú de combate para "Cambiar Pokémon".
    * El jugador puede seleccionar cualquier Pokémon de su equipo que esté vivo para que entre en combate.
### 3. Efectos de Estado (Veneno, Quemadura, Electrocutado)
* **¿Para qué se implementó?**
    Para introducir elementos dinámicos que alteran el curso del combate, añadiendo una dimensión más compleja a las interacciones entre Pokémon y ataques.
* **¿Por qué se consideró necesario?**
    Hace que las batallas sean menos predecibles y más estratégicas. Los efectos de estado obligan al jugador a considerar no solo el daño directo, sino también las consecuencias a largo plazo de los ataques.
* **¿Cómo se implementó?**
    * Ciertas habilidades tienen un efecto de estado asociado (ej. un ataque eléctrico puede "electrocutar").
    * Cada efecto tiene una duración y un impacto específico (ej. veneno/quemadura causan daño por turno, electrocutado puede hacer perder un turno).
    * Los efectos de estado se aplican al inicio de cada turno afectado.
### 4. Mochila con Objetos y Evolución
* **¿Para qué se implementó?**
    Para proporcionar al jugador herramientas adicionales de recuperación y mejora durante el combate, permitiendo mantener a sus Pokémon activos por más tiempo y fortaleciéndolos.
* **¿Por qué se consideró necesario?**
    Ofrece al jugador opciones de supervivencia y progreso. La mochila permite gestionar la vida y la energía, mientras que la evolución añade un sentido de crecimiento y recompensa para los Pokémon.
* **¿Cómo se implementó?**
    * Se implementa una "mochila" o inventario que contiene objetos (ej. pociones para vida, elixires para PP).
    * Hay una opción en el menú de combate para "Usar objeto".
    * Los objetos de evolución se aplican a un Pokémon para cambiar sus estadísticas o habilidades (si la evolución está completamente funcional, puedes detallar más cómo afecta al Pokémon)

