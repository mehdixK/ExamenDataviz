# Aménagement du territoire francilien :<br/> Projets d'aménagements cyclables subventionnés par la Région Île-de-France

En 2020, l'arrêt des activités humaines, et notamment celles liées aux transports, étant dû confinement lié à l’épidémie de Covid-19 a révélé l'impact positif de cet arrêt sur la qualité de l'air en Île-de-France (IDF).

Dans ce contexte, j’ai choisi d’aborder la thématique de la mobilité en IDF. Et cela afin de pouvoir comprendre comment aménager le territoire et ainsi, favoriser l'abandon du véhicule personnel au profit du vélo.
Aujourd'hui, des milliers de franciliens se rendent chaque jour à leur travail, se trouvant pour une grande majorité à Paris intra-muros ou dans la petite couronne de Paris. Certains franciliens utilisent leur voiture afin d'effectuer ce trajet quotidien. La configuration du territoire n’est pas encore optimiser de manière à développer des pistes cyclables. L’objectif de cette data visualisation est de visualiser les territoires en développement sur cette question. En effet, Paris est un territoire très développé et dispose d’une importante variété de transports en communs et de pistes cyclables relié à sa banlieue proche. L'enjeu est de comprendre comment nous pouvons améliorer l'aménagement de pistes cyclables dans ces territoires et encourager ses habitants à avoir les bons gestes.<br/>

Cela pourrait permettre une réflexion autour de l’amélioration des zones cyclables et de se rendre compte de la nécessité de celles-ci.

Le réseau de transports en IDF est très complexe. Pour cette raison, j’ai choisi de ne prendre en compte que Paris et sa petite couronne.

À travers des jeux de données, nous allons visualiser les zones cyclables en IDF et nous les mettrons en relation avec les gares et stations à proximité. En facilitant l’accès aux gares par une piste cyclable et/ou des zones de stationnement de vélos, nous pourrions favoriser l’usage de ce moyen de transport.


# Sommaire
1. [Acquisition des données](#paragraph1)
2. [Structurer les données](#paragraph2)
3. [Visualiser l’information](#paragraph3)
4. [Éditorialiser la visualisation de données](#paragraph4)

## Acquisition des données <a name="paragraph1"></a>

| Source     |     Titre  |   Lien | Lien vers le description des métadonnées |
| ------------- |: -------------: | ---------: | ---------: |
| data.iledefrance.fr     |        Projets d'aménagements cyclables subventionnés par la Région Île-de-France        |      <a href="https://data.iledefrance.fr/explore/dataset/velo_amenag_projets_iledefrance_wgs84/information/">Lien du jeu de données</a> |      <a href="https://data.iledefrance.fr/api/datasets/1.0/velo_amenag_projets_iledefrance_wgs84/attachments/velo_amenag_projets_rif_wgs84_pdf/">Lien vers le document</a> |
| data.iledefrance.fr       |        Hauts-de-Seine - aménagements cyclables        |      <a href="https://data.iledefrance.fr/explore/dataset/amenagements-cyclables/information/?disjunctive.commune&disjunctive.an_ouvert&disjunctive.statut&disjunctive.nom_voie&disjunctive.gestion_voie&disjunctive.nom_off&location=11,48.8367,2.26868&basemap=jawg.streets&dataChart=eyJxdWVyaWVzIjpbeyJjaGFydHMiOlt7InR5cGUiOiJjb2x1bW4iLCJmdW5jIjoiU1VNIiwieUF4aXMiOiJzdF9sZW5ndGhfc2hhcGUiLCJzY2llbnRpZmljRGlzcGxheSI6dHJ1ZSwiY29sb3IiOiIjMDA3MkI3In1dLCJ4QXhpcyI6ImNvbW11bmUiLCJtYXhwb2ludHMiOjUwLCJzb3J0IjoiIiwiY29uZmlnIjp7ImRhdGFzZXQiOiJhbWVuYWdlbWVudHMtY3ljbGFibGVzIiwib3B0aW9ucyI6eyJkaXNqdW5jdGl2ZS5jb21tdW5lIjp0cnVlLCJkaXNqdW5jdGl2ZS5hbl9vdXZlcnQiOnRydWUsImRpc2p1bmN0aXZlLnN0YXR1dCI6dHJ1ZSwiZGlzanVuY3RpdmUubm9tX3ZvaWUiOnRydWUsImRpc2p1bmN0aXZlLmdlc3Rpb25fdm9pZSI6dHJ1ZSwiZGlzanVuY3RpdmUubm9tX29mZiI6dHJ1ZX19fV0sInRpbWVzY2FsZSI6IiIsImRpc3BsYXlMZWdlbmQiOnRydWUsImFsaWduTW9udGgiOnRydWV9">Lien du jeu de données</a> |


## Structurer les données <a name="paragraph2"></a>

## Nettoyager du jeu de données sur OpenRefine :

En utilisant le logiciel OpenRefine, j'ai pu nettoyer, organiser et optimiser mon jeu de données afin que ce dernier réponde à ma problématique.<br/>;
Pour cela, il est possible de télécharger le fichier .json contenant l'historique des opérations réalisées sur OpenRefine.

* Télécharger le jeu de données nettoyé ici
* Télécharger l'historique de modification du jeu de données

### Légende (voir aussi le fichier de métadonnées fourni) :

* OBJECT_ID : Numéro interne de référence
* Shape : Feature geometry.
* NOM : Nom de la voie si elle est connue, sinon type d'aménagement.
* ID : Identifiant TOMTOM pour les objets n'ayant pas été re-vectorisés.
* TYPO5 : Typologie en 5 postes des aménagements cyclables :- Piste cyclable- Bande cyclable- Couloir de bus ouvert aux cyclistes- Chemin et voie verte- Voie double sens cyclable sans piste ou bande (correspond au contre sens cyclable)
* MOA : Nom du maitre d'ouvrage
* NUMDEP : Numéro du département de localisation de l'aménagement
* DIRECTION : Renseigne la direction possible de l'aménagement :- unidirectionnelle : les cyclistes ne peuvent emprunter l'aménagement que dans un seul sens.- * * Bidirectionnelle : les cyclistes peuvent emprunter l'aménagement dans les deux sens.Pour les aménagements unidirectionnels, le sens de circulation autorisé est déterminé par le sens de création de l'objet géographique.
* LATERAL : Latéralité de l'aménagement cyclable :- sur un côté de la voie (uni-latéral)- de chaque côté de la voie (bilatéral)
* ZONE : Type de zone où se situe l'aménagement :- aire piétonne- zone de rencontre- zone 30
* DOUBLSENS : Indique si le sens de circulation de l'aménagement est en contre sens de la circulation automobile
* TYPO_MOA : Type du maitre d'ouvrage : commune, EPCI, Département, autres. DATE_CP : Date de la commission permanente
* SHAPE_Length : Length of feature in internal units.


## Visualiser l’information <a name="paragraph3"></a>

Dans un premier temps, j'ai utilisé la plateforme proposer par OpenDataSoft afin de mettre en évidence le nombre de pistes cyclables. Dans cette visualisation, j'ai simplement sélectionné le nombre de pistes cyclables (toutes confondues) et le département associé à chacune.

Intégrer le bar chart.

Nous pouvons constater que le département du Val de Marne (94000) contient le plus d'entrées donc le plus de pistes cyclables au sein de la petite couronne de Paris. Les départements des Hauts-de-Seine et de la Seine Saint-Denis possèdent quasiment le même nombre de pistes cyclables, respectivement 86 et 89. Ce qui représente quasiment la moitié des pistes comptabilisées dans le Val de Marne.


## Éditorialiser la visualisation de données <a name="paragraph4"></a>

Cette carte représente la répartition spatiale des projets de pistes cyclables subventionnées par la région IDF, nous pouvons constater une répartition inégale de ces pistes. De plus, nous remarquons que celles-ci sont disjointes. Certaines se connectent entre elles mais seulement à l'intérieur d'un même département.

<iframe frameborder="0" width="800" height="600" src="https://data.opendatasoft.com/map/embed/projets_de_pistes_cyclables_en_ile-de-france/?&static=false&scrollWheelZoom=true"></iframe>

Cette représentation nous permet également de mettre en lumière des zones enclavées.<br/>;

<iframe frameborder="0" width="800" height="600" src="https://data.opendatasoft.com/map/embed/projets_de_pistes_cyclables_subventionnees_par_la_region_ile-de-france/?&static=false&scrollWheelZoom=false"></iframe>



Dans un dernier temps, nous pouvons nous poser la question sur le choix de ces aménagements. Un critère pouvant servir de répresentation visuelle est la présence de gares ou de de stations à proximité de ces zones. Pour cela, j'ai enrichi cette carte avec une autre jeu de données traitant des gares et stations ferroviaires en IDF.<br/>;
