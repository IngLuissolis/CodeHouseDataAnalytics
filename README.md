# Análisis Rendimiento Campeón Mundial Qatar 2022

👋 Bienvenido/da

# Descripción del Proyecto:

Para el presente trabajo, se extrajo información de los atributos y estadística del rendimiento de los jugadores de futbol que participaron del campeonato mundial Qatar 2022.

# Hipótesis

- Comprender el rendimiento de la selección Argentina en su conjunto y poder determinar porque fue el campeón del torneo
- Analizar el rendimiento de los jugadores individualmente o para comparar el rendimiento de diferentes jugadores y posiciones.

# Archivo Power Bi ( ProyectoFinal.pbix )

- Solapas:
    - Portada
    - Descripción Proyecto
    - Edad Jugadores
    - Indicadores Ataque x Team
    - Indicadores Defensa x Team
    - Indicadores x Jugador
    - Glosario

- Tablas ( Descripción de Tablas en archivo https://github.com/IngLuissolis/CodeHouseDataAnalytics/blob/master/AnalisisCampeonQatar2022_LuisSolis.pdf )
    - Calendario “birth_year_player”
    - puente “player” (Dimensiones)
    - player_defense
    - player_gca
    - player_misc
    - player_possesion
    - player_shooting
    - player_stats
    - player_passing

- Medidas Calculadas:
    - Max_Goleador = MAX(player_stats[goals])
    - Efectividad_shots = DIVIDE(
    						SUM('player_shooting'[shots_on_target]),
    						SUM('player_shooting'[shots]))
    - Efectividad_goals = DIVIDE(
                            SUM('player_shooting'[goals]),
                            SUM('player_shooting'[goals_per_shot_on_target]))
    - dribbles_completed dividido por passes_received = 
                            DIVIDE(
                                SUM('player_possession'[dribbles_completed]),
                                SUM('player_possession'[passes_received])
                                    )

# Análisis Indicadores (Análisis Argentina vs Francia, Croacia, Marruecos)

- Indicadores Ataque x Team
![Indicadores Ataque x Team](https://github.com/IngLuissolis/CodeHouseDataAnalytics/blob/master/Imagen/Indicadores_Ataque.png)



- Indicadores Defensa x Team
![Indicadores Defensa x Team](https://github.com/IngLuissolis/CodeHouseDataAnalytics/blob/master/Imagen/Indicadores_Defensa.png)



# Conclusiones

- Después de analizar los indicadores de Ataque y Defensa por equipo en la Copa Mundial de Fútbol Qatar 2022, se observó que el equipo de Argentina demostró una alta eficacia en el medio campo en términos de Ataque y Defensa.
- Las variables más destacadas en Ataque fueron los pases completados, tiros al arco, tiros al arco en portería, faltas recibidas y las ocasiones de gol generadas a partir de recuperaciones de balón en la defensa (sca_defense).
- En cuanto a la Defensa por equipo, Argentina demostró una gran actuación en el medio campo. Las variables más destacadas en esta área fueron la recuperación del balón, los pases bloqueados, los tackles en la tercera parte del campo, los dribles ganados y los bloqueos.
- Estos resultados sugieren que el equipo argentino tiene un medio campo sólido que es capaz de realizar una buena transición del juego desde la defensa hasta el ataque. Además, la defensa de Argentina es capaz de bloquear y recuperar el balón con eficacia en el medio campo, lo que les permite mantener la posesión del balón y generar oportunidades de ataque.
- En conclusión, el equipo de Argentina demostró un desempeño sobresaliente en el medio campo tanto en términos de ataque como de defensa. Estos resultados pueden ser útiles para la planificación estratégica de equipos que se enfrenten a Argentina en el futuro.


# Desafios

- Desafio 03: Prototipo del Tablero
    - Archivo:
        - AnalisisCampeonQatar2022_LuisSolis.pdf
        - ProyectoFinal.pbix

- Desafio 02 - Definición Modelo relacional
    - DataSet: Archivos se encuentran en carpeta /DataSet
    - Diagrama Entidad-Relación: /DiagramaER-DataSet.pdf
    - Listado de Tablas: se encuentra en archivo /DataSet/DataSet.xls - solapa Listado de Tablas
    - Listado de columnas de cada tabla: se encuentra en archivo /DataSet/DataSet.xls - solapa Listado de columnas

- Desafio 01 - Descripción del Proyecto - Hipotesis

# Dataset

La información esta separada en 11 archivos CSV y 1 archivo JSON, este ultimo contiene la descripción de los datos.

/Dataset

# Tecnologias utilizadas

- PowerBi

- Microsoft SQL Managment

# Customer Homepage

Animación Gif


# Sitio Deployed



# Feedback

Any suggestion and feedback is welcome. You can message me on email

`edusolis@yahoo.com.ar`
