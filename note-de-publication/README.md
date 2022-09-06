---
description: Historique des modifications, nouveautés et améliorations.
coverY: 0
---

# 🎉 Notes de publication

{% hint style="info" %}
Ces notes de publication ne concernent que l'application JdBEdit.
{% endhint %}

## 06-09-2022 - v2.20.0

### Nouveautés

* JdBEdit peut maintenant ouvrir les liens de la structure `//code.wetrafa.xyz/preview/[id]`.

### Améliorations

* Quelques améliorations de performance et de style.
* Suppression des redirections non nécessaires.
* Maintenant le bouton "Dupliquer" sera affiché lorsque l'on se connecte pendant qu'un gist est ouvert.

### Fixation de bugs <a href="#fixation-de-bugs-v-2-13-0" id="fixation-de-bugs-v-2-13-0"></a>

* Correction des fautes de frappes et des erreurs laissés dans le code.

## 01-08-2022 - v2.19.0

### Nouveautés

* Ajout de l'auto-complétion pour les fichiers SQL.
* Ajouter l'intégration `iframe` du gist (en utilisant l'extension `.pibb`).

### Améliorations

* Mise à jour de la section de paramètres.
* Suppression du paramètre `hardwrap`.
* Dans le panneau de sauvegarde de fichier, le bouton "**Enregistrer**" devient "**Mettre à jour le gist**" si vous êtes connecté.e et que vous en êtes le propriétaire.
* Amélioration de l'accessibilité.
* Et quelques autres petites améliorations...

### Fixation de bugs <a href="#fixation-de-bugs-v-2-13-0" id="fixation-de-bugs-v-2-13-0"></a>

* Correction de l'inclusion de la plage de sélection dans l'URL partageable.
* Correction de la surbrillance des balises `pre` dans l'aperçu du code Markdown.

## 07-02-2022 - v2.18.1

_Cette version est étiquetée par erreur. Il doit s'agir de la `v2.18.0` au lieu de la `v2.18.1`._

### Nouveautés

* ⭐ Les notes déjà sauvegardées et celles que vous créerez peuvent désormais être marquées comme important à l'aide du bouton étoile (⭐) se trouvant sur chaque note où lorsque vous éditez un note.
  * Il est aussi possible de ne voir que les notes marquées comme important.

## 30-11-2021 - v2.17.0

**Sous versions de fixes mineurs** : v2.17.1, v2.17.2

### Nouveautés

* Ajout d'une image Gist GitHub pour les réseaux sociaux lors de partage de lien d'un fichier.
* Ajout dans la barre de touches un bouton permettant d'ajouter facilement une section pliable (`details`) dans le HTML et le Markdown.

## 20-10-2021 - v2.16.0

### Nouveautés

* Vous ne gérez pas encore le Markdown ? Pas de problème ! JdBEdit a désormais un bouton qui vous renvoie directement à une page d'aide lorsque vous éditez du Markdown.
* Vous pouvez aussi, à partir de l'historique de fichiers ouverts, ouvrir dans un nouvel onglet un fichier qui n'est pas marqué comme supprimé dans l'éditeur.

### Améliorations

* Avant, lorsque vous modifiez une note créée dans Notes, la note existante était supprimée avant que vous validiez votre modification, ce qui causait la perte de la note au cas où vous annulez la modification. Maintenant, vous pouvez modifier vos notes sans rien craindre.
* Et quelques autres petites améliorations...

## 07-10-2021 - v2.15.0

### Nouveautés

* Ajout d'une nouvelle option pour la prise en charge de la colorisation du code préformaté dans le Markdown. Langages actuellement pris en charge : Python, Java, PHP, C, C++, Objective-C, Ruby, SQL, TOML, YAML, et les langages par défaut : HTML, CSS, JavaScript, JSON, Markdown et XML. Cette option peut être sauvegardée dans les paramètres et partagée avec un fichier.

{% hint style="warning" %}
L'option n'est visible que sur les fichiers Markdown. Ouvrez un gist Markdown ou nommer un nouveau fichier test.md, puis allez dans les paramètres JdBEdit pour voir l'option.

**Attention:** cette colorisation est un paramètre de l'éditeur, par conséquent, elle ne se sauvegarde pas avec le fichier. C'est uniquement pour l'aperçu dans l'éditeur.
{% endhint %}

* Ajout d'un bouton à la barre de navigation pour accéder plus facilement aux commentaires du fichier, s'il y en a.

### Amélioration

* Ajout d'une petite marge supplémentaire au containeur d'aperçu du markdown.

### Fixations de bugs

* Correction d'un bogue entraînant la suppression de toutes les données (à l'exceptions des paramètres) au lieu de toutes les notes sur Notes.

## 26-08-2021 - v2.14.0

**Sous** __ **versions de fixes mineurs** : v2.14.1, v2.14.2, v2.14.3

### Nouveautés <a href="#ameliorations-v-2-13-0" id="ameliorations-v-2-13-0"></a>

* Il est désormais possible d'exécuter du JavaScript dans un fichier .js, sans passer par la balise `script` dans le HTML. Écrivez et exécutez votre JS et JdBEdit s'occupe du reste.
* Maintenant, vous pouvez exécuter un fichier SVG (titre.svg) sans avoir à inclure son code dans un fichier HTML.
* Étant donné que l'éditeur ne s'adapte pas aux petits écrans, lorsque vous êtes sur un écran dont la largeur est inférieure à 1000 pixels, un petit message que vous pouvez ignorer sera affiché.

### Améliorations <a href="#ameliorations-v-2-13-0" id="ameliorations-v-2-13-0"></a>

* JdBEdit ne propose plus de nom de fichier pour les dot files. C'était considéré comme format invalide avant la version 2.13.0, mais désormais, vous n'aurez plus un "blabla.env" en proposition.

### Fixation de bugs <a href="#fixation-de-bugs-v-2-13-0" id="fixation-de-bugs-v-2-13-0"></a>

* Boutons de mise en forme rapide : un bug a été fixé pour l'attribut `alt` de la balise img et le texte de la balise `a`. Lorsque plusieurs lignes de texte (non-URL) ont été sélectionnées, elles sont fusionnées en une seule ligne.
* Le titre de la page d'un fichier introuvable est désormais persistant, même lorsque vous faites une modification dans l'éditeur.

### Suppression de fonctionnalités <a href="#suppression-de-fonctionnalites-v-2-13-0" id="suppression-de-fonctionnalites-v-2-13-0"></a>

* La fonctionnalité permettant de  marquer du texte sélectionné a été supprimée.
* Dans l'historique des fichiers, vous ne pouvez plus "Cliquer pour copier" l'ID d'un fichier supprimé.

## 02-08-2021 - v2.13.0

**Sous versions de fixes mineurs** : v2.13.1, v2.13.2, v2.13.3

### Nouveautés <a href="#nouveautes-v-2-13-0" id="nouveautes-v-2-13-0"></a>

* ⭐ Il est désormais possible de créer les dot files : les fichiers de configurations dont le nom commence par un point. Ex. : `.gitignore`,  `.env`.
* ⭐ Il est possible de redimensionner le panneau d'aperçu en cliquant sur le bouton contenant les dimensions du cadre d'aperçu situé juste au-dessus de celui-ci. Ensuite vous pouvez choisir entre Mobile, Tablette, Ordinateur et Défaut.

![](<../.gitbook/assets/image (2).png>)

* Vous pouvez maintenant partager votre thème de l'éditeur en cochant "Inclure le thème" dans le [panneau de partage](https://code.wetrafa.xyz/?modal=share).
* Dans ce même panneau de partage, vous pouvez ouvrir des liens en cliquant simplement sur l'icône ouvrir.
* Un ouvrant un fichier en fournissant son id dans le [panneau loadFile](https://code.wetrafa.xyz/?modal=loadFile), vous avez la possibilité de l'ouvrir dans un nouvel onglet. Une case à cocher a été ajouté à cet effet.
* Vous souhaitez rapidement supprimer l'historique de modifications (lorsque vous saisissez du texte) ? Pas de soucis. Une combinaison de touches `Alt` + `W` a été ajouté pour cela.
* ⭐ Lorsque vous ouvrez un fichier qui n'existe plus parce qu'il a été supprimé et que vous aviez déjà ouvert ce même fichier avant qu'il soit supprimé (c'est-à-dire qu'il se trouve déjà dans l'historique des fichiers ouverts), ce fichier supprimé sera également placé dans l'historique des fichiers supprimés, comme ça il sera reconnu et marqué par JdBEdit comme inexistant.
* ⭐ Lorsque vous ouvrez un fichier qui a été renommer, mais que ce fichier avait été ouvert avant qu'il soit renommé (c'est-à-dire qu'il se trouve déjà dans l'historique des fichiers ouverts), JdBEdit met à jour le nom du fichier dans l'historique également.
* ⭐⭐ Une des plus grosses nouveautés : l'affichage des commentaires sur les fichiers Gist GitHub. Accédez aux [`Paramètres`](https://code.wetrafa.xyz/?modal=setting) puis `Voir plus des détails`. Tout en bas vous pourrez charger les commentaires au fur et à mesure s'il y en a. Ils ne sont pas chargés par défaut pour économiser les ressources.

![](<../.gitbook/assets/image (7).png>)

* ⭐ Vous pouvez désormais avoir un aperçu en couleur de vos blocs de code dans des fichiers Markdown et les blocs de codes dans les commentaires du fichier. Cette mise en couleur ne s'enregistre pas avec les fichiers et peut s'activer dans les Paramètres.
* Ajout de la police Fira Code.
* ⭐ Ajout de la ligature de la police (disponible uniquement pour les polices qui supportent la ligature). Seule la police "Fira Code" supporte la ligature pour le moment.
* Ajout d'un large espace à la fin du code pour une meilleure visualisation des dernières lignes de votre code. Cet espace ne contient que la dernière ligne et ne fait pas partie du fichier.

### Améliorations <a href="#ameliorations-v-2-13-0" id="ameliorations-v-2-13-0"></a>

* Lorsque vous partagez un fichier gist sur les réseaux sociaux (messages ou postes), vous pouvez désormais voir le titre et la description de ce fichier, et pas que le titre de temps en temps comme avant. JdBEdit a été optimisé pour cela.
* Amélioration des actions des boutons d'édition rapide (pour HTML et Markdown). Avant, il n'était pas possible d'appliquer une balise sur plusieurs sélections de texte, mais désormais, c'est possible. De plus, le balisage des listes a été amélioré.
* La fonction de mise à jour automatique de l'aperçu du code a été optimisée pour exécuter le code le nombre de secondes défini après la dernière inactivité détectée (lorsque vous ne tapez plus).
* En supprimant les notes dans [Notes](https://code.wetrafa.xyz/?modal=notes), lorsqu'il n'y en plus, l'affichage initial indiquant qu'il n'y a plus de notes réapparaît... Logique !
* L'affichage des listes déroulantes du `Menu A` a été amélioré.
* Amélioration des performances en désactivant la mise à jour automatique des informations sur le curseur dans le code, et autre, du panneau en pied page lorsque celles-ci ne sont pas visibles.
* Lorsque vous ouvrez un fichier censé appliquer un thème (une colorisation du code) donné dans l'URL, si ce thème n'existe pas ou est incorrecte (pour l'une ou l'autre raison), JdBEdit appliquera le thème par défaut ou le thème que vous avez défini dans les paramètres.
* Créer un nouveau fichier est devenu plus facile même avec un autre fichier ouvert. Il suffit de cliquer sur `Nouveau` dans l'onglet `Fichier` du `Menu A` ou avec la combinaison des touches `Ctrl` + `Alt` + `N`. Ensuite, la page s'actualise et un nouveau fichier commence.
* Le tableau de l'historique des fichiers ouverts n'est plus masqué lors de la suppression d'un élément de ce tableau.
* Amélioration de la mise à jour du paramètre URL `select` lors de la sélection du code.
* En important votre historique des fichiers ouverts/dupliqués/supprimés, les caractères avec accent sont dérsomais bien encodés. Plus des carrés ou des points d'interrogation au lieu d'un "é" dans le fichier JSON.
* Et toujours dans l'historique, vous pouvez importer votre sauvegarde tout en profitant d'une fusion sans fail de votre sauvegarde et de l'historique existant.

![](<../.gitbook/assets/image (6).png>)

* Maintenant lorsque vous quittez JdBEdit sans avoir sauvegardé vos modifications et sans fermer l'onglet ou la fenêtre, le message d'alerte qui s'affichait tout de suite à la place du titre de l'onglet ne s'affiche plus que 3 secondes après votre départ.
* Envoyer un [formulaire de contact](https://code.wetrafa.xyz/contact) n'ouvre plus de nouvel onglet, et confirmer le code reCAPTCHA n'envoie plus systématiquement le formulaire.
* Quelques fautes de frappes ont aussi été corrigés.

### Fixation de bugs <a href="#fixation-de-bugs-v-2-13-0" id="fixation-de-bugs-v-2-13-0"></a>

* Correction de la suppression d'un élément de l'historique de fichiers ouverts/dupliqués/supprimés (avant, lors de la suppression d'un élément dans l'historique, le mauvais élément était supprimé au lieu de l'élément sur lequel on a cliqué, et la liste n'était pas mise à jour correctement).
* Quelques dysfonctionnements dans le centre des notifications ont été fixés.
* Correction du dysfonctionnements du paramètre `stacked` dans l'URL (pour l'orientation verticale ou horizontale des cadres Code - Aperçu) lors de l'ouverture d'un fichier Gist.
* Le paramètre de lecture seul a été fixé dans les [Paramètres](https://code.wetrafa.xyz/?modal=setting).

### Suppression de fonctionnalités <a href="#suppression-de-fonctionnalites-v-2-13-0" id="suppression-de-fonctionnalites-v-2-13-0"></a>

* La fonction d'importation d'un pen CodePen a été retirée pour certaines raisons par rapport aux autorisations d'accès de CodePen.
* Suppression du panneau de dialogue CodeMirror pour les notes ou listes des tâches. Utilisez [Notes](https://code.wetrafa.xyz/?modal=notes) à la place, pour une meilleure organisation.
* Suppression de l'outil de compresse du code JavaScript JS Closure.
* Suppression de certaines méthodes dépréciées.

Voilà tout. Enjoy !

## 07-11-2020 - v2.12.3

### Fixation de bugs <a href="#fixation-de-bugs-v-2-12-3" id="fixation-de-bugs-v-2-12-3"></a>

* Lors du chargement d'un seul fichier dans l'éditeur, JdBEdit utilise ce nom de fichier comme nom de fichier JdBEdit s'il n'y a pas déjà un nom de fichier.
* La plage de sélection de textes dans l'URL fonctionne désormais correctement. (Avant lorsqu'on supprimais une sélection, sa plage ne se supprimais pas l'URL.)

## 18-10-2020 - v2.12.0

### Nouveautés <a href="#nouveautes-v-2-12-0" id="nouveautes-v-2-12-0"></a>

* Lorsque le paramètre `theme` est dans l'URL avec une valeur valable, JdBEdit privilégie ce thème  indiqué dans l'URL.
* Nouveau bouton permettant d'insérer une ligne horizontal dans le code HTML et Markdown.

## 08-10-2020 - v2.11.0

### Fixation de bugs <a href="#fixation-de-bugs-v-2-11-0" id="fixation-de-bugs-v-2-11-0"></a>

* Correction de fautes de frappe.
* Correction de l'ouverture du formulaire de contact via le Menu B.

### Nouveautés <a href="#nouveautes-v-2-11-0" id="nouveautes-v-2-11-0"></a>

* A l'aide du bouton permettant d'insérer un modèle de tableau ajouté dans la [version précédente](https://docs.code.wetrafa.xyz/note-de-publication#22-09-2020-v-2-9-0), il est désormais possible de créer un tableau et de le personnaliser en indiquant le nombre de colonnes et de lignes que vous souhaitez pour votre tableau.
* Ajout de suivis d'actions majeures.
* Amélioration de l'interface de connexion avec le jeton d'accès GitHub.

## 06-10-2020 - v2.10.0

### Nouveautés <a href="#nouveautes-v-2-10-0" id="nouveautes-v-2-10-0"></a>

Dans le [sélecteur de couleur](https://code.wetrafa.xyz/?modal=colorPicker), lorsque vous rentrez une couleur valide manuellement dans le champ de texte, cette couleur est automatiquement ajoutée à la liste de couleurs sélectionnées.

## 22-09-2020 - v2.9.0

### Fixation d'un bug <a href="#fixation-dun-bug-v-2-9-0" id="fixation-dun-bug-v-2-9-0"></a>

* Fixer le bug qui bloquait la sauvegarde de fichiers lorsqu'on se connecte via le SSO (on n'était pas considéré comme connecté pour pouvoir achever la sauvegarde).

### Nouveautés <a href="#nouveautes-v-2-9-0" id="nouveautes-v-2-9-0"></a>

* Ajout d'un bouton permettant d'insérer un modèle de tableau à votre code via la barre de touches. Il est désormais possible d'ajouter un modèle de tableau HTML ou Markdown à votre code.

## 14-09-2020 - v2.8.2

### Fixation de bugs <a href="#fixation-de-bugs-v-2-8-2" id="fixation-de-bugs-v-2-8-2"></a>

Petite fixation du paramètre de cassage de ligne.

## 28-08-2020 - v2.8.1

### Fixation de bugs <a href="#fixation-de-bugs-v-2-8-1" id="fixation-de-bugs-v-2-8-1"></a>

* Correction de l'ajout du modèle de style dans l'aperçu du fichier markdown.

## 22-08-2020 - v2.8.0

### Fixation de bugs et améliorations <a href="#fixation-de-bugs-et-ameliorations-v-2-8-0" id="fixation-de-bugs-et-ameliorations-v-2-8-0"></a>

* Correction d'un problème où la position de défilement pouvait sauter lors d'un clic sur une sélection dans Chrome.
* Correction d'un bug où la mise en page de l'éditeur pouvait rester confuse après un appel à rafraîchir lorsque l'option **retour à la ligne** était activée.
* Bloque la fermeture de la boîte de dialogue lorsque l'éditeur perd le focus.
* Désactive la mise en évidence lorsque l'éditeur n'a pas le focus.
* Mise à jour de **CodeMirror** de la version `5.22.2` à `5.57.0`

## 06-08-2020 - v2.7.0

### Fixation de bugs et améliorations <a href="#fixation-de-bugs-et-ameliorations-v-2-7-0" id="fixation-de-bugs-et-ameliorations-v-2-7-0"></a>

* Les notes peuvent à nouveau être supprimée individuellement.

### Nouveautés <a href="#nouveautes-v-2-7-0" id="nouveautes-v-2-7-0"></a>

Plus d'options sont ajoutées dans le panneau de partage pour un partage plus personnalisé :

* Lecture seule
* Inclure la sélection&#x20;
* Afficher le code en pleine page

## 29-07-2020 - v2.6.1

### Fixation de bugs et améliorations diverses <a href="#fixation-de-bugs-et-ameliorations-diverses-v-2-6-1" id="fixation-de-bugs-et-ameliorations-diverses-v-2-6-1"></a>

Pas grand chose à mentionner.

## 07-06-2020 - v2.6.0

### Fixation de bugs et améliorations <a href="#fixation-de-bugs-et-ameliorations-v-2-6-0" id="fixation-de-bugs-et-ameliorations-v-2-6-0"></a>

* Le champ de code est correctement mis en Pleine page lorsque ce mode est activé.
* Curseur mis sur pointeur lorsque vous survolez un lien dans l'aperçu d'un fichier JSON.
* Les librairies ont été mis à jour pour l'ajout rapide dans le panneau Recherche des librairies ([libraries](https://code.wetrafa.xyz/?modal=libraries)).
* Améliorations diverses

### Nouveautés <a href="#nouveautes-v-2-6-0" id="nouveautes-v-2-6-0"></a>

* Nouvelle interface du panneau Extraits de code ([addTo](https://code.wetrafa.xyz/?modal=addTo)).
* Certains éléments du panneau Paramètres ont été réorganisés.
* La navigation dans l'historique de modifications est désormais accessible via la barre de touches juste au dessus de votre code.
* [**Notes**](https://code.wetrafa.xyz/?modal=notes) :&#x20;
  * Ajout de la date de création/dernière modification d'une note.
  * Vous pouvez réorganiser les notes à votre guise.
  * Plus besoin de développer chaque note pour la modifier ou la supprimer, car vous pouvez désormais les faire tout en gardant les notes réduites.

## 08-05-2020 - v2.5.0

### Fixation de bugs et améliorations <a href="#fixation-de-bugs-et-ameliorations-v-2-5-0" id="fixation-de-bugs-et-ameliorations-v-2-5-0"></a>

* La mise en commentaire du texte dans différents langages pris en charge est désormais stable.
* Un délai de 5 secondes vous est accordé pour annuler la suppression d'un gist ou d'un brouillon avant qu'il disparaisse définitivement.
* Améliorations diverses

### Nouveautés <a href="#nouveautes-v-2-5-0" id="nouveautes-v-2-5-0"></a>

* Les formats YAML et TOML sont désormais pris en charge. Vous pouvez maintenant éditer vos fichiers de paramètres en toutes tranquillité. Le HTML, Markdown, SVG, JSON et Texte brut (et JS, CSS, TOML, YAML, Python et Java en mode édition uniquement) sont pris en charge.
* Les fermetures involontaires de la page/onglet ne vous feront plus perdre votre travail, car JdBEdit vous en prévient lorsque votre travail n'est pas enregistré.

## 11-04-2020 - v2.4.0

### Fixation de bugs et améliorations <a href="#fixation-de-bugs-et-ameliorations-v-2-4-0" id="fixation-de-bugs-et-ameliorations-v-2-4-0"></a>

* Amélioration de la fonctionnalité pleine page.
* Comme pour l'aperçu du code, il est désormais possible de coder en plein écran.
* Un problème de duplication des gists a été résolu.
* Amélioration des performances.

### Nouveautés <a href="#nouveautes-v-2-4-0" id="nouveautes-v-2-4-0"></a>

* Lors du téléchargement d'un fichier en tant que fichier Word, tous les scripts (s'il y en a) contenus dans le code sont retirés, car Word n’exécute pas JavaScript.
* JdBEdit insère maintenant la plage de sélection dans l'URL pour permettre de pointer une partie spécifique du code lors du partage d'un fichier.
* Il y a désormais une demande de confirmation lorsque vous essayez de dupliquer un gist en l'ouvrant en tant que template afin d'éviter toute perte de données non sauvegardées.

## 07-04-2020 - v2.3.1

### Fixation de bugs mineurs <a href="#fixation-de-bugs-mineurs-v-2-3-1" id="fixation-de-bugs-mineurs-v-2-3-1"></a>

* On peut désormais de nouveau  ouvrir le code normalement sur CodePen.

### Améliorations <a href="#ameliorations-v-2-3-1" id="ameliorations-v-2-3-1"></a>

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

### Fixation de bugs mineurs et majeurs <a href="#fixation-de-bugs-mineurs-et-majeurs-v-2-3-0" id="fixation-de-bugs-mineurs-et-majeurs-v-2-3-0"></a>

* Ajour du paramètre URL lors de l'ouverture de dernier fichier ouvert.

### Améliorations <a href="#ameliorations-v-2-3-0" id="ameliorations-v-2-3-0"></a>

* Amélioration du fonctionnement d'autres paramètres URL.
* Amélioration de la fonctionnalité **Aller à la ligne** : Nouveau style + atteinte instantanée de la ligne sélectionnée.
* JdBEdit propose de rouvrir le fichier Gist ouvert en dernier si celui-ci n'a pas été supprimé via le navigateur utilisé.

**jdb.js** :

* `v1.24.1` → `v1.24.2`
* Meilleur description du code
* Réduction de taille du fichier
* Suppression de fonctions :&#x20;
  * `jdb.head`
  * `jdb.body`
  * `jdb.goBack`
  * `jdb.noBack`
  * `jdb.hide`
  * `jdb.show`
  * `jdb.addEvent`
  * `jdb.addMultipleEvent`

### **Nouveautés** <a href="#nouveautes-v-2-3-0" id="nouveautes-v-2-3-0"></a>

* Nouvelle interface pour enregistrer des notes dans l'éditeur accessible via la barre de menu. De ce fait, l'option **Sauvegarder vos notes actuelles et à venir** a été retirée des paramètres.
* Nouvelles option **Retour à la ligne forcé** dans les paramètres : permet le passage à la ligne du texte lorsque le panneau du code est  redimensionné à une taille plus petite. Désactivé par défaut.
* Nouvelle barre de navigation pour les mises en formes Markdown mais aussi pour le HTML.&#x20;
* Nouveaux raccourcis Emmet pour les classes JdB.CSS :&#x20;
  * `button:jdb`
  * `btn:jdb`

Le paramètre URL `?login=true` est remplacé par la destination `/login` qui redirige vers `?modal=login` Nouvelle page des paramètres URL : [code.wetrafa.xyz/url-parameters](https://code.wetrafa.xyz/url-parameters)

## 28-11-2019 - v2.2.3

* Fixation de bugs mineurs.
* Fixation du bug qui empêchait l'importation du fichier dans l'éditeur.
* Amélioration de performances.
* Amélioration de la possibilité de connexion avec un `acces_token` (jeton d'accès GitHub).
* Amélioration de l'interface du panneau Paramètre JdBEdit.
* Amélioration de notifications qui préviennent qu'un langage n'est pas pris en charge.&#x20;
* Amélioration de l'interface du panneau de connexion qui s'appelle désormais Portail de connexion.
* Suppression du conflit dans la création d'un Gist alors q'un brouillon est ouvert, et vice versa.

## 04-11-2019 - v2.2.2

### Fixation de bugs (Améliorations) : <a href="#fixation-de-bugs-ameliorations-v-2-2-2" id="fixation-de-bugs-ameliorations-v-2-2-2"></a>

* Ajout d'un badge pro pour les comptes GitHub qui ont un accès PRO.
* Il y a désormais un avertissement lorsque vous ouvrez un brouillon alors qu'il y a du code non sauvegardé.
* Il faudra d'abord fermer le Gist ouvert avant d'ouvrir un brouillon.
* Amélioration des moyens de connexion.

## 24-09-2019 - v2.2.1

### Fixation de bugs (Améliorations) : <a href="#fixation-de-bugs-ameliorations-v-2-2-1" id="fixation-de-bugs-ameliorations-v-2-2-1"></a>

* Ajout d'un badge pro pour les comptes GitHub qui ont un accès PRO.
* Vous pouvez à nouveau  rentrer votre code couleur dans le sélecteur de couleur.
* Ajout d'aide pour résoudre les certains problèmes rencontrés dans l"éditeur.

## 21-08-2019 - v2.2.0

### Fixation de bugs (Améliorations) : <a href="#fixation-de-bugs-ameliorations-v-2-2-0" id="fixation-de-bugs-ameliorations-v-2-2-0"></a>

* Retirer le paramètre URL modal lorsque le panneau en question n'est pas affiché ; et le remettre lorsque le panneau est affiché.
* Ajout de plus d'informations sur les types de fichiers pris en charge.
* Fixation d'un bug mineur dans l'historique de fichiers ouverts.
* Possibilité de télécharger en version `.docs` les fichiers HTML, Markdown et Texte brut uniquement.
* Désactivation du panneau d'aperçu améliorée.
* L'éditeur se désactive et devient inutilisable lorsque l'accès aux cookies est interdit.
* Fixer le lien du script `emmet.js`
* Les couleurs sélectionnées sont désormais sauvegardées dans le Selecteur de couleur. Jusqu'à 30 couleurs peuvent êtres sauvegardées.

## 19-08-2019 - v2.1.9

### Fixation de bugs mineurs (Améliorations) : <a href="#fixation-de-bugs-mineurs-ameliorations-v-2-1-9" id="fixation-de-bugs-mineurs-ameliorations-v-2-1-9"></a>

* Correction de quelques fautes de frappe.
* Suppression du bogue lors de l'envoi du formulaire de contact.
* Mise à jour de liens corrompus.
* Correction du bug lors de l'envoi du formulaire de contact.

##
