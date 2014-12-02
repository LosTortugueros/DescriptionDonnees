# DescriptionDonnees

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
