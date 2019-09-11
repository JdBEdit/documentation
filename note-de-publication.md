---
description: 'Historique des modifications, des nouveautés et améliorations.'
---

# Note de publication

## 02-09-2019 - v2.2.1 beta

#### Fixation de bugs \(Améliorations\) :

* Ajout d'un badge pro pour les comptes GitHub qui ont un accès PRO.

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

Pour sauvegarder des notes, allez dans  l'onglet **Paramètre JdBEdit** puis cochez-y la case **Sauvegarder vos notes actuelles et à venir** pour enregistrer vos notes à chaque fois vous en créer un.

Pour récupérer des notes, il suffit d'ouvrir le **Menu A**, puis survoler le bouton **Édition**, puis cliquer sur **Récupérer les notes sauvegardées.** Vous pouvez éviter supprimer ces notes sauvegardées. Le bouton **Supprimer les notes sauvegardées** se situe juste après le bouton **Récupérer les notes sauvegardées**.

Accès : ****`Menu A` &gt; `Édition` &gt; _Récupérer les notes sauvegardées_

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



