# Description des données loggés

Format global : 
 * données disponibles à cette adresse : http://etud.insa-toulouse.fr/~livet/{username}.json
 * chaque fichier json contient un gros tableau avec les objets décrits ci-dessous

## Programme Java

Toutes les données qui viennent du programme Java ont une source = javalog.

### Touches

```json
{"source":"javalog", "keys": [1417456528,1417456530,1417456530]}
```

Le tableau ```keys``` contient le timestamp à laquelle des touches ont été appuyées.

### Clicks

```json
{"source":"javalog", "clicks": [1417456528,1417456530,1417456530]}
```

Le tableau ```clicks``` contient le timestamp à laquelle des clicks ont été faits.

### Distance parcourue avec la souris

```json
{"source":"javalog","time":1417507642,"distance":0.2959515}
```

Le champ ```time``` contient l'heure à laquelle la distance a été calculée et ```distance``` la distance correspondante en mètres.

### Ram libre sur la machine

```json
{"source":"javalog","ram":1007296512,"time":1417715359}
```
Le champ ```time``` contient l'heure à laquelle la mesure a été prisé, ```ram``` la RAM disponible à ce moment là sur la machine.

### Musique ''next'' sur le raspberry

```json
{'source': 'javalog', 'next': [{'timestamp': '1417743882', 'name': 'The Birds & the Bees', 'artist': 'The 2 Bears'}]}
```

Permet de logger lorsqu'une musique a été passé (sur le jukebox de l'équipe). ```next``` est un tableau contenant le ```timestamp``` auquel le next a été fait et ```name``` et ```artist``` la musique nexté.

## Programme Android
### Boisson bu

```json
{ "source": "mobile", "capteur": "boisson", "timestamp":1293384382, "type":"cafe|the|coca|redbull|eau|soda|biere|autre" }

```
Le champ ```timestamp``` contient l'heure à laquelle la boisson a été bu et ```type``` la boisson correspondante.

### Nourriture mangé

```json
{ "source": "mobile", "capteur": "nourriture", "timestamp":1293384382, "type":"pizza|pfour|crepe|inconnue" }
```
Le champ ```timestamp``` contient l'heure à laquelle la nourriture a été ingurgité et ```type``` la nourriture correspondante.
