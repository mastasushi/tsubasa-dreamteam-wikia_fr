# Ajouter un personnage au Wikia

Voici la procédure pour ajouter un personnage

1. Ajouter les images dans le wikia :

http://fr.captain-tsubasa-tatakae-dream-team-fr.wikia.com/wiki/Sp%C3%A9cial:T%C3%A9l%C3%A9verser

- Le format de l'image pour les portraits doit être sous la forme suivante :
![Portrait](doc/000208%20Misaki-doubletete-vitesse-ligue.png =100x)

`{idJoueur}_{nom_personnage}-{TS_principage}-{type}-{acquisition}.png`

ex: 000208 Misaki-doubletete-vitesse-ligue.png

- Pour la miniature :

`{idJoueur}_{nom_personnage}-{TS_principage}-{type}-{acquisition}-thumb.png`

ex: 000208 Misaki-doubletete-vitesse-ligue-thumb.png

2. Ajouter une page

![Ajouter une page](doc/ajouter%20page.png)

3. Choisir un titre sur le format "Joueur - Nom joueur"
ex: Elcide Pierre - L'Artiste du Terrain

Si on vous le demande, sélectionner le mode "page vierge".

4. Passer en mode source

- Copier le contenu de "fiche perso.txt"

    [fiche perso.txt](doc/fiche%20perso.txt)

- Remplir les infos (ces modèles ne sont plus à jour)

    [Exemple Goal](doc/0000XX_Goal.txt)

    [Exemple Joueur](doc/0000XX_Joueur.txt)

~~~Pour l'instant on rentre les stats des versions UR, mais dans le futur, on fera peut-être SSR + UR sur la même page ou alors sur 2 pages séparées, on verra.~~~

On peut maintenant remplir les stats sur la **version en rareté par défaut** et également sur la **version évoluée**.

toutes les informations préfixées par `base_` concernent la version non évoluée.

### Voici les valeurs possibles pour chaque catégorie

Rareté
```
rareté = N | R | SR | SSR | UR
```

Type
```
type = force | vitesse | technique
```

Poste

```
poste = GB | DF | MD | MO | AT
```
Quand le joueur a plusieurs postes, rajouter une nouvelle ligne avec _2, _3, ex:
```
|poste = AT
|poste_2 = MO
```

Acquistion
```
acquisition = Dream Fest | Dream Collection | Recrutement | Scénario | Grande Rencontre |
              Raid SSR | Confédération | PvP | Ligue | Evénements Spéciaux
```

### Techniques Spéciales
La TS principale doit être renseignée TS_main, et tous ses paramètres ensuite TS_main_type, TS_main_effet, TS_main_coût, etc...

Idem pour les TS suivantes, TS_1_type, TS_2_type, etc...

#### Valeurs possibles

Type:
```
_type = tir | balle_haute | balle_basse | passe | combinaison | dribble |
        tacle | interception | contre | arrêt | coup_de_poing
```

Effet:
```
_effet = {{effet_souffle|nombre}} | {{effet_distance}} | {{effet_angle}}
```

Combinaison:
```
_combinaison = {{combinaison|joueur1|joueur2|joueur3}} | *
```

Les lignes qui ne sont pas applicables doivent être supprimées (ex: TS_1, TS_2, farmable, passive_skill...)

Lorsque vous ne connaissez pas une info, mettez ?, si quelqu'un la connait, il le signalera.

Pour les 4 dernières lignes, il ne faut pas mettre la valeur à Non, mais supprimer la ligne, si par exemple le perso n'est pas farmable.


5. Ajouter le perso dans la liste des personnages :

http://fr.captain-tsubasa-tatakae-dream-team-fr.wikia.com/wiki/PERSONNAGES?action=edit

passer en mode source et ajouter l'élément dans la bonne section sous la forme suivante :

```
=== SSR Farmable ===
<gallery ...>
...
000227_Taro Misaki-champagneduo-vitesse-farm-thumb.jpg|'''Taro Misaki''' - Football Champagne|link=Taro Misaki - Football Champagne
</gallery>
```

en respectant l'ordre décroissant sur l'ID (qui donne plus ou moins l'ordre chronologique de sortie)

