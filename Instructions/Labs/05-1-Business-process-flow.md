---
lab:
  title: "Labo\_5.1\_: personnaliser un flux des processus d’entreprise"
---

# Module 5 : utiliser Dynamics 365 Sales Insights et l’accélérateur des ventes 

## Labo pratique 5.1 : personnaliser un flux de processus métier

## Scénario

Contoso Coffee cherche à ajouter quelques étapes supplémentaires à son processus d’entreprise testé et approuvé. Bien que les vendeurs aient réussi à suivre ce cadre par le passé, ils signalent que quelques nouvelles suggestions aideraient à alimenter les prospects et à conclure des contrats à valeur élevée.

Les vendeurs souhaitent ajouter les étapes suivantes à leur processus d’entreprise :

-   Pour les clients potentiels à valeur élevée avec un budget de plus de 1 000 000 \$, contacter les prospects personnellement pour confirmer leur intérêt avant de passer à la qualification.
-   Au cours de l’étape de développement, s’assurer que les vendeurs effectuent le suivi des points sensibles des clients existants, afin d’identifier les zones potentielles de ventes supplémentaires qui auraient pu être manquées précédemment.

Dans ce labo, nous allons personnaliser le flux de processus métier pour répondre aux demandes de nos vendeurs.

## Exercice 1 : personnaliser le flux de processus métier

### Tâche 1 : créer un flux de processus métier

Dans cette tâche, vous allez créer un flux de processus métier à partir du processus de vente opportunité, puis tester le nouveau flux.

1.  Accédez à [https://make.powerapps.com](https://make.powerapps.com/).
2.  Vérifiez que vous êtes dans l’environnement **Évaluation des ventes**.
3.  Cliquez sur **Solutions**.
4.  Dans la barre de commandes en haut, cliquez sur le bouton **+ Nouvelle solution**.
5.  Dans le champ **Nom d’affichage**, entrez **Contoso**.
6.  Sélectionnez **+ Nouvel éditeur**.
7.  Configurez le nouvel éditeur comme suit :
    1.  **Nom complet :** Contoso
    2.  **Nom :** Contoso
    3.  **Préfixe :** Contoso
    4.  **Préfixe de valeur de choix :** 1 0000
8.  Cliquez sur **Enregistrer**.
9.  Sous Éditeur, sélectionnez le nouvel éditeur **Contoso** que vous venez de créer.
10. Sélectionnez **Créer**.
11. Dans la **barre de commandes**, sélectionnez **Ajouter**.
12. Dans le menu qui s’affiche, sélectionnez **Processus**\>**Automation**.
13. À présent, recherchons le **processus de vente** dans la liste des processus. Pour cela, placez-vous dans la zone de recherche du coin supérieur. Sélectionnez le processus que vous avez trouvé.
14. Cliquez sur le bouton **Ajouter**.
15. Sélectionnez le **processus de vente** pour l’ouvrir.
16. Un nouvel onglet s’ouvre dans l’éditeur de flux de processus métier. Conservez l’ancien onglet avec la liste Solutions ouverte. Maintenant, ajoutons les étapes demandées par nos vendeurs.
17. Tout d’abord, ajoutons une condition pour vérifier le budget du client et identifier nos clients potentiels à valeur élevée avec des budgets de plus de 1 000 000 \$. Faites glisser **Condition** à partir de l’onglet **Composants** et placez-le entre les étapes **Qualifier** et **Développer**.
18. Sélectionnez la **condition**, accédez à l’onglet **Propriétés**, puis entrez **Vérifier le budget** pour le **nom complet**.
19. Sous **Règles**, sélectionnez le **champ** **Montant budgétaire**.
20. Sélectionnez l’**opérateur** **Est supérieur ou égal à**.
21. Sélectionnez le **type** **Valeur**.
22. Entrez **1 000 000** comme **valeur**, puis cliquez sur **Appliquer**.
23. Nous devons maintenant ajouter une nouvelle étape pour terminer la condition. Dans le volet Composants, ajoutez une nouvelle étape à droite de la condition.
24. Sélectionnez l’onglet **Propriétés**.
25. Entrez **Confirmer l’intérêt** pour le **nom complet**. Sélectionnez **Appliquer**.
26. Cliquez sur le bouton **Détails** de l’étape **Confirmer l’intérêt**.
27. Sélectionnez l’**étape de données \#1 Nouvelle étape** à l’intérieur de l’étape **Confirmer l’intérêt**.
28. Dans l’onglet **Propriétés**, ouvrez la liste déroulante du **champ de données**. Sélectionnez **Confirmer l’intérêt**. Le nom de l’étape est mis à jour automatiquement.
29. Cochez la case **Obligatoire**, puis cliquez sur **Appliquer**.
30. Ensuite, nous allons ajouter une nouvelle étape pour enquêter sur les points sensibles du client dans l’étape Développement, comme demandé par nos vendeurs. Sélectionnez l’étape **Développer** et développez **Détails**.
31. Dans le volet Composants, faites glisser une **étape de données** sous Étape de données\#4.
32. Dans la liste déroulante Champ de données, sélectionnez **Points sensibles du client**. Il s’agit maintenant d’une étape suggérée dans l’étape Développer pour identifier les points sensibles du client. Nous ne marquons pas ce champ comme requis.
33. Sélectionnez **Appliquer**.
34. Cliquez sur **Valider** pour vérifier que les modifications que vous avez apportées sont valides et que le flux de processus métier fonctionne comme prévu.
35. S’il n’y a aucun problème, cliquez sur **Mettre à jour**.
36. Fermez l’onglet avec l’éditeur de flux de processus métier.
37. De retour sous votre onglet précédent, cliquez sur **Terminé** dans la fenêtre contextuelle dans la zone Solution par défaut. Dans le menu supérieur, sélectionnez **Publier toutes les personnalisations**. Vous devrez peut-être supprimer la recherche « opportunité » dans la zone de texte en haut à droite pour pouvoir afficher ce bouton.
38. Attendez la **publication** de vos personnalisations.

### Tâche 2 : tester le flux de processus métier

1.  Revenez à l’application Centre des ventes.
2.  Accédez à la section **Opportunités**, puis cliquez sur **+ Nouveau** pour créer une opportunité. Entrez une rubrique telle que **Intéressés par de nouvelles machines**.
3.  Sélectionnez un contact existant pour le champ de contact.
4.  Ouvrez l’étape **Qualifier** du flux de processus métier Ventes. Entrez *800 000 \$* pour le budget estimé.
5.  Le flux de processus métier doit comporter 4 étapes : **Qualifier**, **Développer**, **Proposer** et **Fermer**. L’étape Confirmer l’intérêt ne fait pas partie du processus si le montant budgétaire est inférieur à 1 000 000 \$.
6.  Passez le **montant du budget** à *1 200 000 \$*.
7.  Le flux de processus métier doit maintenant avoir 5 étapes : **Qualifier**, **Confirmer l’intérêt**, **Développer**, **Proposer** et **Fermer**. Passez de l’étape Qualifier à l’étape suivante.
8.  **Enregistrez** l’opportunité.
9.  Sélectionnez l’étape **Qualifier** et sélectionnez le bouton **Étape suivante** pour passer à l’étape **Confirmer l’intérêt**.
10. Confirmez l’intérêt en sélectionnant **Non**, puis **Oui**.
11. Cliquez sur le bouton **Étape suivante** pour passer à l’étape **Proposer**.
12. Vérifiez que le champ Points sensibles du client s’affiche en bas de l’étape Développer.
13. Entrez *Les machines actuelles ne peuvent pas gérer le volume du client* dans le champ Points sensibles du client.
14. Sélectionnez **Phase suivante**.
15. **Sauvegardez** l’enregistrement.

