# Automatiser en 12 semaines : consignes pour Claude

Programme personnel en 12 semaines pour apprendre à automatiser avec l'IA, sous forme d'app web installable sur iPhone. Tout est dans `index.html`, en JavaScript sans bibliothèque.

Données : une seule clé `localStorage`, `autom12_v1`, qui contient tout l'état sous forme JSON. Ne la renomme pas. Si le format de l'état doit évoluer, ajoute des champs avec une valeur par défaut au chargement, sans casser une sauvegarde existante.

## Façon de travailler

- Réponds en français. L'utilisateur n'est pas développeur : explique en mots simples et dis clairement ce qui est fait, testé ou non vérifié.
- Toute l'app tient dans `index.html` : HTML, style et script, sans compilation ni dépendance à installer. Garde ce format, ne crée pas de sous-dossier, n'ajoute pas d'outil de compilation.
- Écris comme le code existant : même langue dans les commentaires, mêmes noms, même style.
- Les données de l'utilisateur ne sont que dans le `localStorage` de son téléphone, sans copie ailleurs. Ne renomme jamais une clé et ne change jamais le format d'une donnée existante ; tu peux seulement en ajouter.
- L'utilisateur se sert surtout d'un iPhone : tout doit marcher à 375 px de large, avec des zones tactiles confortables. Pour un nombre, le clavier numérique de l'iPhone n'a ni « − » ni « : ».

## Avant d'envoyer

- Vérifie que le script se lit sans erreur : extrais le contenu du `<script>` et lance `node --check` dessus.
- Si tu peux ouvrir un navigateur, teste au format téléphone (375 × 812) : la page s'affiche sans erreur dans la console et rien ne déborde sur le côté.
- La publication suit la branche `main`. Si tu travailles sur une autre branche, dis à l'utilisateur qu'il faut fusionner pour mettre en ligne, et propose de le faire.
