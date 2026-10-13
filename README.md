
THÈME : concevoir une application de vente de mode, beauté et hygiène avec ChatGPT, Gemini et Figma

 Introduction

En tant que développeuse responsable d’une équipe full stack, je dois transformer le besoin du client en une application utilisable, fiable et maintenable. ChatGPT, Gemini et Figma peuvent accélérer certaines étapes, mais ils ne remplacent ni les échanges avec le client, ni les tests auprès des utilisateurs, ni la vérification du code. "La responsabilité de ce qui est intégré dans l’application reste celle de l’équipe de développement."

L’application doit permettre de vendre des vêtements, chaussures, sacs, produits de beauté et d’hygiène, soins capillaires et perruques pour femmes et hommes. Elle peut être consultée par des personnes de 14 à 45 ans, mais je distingue les "acheteurs adultes visés en priorité" des utilisateurs mineurs. Les contenus, la collecte de données et les achats concernant les mineurs doivent être encadrés ; les publicités ne doivent pas les mettre en avant sans vérification des règles applicables.

Pour cadrer le projet, je pars sur une "boutique en ligne pour un seul commerçant", et non une marketplace avec plusieurs vendeurs. Cela permet de limiter la première version à un catalogue, un stock, un processus de commande et une organisation de livraison. Si le client veut accueillir plusieurs vendeurs, je lui explique que cela change fortement le périmètre : il faudra gérer leurs comptes, leurs catalogues, les commissions, les paiements et les litiges.

1. Première réunion avec le client

Je commence par comprendre le commerce et ses problèmes actuels. Je demande comment le client présente ses produits, suit son stock, reçoit les commandes, confirme les paiements et organise les livraisons. Je clarifie aussi qui mettra à jour le catalogue, qui répondra aux clients et quel budget est prévu pour le développement et la maintenance.

Je ne suppose pas que les clients ont tous les mêmes habitudes à Pointe-Noire. Je demande quels moyens de commande, de paiement et de livraison le commerçant utilise réellement, et quels appareils ses clients ont l’habitude d’utiliser.

- À ChatGPT :préparer un guide de questions et organiser mes notes.
- À Gemini : relire le compte rendu et relever les points encore flous.
- Je vérifie moi-même :que le compte rendu correspond aux réponses du client et que les besoins sont séparés de mes idées.
- Risques :l’IA peut mal résumer la réunion ou proposer des fonctionnalités hors budget.
- Critère pour continuer : le client valide le problème à résoudre, le public visé, les contraintes et le périmètre envisagé.

2. Étude du marché et des futurs utilisateurs

Je regarde les offres concurrentes, leurs catégories, leurs fiches produit, leurs prix affichés, leurs moyens de contact et leurs informations sur la livraison et les retours. Les sites concurrents sont des indices utiles, mais leurs propres affirmations ne suffisent pas à prouver la qualité de leur service. Si possible, je vérifie certains éléments en contactant le vendeur ou en testant le parcours d’achat.

Je parle aussi à quelques clients potentiels. Je leur demande comment ils choisissent une taille ou une teinte, quelles informations leur manquent avant d’acheter et ce qui les rassurerait. Pour les produits intimes, je pose des questions avec discrétion et sans demander de détails personnels inutiles.

- À ChatGPT :préparer des questions neutres pour les entretiens et classer des notes anonymisées.
- À Gemini : proposer une liste de points à comparer entre les offres observées.
- Je vérifie moi-même :chaque observation auprès de sa source et je ne généralise pas à toute la population à partir de quelques personnes.
- Risques : copier les concurrents ou confondre un compliment avec une vraie intention d’achat.
- Critère pour continuer : je comprends mieux les besoins des clients et je peux formuler un avantage potentiel à tester, sans prétendre qu’il est déjà prouvé.

3. Définition de la première version et du catalogue

Je limite la première version au parcours essentiel : trouver un produit, comprendre ses caractéristiques, choisir une variante, ajouter l’article au panier, renseigner la livraison, choisir un moyen de paiement proposé par le commerçant et recevoir une confirmation claire.

Je définis les informations nécessaires selon le type de produit :

- Vêtements et chaussures : tailles, pointures, couleurs, disponibilité et guide des tailles si le commerçant peut le fournir.
- Sacs : dimensions, matières, couleurs et photos fidèles à l’article vendu.
- Produits de beauté et d’hygiène : contenance, ingrédients ou informations du fabricant quand elles sont disponibles, précautions d’utilisation fournies par la marque.
- Perruques et soins capillaires : longueur, couleur, texture ou autres variantes réellement proposées.
- Produits intimes : présentation sobre, commande discrète et collecte minimale d’informations personnelles.

Je demande au client d’indiquer les prix, le stock, les frais de livraison, les délais, les coordonnées de contact et les conditions applicables aux retours. Je ne rédige pas moi-même une politique de remboursement sans validation du client et vérification des règles applicables.

- À ChatGPT :convertir les besoins en parcours utilisateur et critères d’acceptation.
- À Gemini :relever des cas à prévoir, comme une taille épuisée ou un article retiré du panier.
- Je vérifie moi-même : que les données et règles viennent du commerçant et correspondent au fonctionnement de la boutique.
- Risques : afficher une mauvaise taille, un stock périmé, une composition non vérifiée ou une promesse de livraison impossible.
- Critère pour continuer : le commerçant peut fournir des informations fiables et désigne la personne qui tiendra le catalogue à jour.

 4. Conception et test dans Figma

Je dessine dans Figma les écrans principaux : accueil, catégories, recherche, filtres, fiche produit, panier, validation de commande et suivi. Je prévois également les situations d’erreur : produit indisponible, variante épuisée, panier vide, attente de confirmation ou problème de connexion.

Je fais tester le prototype à quelques personnes en leur donnant une tâche concrète, par exemple : « Trouvez une paire de chaussures de votre pointure et ajoutez-la au panier ». Je les observe sans les guider afin de voir si les informations et les actions sont compréhensibles.

- À ChatGPT :proposer des textes de boutons ou des messages d’erreur plus clairs.
- À Gemini : relire le parcours à partir d’une description ou de captures expurgées de données privées.
- Je vérifie moi-même : la lisibilité, la cohérence du parcours et les retours des personnes qui essaient le prototype.
- Risques : obtenir une maquette esthétique mais difficile à utiliser ou tester uniquement avec des proches ayant les mêmes habitudes que moi.
- Critère pour continuer :les personnes testées arrivent à trouver un produit et à comprendre les prochaines étapes sans assistance constante.

 5. Préparation technique et développement des composants front-end

Avant de coder, je définis avec l’équipe le découpage des composants : cartes produit, filtres, sélecteur de taille ou de couleur, panier, formulaire de commande et messages de confirmation ou d’erreur. Je m’accorde avec les développeurs back-end sur les données reçues et envoyées.

Je veille notamment à ce qu’une commande « reçue » ne soit pas affichée comme « confirmée » tant que le serveur n’a pas réellement confirmé son statut. Je prévois aussi une manière visible de signaler une indisponibilité ou une erreur.

- À ChatGPT  proposer un squelette de composant ou expliquer une erreur à partir d’un exemple non confidentiel.
- À Gemini : faire une première revue du code ou proposer des cas à vérifier.
- Je vérifie moi-même : le code dans le projet, ses dépendances, les données utilisées, les règles métier et l’affichage sur les écrans ciblés.
- Risques : intégrer du code généré sans le comprendre, afficher un faux stock ou une fausse confirmation, ou transmettre des données sensibles à l’IA.
- Critère d’intégration :le composant correspond à la maquette validée, respecte les règles et données convenues et a été relu par un autre membre de l’équipe.

6. Vérifications et livraison

Avant la livraison, l’équipe vérifie le parcours avec les différentes situations prévues : choix d’une variante, indisponibilité d’un article, erreur dans le formulaire, commande reçue et réponse du serveur. Nous comparons le rendu à Figma et vérifions l’affichage sur les écrans prévus pour le projet.

Je remets les composants front-end, la référence Figma, les instructions de lancement et les échanges attendus avec le back-end. Je précise ce qui est terminé, ce qui reste à faire et les limites connues. Les frais et délais annoncés, les coordonnées du vendeur, les conditions de commande et les informations de retour doivent être validés avant une vraie mise en vente.

- À ChatGPT et Gemini : préparer des scénarios de vérification et un brouillon de documentation.
- Je vérifie moi-même : le résultat dans l’application, les données affichées, les erreurs et la conformité du livrable aux critères convenus.
- Risques :livrer une maquette qui n’est pas connectée aux vraies données, ou cacher une règle commerciale encore indécise.
- Critère de livraison : un autre développeur peut lancer et comprendre les composants ; le client peut suivre une commande de démonstration et confirmer que le périmètre livré est celui qui a été convenu.

 Conclusion

Pour ce projet, une bonne application ne se résume pas à afficher beaucoup de produits. L’acheteur doit pouvoir comprendre ce qu’il achète, choisir la bonne variante, voir le prix et les conditions clairement, et savoir ce qu’il advient de sa commande.

ChatGPT et Gemini m’aident à préparer et à relire certaines étapes ; Figma me permet de représenter et tester les parcours. Mais c’est à moi, développeuse responsable, de vérifier les propositions, les règles métier et le code. Je n’intègre une proposition que si elle répond au besoin du client, est comprise par les utilisateurs testés et fonctionne avec des informations commerciales fiables.



Rédige un devoir complet et bien structuré en français à partir du sujet suivant :

« Vous êtes développeuse responsable d’une équipe full stack. Votre entreprise vous demande de concevoir une application de vente de vêtements, chaussures, sacs, produits de beauté et d’hygiène corporelle, produits intimes, soins capillaires et perruques pour femmes et hommes. Décrivez précisément votre méthode de travail, de la première réunion avec le client jusqu’à la livraison des composants front-end. Pour chaque étape, expliquez ce que vous confiez à ChatGPT et Gemini, comment vous utilisez Figma, ce que vous vérifiez vous-même, les risques possibles et les critères qui permettent de décider qu’une proposition peut être intégrée à l’application. »

### Contexte

- Je suis étudiante en première année de Full Stack et Data et j’habite à Pointe-Noire, en République du Congo.
- Le public potentiel va de 14 à 45 ans, femmes et hommes. Explique pourquoi cette tranche est large et distingue les besoins des différents groupes sans présenter les 14–45 ans comme un public homogène.
- Prends en compte la présence de mineurs avec prudence. Ne prétends pas connaître les règles juridiques applicables sans les vérifier auprès d’une source fiable.
- Pour cadrer le projet, pars sur une boutique en ligne pour un seul commerçant. Explique brièvement qu’une marketplace avec plusieurs vendeurs demanderait davantage de fonctionnalités et de travail.
- Traite comme des éléments à vérifier auprès du client et des utilisateurs les stocks, les prix en FCFA, les tailles et variantes, les photos, les moyens de paiement, la livraison, les retours, les téléphones utilisés et les conditions de connexion.
- Présente les produits intimes avec respect et discrétion. Pour les produits de beauté et d’hygiène, n’invente ni ingrédients ni promesses médicales.
- Adapte les exemples à Pointe-Noire, mais ne transforme pas des suppositions sur la ville en faits. Indique comment les vérifier sur le terrain.


PROMPT:

Méthode et responsabilités

Décris les étapes dans l’ordre, depuis la réunion initiale jusqu’à la remise du front-end. Pour chacune, présente clairement :

1. Les actions de la développeuse et de l’équipe.
2. Ce que ChatGPT peut aider à préparer ou produire.
3. Ce que Gemini peut aider à relire ou à proposer.
4. Comment Figma sert à organiser les écrans, les composants et le prototype.
5. Les vérifications humaines nécessaires.
6. Les risques possibles.
7. Les critères concrets pour valider l’étape et passer à la suivante.

Ne présente pas Figma comme une IA automatiquement capable de tout concevoir. Ne présente pas le code produit par ChatGPT ou Gemini comme prêt à intégrer sans lecture, adaptation et vérification par la développeuse. N’invente pas d’entretiens, de tests, de résultats, de statistiques, de clients intéressés ou de partenariats : décris plutôt comment les obtenir et les vérifier.

Format souhaité

- Écris à la première personne, dans le rôle de la développeuse responsable du projet, avec un ton professionnel, naturel et accessible à une étudiante de première année.
- Organise le devoir avec un titre, une introduction, des étapes numérotées et une conclusion.
- Vise environ 1 200 à 1 600 mots.
- Fais ressortir les décisions concrètes du projet : périmètre de la première version, parcours d’achat, données du catalogue, composants front-end, tests, critères de livraison et documentation.
- Si tu mentionnes des concurrents ou des règles juridiques, vérifie les informations avec des sources fiables et ajoute des liens. Distingue les faits vérifiés des hypothèses et des affirmations publiées par les entreprises elles-mêmes.
- Termine en rappelant que les IA assistent le travail, mais que la développeuse reste responsable des décisions techniques, des vérifications et du code livré.
