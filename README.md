<img src = "https://www.justfocus.fr/wp-content/uploads/2020/05/velo-paris.jpg" title = "Cyclistes parisiens" alt = "Photo sur laquelle nous pouvons voir des personnes faisant du vélo sur une piste cyclable au centre de Paris">

# Aménagement du territoire francilien :<br/> Projets d'aménagements cyclables subventionnés par la Région Île-de-France

En 2020, l'arrêt des activités humaines dû à la pandémie, a permis de révéler l'impact positif de cet arrêt sur la qualité de l'air en Île-de-France (IDF).

Dans ce contexte, j’ai choisi d’aborder la thématique de la mobilité en IDF. Et cela afin de pouvoir comprendre comment aménager le territoire et ainsi, favoriser l'abandon du véhicule personnel au profit du vélo.
Aujourd'hui, des milliers de franciliens se rendent chaque jour à leur travail, se trouvant pour une grande majorité à Paris intra-muros ou dans la petite couronne de Paris. Certains franciliens utilisent leur voiture afin d'effectuer ce trajet quotidien. Le territoire francilien n’est pas encore optimal sur la question des pistes cyclables. L’objectif de cette data visualisation est de visualiser les territoires en développement sur cette question. En effet, Paris est un territoire très développé et dispose d’une importante variété de transports en communs et de pistes cyclables reliées à sa banlieue proche. L'enjeu est de comprendre comment nous pouvons améliorer l'aménagement de pistes cyclables dans ces territoires et encourager ses habitants à avoir les bons gestes.<br/>

Cela pourrait permettre une réflexion autour de l’amélioration des zones cyclables et de se rendre compte de la nécessité de celles-ci.

Le réseau de transports en IDF est très complexe. Pour cette raison, j’ai choisi de ne prendre en compte que Paris et sa petite couronne.


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

En utilisant le logiciel OpenRefine, j'ai pu nettoyer, organiser et optimiser mon jeu de données afin que ce dernier réponde à ma problématique.
Pour cela, il est possible de télécharger le fichier .json contenant l'historique des opérations réalisées sur OpenRefine.

* <a href="https://wetransfer.com/downloads/3b640124cbd7feabdb960586dc81c77720210202112241/775b734f42583f1cb85328f9eff995e320210202112241/20510e">Télécharger le jeu de données nettoyé</a>
* <a href="https://wetransfer.com/downloads/3b640124cbd7feabdb960586dc81c77720210202112241/775b734f42583f1cb85328f9eff995e320210202112241/20510e">Télécharger l'historique de modification du jeu de données</a>

### Légende : Voir fichier PDF téléchargeable depuis le lien dans le tableau ci-dessus.

## Visualiser l’information <a name="paragraph3"></a>

Dans un premier temps, j'ai utilisé l'outil Palladio afin de mettre en évidence le nombre de pistes cyclables. Dans cette visualisation, j'ai simplement sélectionné le nombre de pistes cyclables (toutes confondues) et le département associé à chacune.

<svg width="1341" height="800" version="1.1" xmlns="http://www.w3.org/2000/svg" style=""><rect class="overlay" width="1341" height="800" fill="none"></rect><g class="main"><g class="layer nodes"><circle class="node source fixed" r="5" transform="translate(329.6844521495609,411.1634209164299)"></circle><circle class="node source fixed" r="7.340963156372632" transform="translate(214.2692137818483,133.66487219432588)"></circle><circle class="node source fixed" r="7.783932925003668" transform="translate(464.92832202844966,44.553597909076984)"></circle><circle class="node source fixed" r="20" transform="translate(552.3154645370448,341.8590199320205)"></circle><circle class="node target fixed highlighted" r="14.056340223748242" transform="translate(620.5681402910413,209.48014314602676)"></circle><circle class="node target fixed highlighted" r="14.98694448649686" transform="translate(217.5160442797419,276.69596938120617)"></circle><circle class="node target highlighted" r="-3.9222228425577033" transform="translate(388.16505700790094,250.2904598997195)"></circle><circle class="node target highlighted" r="3.298698939863178" transform="translate(378.66659844482456,216.777624911801)"></circle><circle class="node target highlighted" r="-10.967196750250837" transform="translate(435.8143044554281,232.43872124628865)"></circle><circle class="node target highlighted" r="3.298698939863178" transform="translate(417.7948981704635,157.20207794187422)"></circle></g><g class="layer labels"><g class="anchor-node source" transform="translate(326.6425032753157,421.0385152517516)"><text transform="translate(-7.361852076101795,5)" style="font-family: karla, Arial, Helvetica; font-size: 11px;">75</text></g><g class="anchor-node source" transform="translate(205.58327123462755,127.95311660334335)"><text transform="translate(-11.715878595629771,5)" style="font-family: karla, Arial, Helvetica; font-size: 11px;">92</text></g><g class="anchor-node source" transform="translate(468.0121575188964,34.51455864297918)"><text transform="translate(-4.552696598966812,5)" style="font-family: karla, Arial, Helvetica; font-size: 11px;">93</text></g><g class="anchor-node source" transform="translate(559.5367158964132,349.1816506076366)"><text transform="translate(-1.8661488801027855,5)" style="font-family: karla, Arial, Helvetica; font-size: 11px;">94</text></g><g class="anchor-node target highlighted" transform="translate(630.7487073724933,208.01168702462246)"><text transform="translate(-1.1870890912722145,5)" style="font-family: karla, Arial, Helvetica; font-size: 11px;">Voie double sens cyclable sans piste ou bande</text></g><g class="anchor-node target highlighted" transform="translate(207.77199148142995,280.1482979788233)"><text transform="translate(-66.44255771067718,5)" style="font-family: karla, Arial, Helvetica; font-size: 11px;">Piste cyclable</text></g><g class="anchor-node target highlighted" transform="translate(384.96594062767804,260.6061832212339)"><text transform="translate(-88.62792769074417,5)" style="font-family: karla, Arial, Helvetica; font-size: 11px;">Chemin mixte ou voie verte</text></g><g class="anchor-node target highlighted" transform="translate(369.69638563635226,211.44506723865152)"><text transform="translate(-69.89411206097363,5)" style="font-family: karla, Arial, Helvetica; font-size: 11px;">Bande cyclable</text></g><g class="anchor-node target highlighted" transform="translate(445.9704149370773,234.89044428974455)"><text transform="translate(-2.2290573400309692,5)" style="font-family: karla, Arial, Helvetica; font-size: 11px;">Couloir bus ouvert aux cyclistes</text></g><g class="anchor-node target highlighted" transform="translate(419.7152178792296,146.93902751352698)"><text transform="translate(-13.274080107615946,5)" style="font-family: karla, Arial, Helvetica; font-size: 11px;">Autres</text></g></g><g class="layer links"><path class="link" d="M552.3154645370448,341.8590199320205L620.5681402910413,209.48014314602676" href="#path3_4" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M552.3154645370448,341.8590199320205L217.5160442797419,276.69596938120617" href="#path3_5" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M214.2692137818483,133.66487219432588L620.5681402910413,209.48014314602676" href="#path1_4" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M329.6844521495609,411.1634209164299L217.5160442797419,276.69596938120617" href="#path0_5" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M464.92832202844966,44.553597909076984L217.5160442797419,276.69596938120617" href="#path2_5" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M464.92832202844966,44.553597909076984L417.7948981704635,157.20207794187422" href="#path2_9" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M552.3154645370448,341.8590199320205L417.7948981704635,157.20207794187422" href="#path3_9" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M214.2692137818483,133.66487219432588L217.5160442797419,276.69596938120617" href="#path1_5" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M552.3154645370448,341.8590199320205L388.16505700790094,250.2904598997195" href="#path3_6" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M329.6844521495609,411.1634209164299L378.66659844482456,216.777624911801" href="#path0_7" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M464.92832202844966,44.553597909076984L378.66659844482456,216.777624911801" href="#path2_7" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M552.3154645370448,341.8590199320205L378.66659844482456,216.777624911801" href="#path3_7" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M214.2692137818483,133.66487219432588L378.66659844482456,216.777624911801" href="#path1_7" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M214.2692137818483,133.66487219432588L417.7948981704635,157.20207794187422" href="#path1_9" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M464.92832202844966,44.553597909076984L620.5681402910413,209.48014314602676" href="#path2_4" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M329.6844521495609,411.1634209164299L620.5681402910413,209.48014314602676" href="#path0_4" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M329.6844521495609,411.1634209164299L435.8143044554281,232.43872124628865" href="#path0_8" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M464.92832202844966,44.553597909076984L388.16505700790094,250.2904598997195" href="#path2_6" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M464.92832202844966,44.553597909076984L435.8143044554281,232.43872124628865" href="#path2_8" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M214.2692137818483,133.66487219432588L388.16505700790094,250.2904598997195" href="#path1_6" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path><path class="link" d="M329.6844521495609,411.1634209164299L388.16505700790094,250.2904598997195" href="#path0_6" style="fill: none; stroke-opacity: 0.5; stroke: rgb(102, 102, 102); stroke-width: 1;"></path></g></g></svg>

<a href="https://wetransfer.com/downloads/4b6c523f8bd2570c1b388a034607c68520210202112711/ac7a956639b52c4452aa4dd49088cfe320210202112711/f2438d">Télécharger ici</a> le fichier .json permettant d'accéder à un affichage dynamique de ce graphique sur Palladio.

Lorsque nous utilisons les facettes sur Palladio, nous pouvons constater que le département du Val de Marne contient le plus de pistes cyclables, c'est-à-dire 192, au sein de la petite couronne de Paris. Les départements des Hauts-de-Seine et de la Seine Saint-Denis possèdent quasiment le même nombre de pistes cyclables, respectivement 86 et 89. Ce qui représente quasiment la moitié des pistes comptabilisées dans le Val de Marne.


## Éditorialiser la visualisation de données <a name="paragraph4"></a>

Cette carte représente la répartition spatiale des projets de pistes cyclables subventionnées par la région IDF, nous pouvons constater une répartition inégale de ces pistes. De plus, nous remarquons que celles-ci sont disjointes. Certaines se connectent entre elles mais seulement à l'intérieur d'un même département.

<iframe frameborder="0" width="800" height="600" src="https://data.opendatasoft.com/map/embed/projets_de_pistes_cyclables_en_ile-de-france/?&static=false&scrollWheelZoom=true"></iframe>

Cette représentation nous permet également de mettre en lumière des zones enclavées.<br/>;

<iframe frameborder="0" width="800" height="600" src="https://data.opendatasoft.com/map/embed/projets_de_pistes_cyclables_subventionnees_par_la_region_ile-de-france/?&static=false&scrollWheelZoom=false"></iframe>

Cette carte permet de mettre en évidence les pistes cyclables existantes avant octobre 2011 dans le département des Hauts-de-Seine et prendre en compte les pistes cyclables en projets et subventionnés la région IDF. Les pistes cyclables colorées en rouge ont été livrées entre octobre 2011 et la fin de l'année 2018. De ce fait, nous pouvons constater que la région IDF a subventionné des pistes cyclables permettant la continuation des pistes existantes.


Dans un dernier temps, nous pouvons nous poser la question sur le choix de ces aménagements. Un critère pouvant servir de répresentation visuelle est la présence de gares ou de de stations à proximité de ces zones.
