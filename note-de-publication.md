---
description: 'Historique des modifications, nouveautés et améliorations.'
---

# Notes de publication

![Notes de mises &#xE0; jour JdBEdit](.gitbook/assets/update_uxn2.png)

## 22-08-2020 - v2.8.0

### Fixation de bugs et améliorations

* Correction d'un problème où la position de défilement pouvait sauter lors d'un clic sur une sélection dans Chrome.
* Correction d'un bug où la mise en page de l'éditeur pouvait rester confuse après un appel à rafraîchir lorsque l'option **retour à la ligne** était activée.
* Bloque la fermeture de la boîte de dialogue lorsque l'éditeur perd le focus.
* Désactive la mise en évidence lorsque l'éditeur n'a pas le focus.
* Mise à jour de **CodeMirror** de la version `5.22.2` à `5.57.0`

## 06-08-2020 - v2.7.0

### Fixation de bugs et améliorations

* Les notes peuvent à nouveau être supprimée individuellement.

### Nouveautés

Plus d'options sont ajoutées dans le panneau de partage pour un partage plus personnalisé :

* Lecture seule
* Inclure la sélection 
* Afficher le code en pleine page

## 29-07-2020 - v2.6.1

### Fixation de bugs et améliorations diverses

Pas grand chose à mentionner.

## 07-06-2020 - v2.6.0

### Fixation de bugs et améliorations

* Le champ de code est correctement mis en Pleine page lorsque ce mode est activé.
* Curseur mis sur pointeur lorsque vous survolez un lien dans l'aperçu d'un fichier JSON.
* Les librairies ont été mis à jour pour l'ajout rapide dans le panneau Recherche des librairies \([libraries](https://code.wetrafa.xyz/?modal=libraries)\).
* Améliorations diverses

### Nouveautés

* Nouvelle interface du panneau Extraits de code \([addTo](https://code.wetrafa.xyz/?modal=addTo)\).
* Certains éléments du panneau Paramètres ont été réorganisés.
* La navigation dans l'historique de modifications est désormais accessible via la barre de touches juste au dessus de votre code.
* [**Notes**](https://code.wetrafa.xyz/?modal=notes) : 
  * Ajout de la date de création/dernière modification d'une note.
  * Vous pouvez réorganiser les notes à votre guise.
  * Plus besoin de développer chaque note pour la modifier ou la supprimer, car vous pouvez désormais les faire tout en gardant les notes réduites.

## 08-05-2020 - v2.5.0

### Fixation de bugs et améliorations

* La mise en commentaire du texte dans différents langages pris en charge est désormais stable.
* Un délai de 5 secondes vous est accordé pour annuler la suppression d'un gist ou d'un brouillon avant qu'il disparaisse définitivement.
* Améliorations diverses

### Nouveautés

* Les formats YAML et TOML sont désormais pris en charge. Vous pouvez maintenant éditer vos fichiers de paramètres en toutes tranquillité. Le HTML, Markdown, SVG, JSON et Texte brut \(et JS, CSS, TOML, YAML, Python et Java en mode édition uniquement\) sont pris en charge.
* Les fermetures involontaires de la page/onglet ne vous feront plus perdre votre travail, car JdBEdit vous en prévient lorsque votre travail n'est pas enregistré.

## 11-04-2020 - v2.4.0

### Fixation de bugs et améliorations

* Amélioration de la fonctionnalité pleine page.
* Comme pour l'aperçu du code, il est désormais possible de coder en plein écran.
* Un problème de duplication des gists a été résolu.
* Amélioration des performances.

### Nouveautés

* Lors du téléchargement d'un fichier en tant que fichier Word, tous les scripts \(s'il y en a\) contenus dans le code sont retirés, car Word n’exécute pas JavaScript.
* JdBEdit insère maintenant la plage de sélection dans l'URL pour permettre de pointer une partie spécifique du code lors du partage d'un fichier.
* Il y a désormais une demande de confirmation lorsque vous essayez de dupliquer un gist en l'ouvrant en tant que template afin d'éviter toute perte de données non sauvegardées.

## 07-04-2020 - v2.3.1

### Fixation de bugs mineurs

* On peut désormais de nouveau  ouvrir le code normalement sur CodePen.

### Améliorations

* Demande de confirmation de suppression d'une note avant de complètement supprimer celle-ci.
* Interface des onglets pop-ups simplifiée.

**jdb.js** :

* `v1.24.1` → `v1.24.2`
* La fonction `jdb.ellipsis` accepte désormais un troisième paramètre : **texte**. Si le premier paramètre qui peut être un sélecteur ou un DOM est `null`, la fonction traitera le troisième paramètre qui doit être un texte et le retournera le résultat.

```javascript
var text = "Ceci est le texte a découpé si trop long...";
var selecteur = "h1";
var element = document.getElementById("name");

//# Pour découper un text directement :
jdb.ellipsis(null, 25, text);
// Retourne "Ceci est le texte a décou..."

//# Pour découper le texte d'une élément :
jdb.ellipsis(selecteur, 25);
//# ou
jdb.ellipsis(element, 25);
// Ne retourne rien mais découpe automatiquement
// le texte de l'élément sélectionné et le
// remplace par "Ceci est le texte a décou..."
```

* Le paramètre `callback` de la fonction `jdb.getUrlParam` a été amélioré afin d'utiliser la valeur du paramètre URL quelle qu’elle soit. Exemple :

```javascript
jdb.getUrlParam("name", null, function (value) {
    if (value !== null) {
        // URL = https://..../?name=xxxx
        // Le paramètre existe dans l'URL.

        if (value === "John") {
            // URL = https://..../?name=John
            // La valeur du paramètre est "John".
            ...
        }
        ...
    } else {
        // URL = https://..../
        // Le paramètre n'existe pas dans l'URL.
        ...
    }
});
```

## 25-03-2020 - v2.3.0

### Fixation de bugs mineurs et majeurs

* Ajour du paramètre URL lors de l'ouverture de dernier fichier ouvert.

### Améliorations

* Amélioration du fonctionnement d'autres paramètres URL.
* Amélioration de la fonctionnalité **Aller à la ligne** : Nouveau style + atteinte instantanée de la ligne sélectionnée.
* JdBEdit propose de rouvrir le fichier Gist ouvert en dernier si celui-ci n'a pas été supprimé via le navigateur utilisé.

**jdb.js** :

* `v1.24.1` → `v1.24.2`
* Meilleur description du code
* Réduction de taille du fichier
* Suppression de fonctions : 
  * `jdb.head`
  * `jdb.body`
  * `jdb.goBack`
  * `jdb.noBack`
  * `jdb.hide`
  * `jdb.show`
  * `jdb.addEvent`
  * `jdb.addMultipleEvent`

### **Nouveauté**

* Nouvelle interface pour enregistrer des notes dans l'éditeur accessible via la barre de menu. De ce fait, l'option **Sauvegarder vos notes actuelles et à venir** a été retirée des paramètres.
* Nouvelles option **Retour à la ligne forcé** dans les paramètres : permet le passage à la ligne du texte lorsque le panneau du code est  redimensionné à une taille plus petite. Désactivé par défaut.
* Nouvelle barre de navigation pour les mises en formes Markdown mais aussi pour le HTML. 
* Nouveaux raccourcis Emmet pour les classes JdB.CSS : 
  * `button:jdb`
  * `btn:jdb`

Le paramètre URL `?login=true` est remplacé par la destination `/login` qui redirige vers `?modal=login` Nouvelle page des paramètres URL : [code.wetrafa.xyz/url-parameters](https://code.wetrafa.xyz/url-parameters)

## 28-11-2019 - v2.2.3

* Fixation de bugs mineurs.
* Fixation du bug qui empêchait l'importation du fichier dans l'éditeur.
* Amélioration de performances.
* Amélioration de la possibilité de connexion avec un `acces_token` \(jeton d'accès GitHub\).
* Amélioration de l'interface du panneau Paramètre JdBEdit.
* Amélioration des notifications qui prévienne qu'un langage n'est pas pris en charge. 
* Amélioration de l'interface du panneau de connexion qui s'appelle désormais Portail de connexion.
* Suppression du conflit dans la création d'un Gist alors q'un brouillon est ouvert, et vice versa.

## 04-11-2019 - v2.2.2

#### Fixation de bugs \(Améliorations\) :

* Ajout d'un badge pro pour les comptes GitHub qui ont un accès PRO.
* Il y a désormais un avertissement lorsque vous ouvrez un brouillon alors qu'il y a du code non sauvegardé.
* Il faudra d'abord fermer le Gist ouvert avant d'ouvrir un brouillon.
* Amélioration des moyens de connexion.

## 24-09-2019 - v2.2.1

#### Fixation de bugs \(Améliorations\) :

* Ajout d'un badge pro pour les comptes GitHub qui ont un accès PRO.
* Vous pouvez à nouveau  rentrer votre code couleur dans le sélecteur de couleur.
* Ajout d'aide pour résoudre les certains problèmes rencontrés dans l"éditeur.

## 21-08-2019 - v2.2.0

#### Fixation de bugs \(Améliorations\) :

* Retirer le paramètre URL modal lorsque le panneau en question n'est pas affiché ; et le remettre lorsque le panneau est affiché.
* Ajout de plus d'informations sur les types de fichiers pris en charge.
* Fixation d'un bug mineur dans l'historique de fichiers ouverts.
* Possibilité de télécharger en version `.docs` les fichiers HTML, Markdown et Texte brut uniquement.
* Désactivation du panneau d'aperçu améliorée.
* L'éditeur se désactive et devient inutilisable lorsque l'accès aux cookies est interdit.
* Fixer le lien du script `emmet.js`
* Les couleurs sélectionnées sont désormais sauvegardées dans le Selecteur de couleur. Jusqu'à 30 couleurs peuvent êtres sauvegardées.

## 19-08-2019 - v2.1.9

#### Fixation de bugs mineurs \(Améliorations\) :

* Correction de quelques fautes de frappe.
* Suppression du bogue lors de l'envoi du formulaire de contact.
* Mise à jour de liens corrompus.
* Correction du bug lors de l'envoi du formulaire de contact.

## 15-07-2019

#### Fixation de bugs mineurs \(Améliorations\) :

* Correction de quelques fautes de frappe.
* Suppression du bogue lors de l'envoi du formulaire de contact.
* Mise à jour de liens corrompus.

## 27-12-2018

### Sauvegarde des notes

#### Nouveau

Pour ceux qui aiment faire des petites notes ou une sorte de liste de tâches pendant qu'ils codent, JdBEdit vous offre aussi la possibilité de sauvegarder vos notes et de les récupérer à n'importe quel moment, sur n'importe quel document.

Pour sauvegarder des notes, allez dans l'onglet **Paramètre JdBEdit** puis cochez-y la case **Sauvegarder vos notes actuelles et à venir** pour enregistrer vos notes à chaque fois vous en créer un.

Pour récupérer des notes, il suffit d'ouvrir le **Menu A**, puis survoler le bouton **Édition**, puis cliquer sur **Récupérer les notes sauvegardées.** Vous pouvez éviter supprimer ces notes sauvegardées. Le bouton **Supprimer les notes sauvegardées** se situe juste après le bouton **Récupérer les notes sauvegardées**.

Accès : _\*\*_`Menu A` &gt; `Édition` &gt; _Récupérer les notes sauvegardées_

## 25-12-2018

### Plus d'espace pour le code

#### Amélioration

Pour vous faire encore plus de place, j'ai non seulement orienté certaines notifications vers le centre des notifications mais j'ai aussi réduit la hauteur de la barre de navigation et donné la possibilité de masquer la barre de crédit fixée en bas de la page.

## 23-12-2018

### Enregistrer un brouillon

#### Nouveau

Cela s'est probablement passé à plusieurs reprises à chacun d'entre nous. Vous travaillez sur un code ou un projet quelconque dans un éditeur, l'onglet ou le navigateur se bloque, l'ordinateur s'éteint, une panne électrique, etc., et nous nous grattons les cheveux parce que nous n'avons pas pu sauvegarder le travail.

En plus de la possibilité de télécharger votre code sur l'appareil ou en ligne, JdBEdit offre désormais la possibilité de créer un brouillon de votre code qu'il récupérera automatique au prochain chargement \(ex : après actualisation, après des jours, etc.\).

Ce brouillon contient le titre et la description du code et le code en soi et permet de stocker une copie du code sur lequel vous travaillez sur votre appareil, de sorte que vous ne perdez rien \(même si vous êtes sans connexion internet\).

Il n'y a aucun délais d'expiration pour les brouillons.

Accès :

* `Menu A` &gt; `Edition` &gt; _Enregistrer un brouillon_
* `Ctrl` + `B`

## 21-12-2018

### Centre de notifications

#### Nouveau

Le nouveau centre des notifications vous donne accès aux notifications persistantes, toutes en un seul lieu, afin de vous libérer de la place sur l'écran. Une fois le centre de notifications ouvert, toutes les notifications contenues sont marquées comme lues excepté la notification pour l'acceptation de l'utilisation des cookies qui résistera tant que vous n'avez pas acceptez l'accord.

Accès :

* _La cloche sur la barre de navigation_,
* `Ctrl` + `Alt` + `0`

## 05-09-2018

### Ajout rapide de librairies JS et CSS

#### Amélioration

Ajoutez désormais n'importe quelle bibliothèque CSS et ou JS à votre document en mettant le curseur à l'endroit où vous souhaitez insérer la balise \(`script` ou `link`\) du fichier de votre bibliothèque, ensuite, faites une recherche rapide sur [CDNJS](https://cdnjs.com) via le panneau **Librairie**.

Accès :

* `Menu A` &gt; `Edition` &gt; _Ajouter une ressource externe_.
* [https://code.wetrafa.xyz/?modal=libraries](https://code.wetrafa.xyz/?modal=libraries)

## 10-04-2018

### Sélecteur de couleur

#### Nouveau

La nouvelle interface utilisateur du sélecteur de couleur JdBEdit est désormais disponible dans les sections de style HTML et en mode d'édition CSS. Vous avez une variété de choix de couleurs à découvrir en survolant tout simplement le curseur de votre souris sur le grand cadre de l'onglet Sélecteur de couleur. Cliquez sur la couleur active et obtenez son code et 10 autres dégradées de la couleur sélectionnée.

Accès :

* `Menu A` &gt; `Options` &gt; `Outils` &gt; _Sélecteur de couleur_.
* [https://code.wetrafa.xyz/?modal=colorPicker](https://code.wetrafa.xyz/?modal=colorPicker)

### Des titres d'onglets intelligents pour un meilleur marquage

#### **Amélioration**

Le titre du fichier devient le titre de la page, ainsi les signets et les onglets du navigateur auront une étiquette significative. Ce titre peut être définie soit par une balise `<title>Mon titre</title>` dans le document \(si votre fichier est en HTML\), soit JdBEdit génère un titre comme par exemple "JdBEdit\_5755.html". Le nom du fichier doit contenir l'extension du langage par défaut de votre fichier afin d'appliquer la bonne colorisation du code. JdBEdit peut vous proposer aussi une extension pour les 4 langages \(HTML, CSS, JavaScript et Markdown\) pris en charge par l'éditeur.

Pour nommer votre fichier, rendez-vous dans le champ de texte se trouvant entre le bouton `Exécuter` et le bouton `valider` de la barre de navigation.

Lors de l'enregistrement \(en ligne ou par téléchargement\), si aucun nom n'est attribué à votre fichier, JdBEdit donnera alors automatiquement un nom à votre fichier.

## 22-02-2018

### Nouvelle Console JavaScript

#### Nouveau

Il y a une console JavaScript intégrée à l'éditeur JdBEdit - plus vraiment besoin d'ouvrir des outils de développement externes pour tester vos petits codes. Exécutez votre code JavaScript et faites noter dans la console le résultat de votre code \(s'il doit y en avoir\) en utilisant `console.log`.

**Exemple:**

```javascript
var person = {
  name: "John",
  skills: ["JavaScript", "HTML"]
};
console.log(person.name + " est fort en " +
            person.skills.join(" et ") + " mais surtout en " + 
            person.skills[0]);
```

Accès :

* `Menu A` &gt; `Options` &gt; _Console_
* `Ctrl` + `Alt` + `C`
* \_\_[_https://code.wetrafa.xyz/?modal=console_](https://code.wetrafa.xyz/?modal=console)\_\_

## 04-12-2017

### Emmet

#### Nouveau

**JdBEdit prend désormais en charge** [**Emmet**](http://docs.emmet.io/)**.** Emmet est un plugin pour de nombreux éditeurs de texte populaires qui améliore considérablement le flux de travail HTML et CSS.

#### Avantages d'Emmet

* Sa syntaxe s’inspire des sélecteurs CSS,
* Chaque abréviation est transformée au moment de l'exécution: il suffit de modifier légèrement son nom pour obtenir un résultat différent,
* Avec Emmet, vous pouvez écrire rapidement un tas de code, envelopper le code avec de nouvelles balises, parcourir et sélectionner rapidement des parties de code importantes et plus encore!

En HTML, essayez de taper `ul.site-nav>li*4>a{Lien $}` et appuyez sur `Tab`.

En CSS, essayez `df`, ensuite `Tab` et cela va se développer en `display: flex;`.

Emmet est activable dans les paramètres de l'éditeur.

## 27-11-2017

### 30+ Bibliothèques CSS et JavaScript

#### Nouveau

Ajoutez des bibliothèques CSS et JavaScript populaires à votre page en mettant le curseur à l'endroit où vous souhaitez insérer la balise, ensuite, sélectionnez la bibliothèque voulu depuis les paramètres.

* Accès : [https://code.wetrafa.xyz/?modal=libraries](https://code.wetrafa.xyz/?modal=libraries)

## 23-11-2017

### Télécharger la page en tant que fichier html autonome

#### Amélioration

Gardez une copie locale de votre code dans un fichier qui se chargera dans n'importe quel navigateur, au clic d'un bouton ou au glisser/déposer. Disponible au `Menu A` &gt; `Fichier` &gt; _Télécharger_.

## 30-08-2017

### Panneau tout en un

#### Nouveau

Ne placez pas votre code dans 3 petites cases, utilisez une véritable page html pour éviter les problèmes d'importation et d'exportation quand vient le temps d'utiliser votre démo

## 24-07-2017

### Paramètres JdBEdit

#### Amélioration

**Les paramètres de l'éditeur ont atterri**, vous pouvez maintenant définir quelques points comme le niveau et l'unité d'indentation, la police du champ de code, la dissimulation des numéros de ligne, le theme, la taille et la famille de police de caractère, mode lecture seul, mode d'aperçu automatique, etc.

Étant donné que certains violoneux ne sont pas des amateurs énormes de choses automatiques, j'ai également ajouté la possibilité de désactiver la fermeture automatique des balises HTML et l'autocompletion que vous pourrez réactiver quand vous le souhaitez.

* Accès : [https://code.wetrafa.xyz/?modal=setting](https://code.wetrafa.xyz/?modal=setting)

## 19-06-2017

### **Début de changelog pour JdBEdit**

#### Nouveau

**De grandes nouvelles aujourd'hui**, je commence à faire le changelog public pour mon éditeur, JdBEdit via lequel vous serez toujours mis au courant de toutes les mises à jour, améliorations et corrections qui seront faites sur [**code.wetrafa.xyz**](https://code.wetrafa.xyz/).

Même si je travaille tout le temps sur JdBEdit, parfois il peut sembler que peu de choses se passent. Ce changelog \(journal des modifications\) est ici pour améliorez cette partie très importante de la communication entre vous et moi.

Vous recevrez toujours une notification dans l'éditeur lorsque j'apporterai une modification dans l'application. Toutes les modifications, les plus importantes en tout cas, seront disponibles sur notre [page publique du journal des modifications](https://docs.code.wetrafa.xyz/changelog).

