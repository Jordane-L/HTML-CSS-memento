# HTML-CSS-Memento V1

## I - Les deux familles de balises

1.LES BALISES DE TYPE INLINE

Liste des balises inline les plus courantes :

```<a> </a> ``` Permet d'insérer un lien

```<img/>``` Balise auto-fermante (attention au / en fin de balise) qui permet d'insérer une image

```<em> </em>``` Permet de mettre en avant un mot à un degré normal.

```<input/>``` Balise auto-fermante qui renvoie à un champ de formulaire

```<span> </span>``` Non sémantique, elle permet d'y mettre ce qu'on veut. Une sorte de balise fourre-tout (son équivalent dans la famille des balises block est ```<div>```)

```<strong> </strong>```Permet de mettre en avant un mot à un degré important.

**Particularités**
- Qu'il y ait un retour à la ligne ou non entre deux balises de type inline dans le code, elles apparaitront toujours par défaut les unes à coté des autres dans le navigateur.
- Leur taille est déterminée automatiquement par leur contenu.


2.LES BALISES DE TYPE BLOCK

Liste des balises block les plus courantes :

```<p> </p>``` Balise qui définit un paragraphe

```<h1> </h1>, <h2> </h2>, <h3> </h3>, <h4> </h4>, <h5> </h5>, <h6> </h6>``` Balises qui permettent de définir des titres. Ceux-ci apparaissent par ordre hiérarchique. ```<h1>``` étant le plus important visuellement par défaut mais également aux yeux de Google. En général on utilise les trois premiers niveaux ```<h1>,<h2>,<h3>```

```<div> </div>``` A la manière de la balise span, cette balise est neutre et sert à stocker des éléments de façon non sémantique. C'est une balise fourre-tout.

```<ul> </ul>``` permet de définir une liste à puce non ordonnée. C'est à dire qu'on aura par défaut des points qui viendront se placer devant chaque élément.

 ```<li> </li>``` est la balise enfant de ```<ul>``` et ```<ol>```. Elle définit un élément de la liste. On peut insérer autant de ```<li>``` qu'on le souhaite au sein d'une balise ```<ul>``` ou ```<ol>```
 
```<ol> </ol>``` permet de définir une liste à puce ordonnée. C'est à dire qu'on aura par défaut des numéros qui viendront se placer devant chaque élément.

**Particularités**
- Qu'il y ait un retour à la ligne ou non entre deux balises de type block dans le code, elles apparaitront toujours par défaut les unes en dessous des autres dans le navigateur.
- Leurs dimensions dépendent de leur parent dit "conteneur" par défaut.
- Elles sont redimensionnables via le css
 

3.ON PEUT TRANSFORMER UNE BALISE DE TYPE INLINE EN BALISE DE TYPE BLOCK ET INVERSEMENT

Par exemple une balise ```<a>``` (balise inline par défaut) peut basculer dans la famille des balises de type block.

**Comment ?**
 
Dans votre feuille de style CSS, il suffit d'y appliquer cette règle en ciblant la balise de cette manière : 
```
a {
display: block;
}
```


4.ET SI ON FUSIONNAIT LES DEUX TYPES POUR AVOIR UNE SUPER BALISE

Il est tout à fait possible de combiner les avantages de chacune de ces deux familles de balises. Cela nous donnera deux avantages :
- Placer nos éléments les uns à côté des autres (Rappel : ce qui n'est pas possible si la balise est de type block)
- Pouvoir les redimensionner (Rappel : ce qui n'est pas possible si la balise est de type inline)

**Comment ?**
Dans votre feuille de style CSS, il suffit d'y appliquer cette règle en ciblant la balise en question. Par ex : 
```
a {
display: inline-block;
}
```
