---
lab:
  title: "Labo\_2.1\_: gérer les prospects et les opportunités"
---

# Module 2 : Gérer les prospects et les opportunités avec Dynamics 365 Sales

## Labo pratique 2.1 - Gérer les prospects et les opportunités

### Scénario
Contoso Coffee envisage d’utiliser Dynamics 365 Sales pour formaliser son processus de vente et traiter un backlog de prospects inexploités qui ont été importés par l’équipe marketing à partir de salons commerciaux et de campagnes. En tant qu’analyste des ventes chez Contoso Coffee, vous avez été invité à évaluer et à mettre à jour les enregistrements des prospects pour vous assurer que l’équipe de direction travaille à partir d’un rapport de pipeline rigoureux lors de leur prochaine réunion.

À l’issue de ce labo, vous pourrez :
- Créer et mettre à jour des enregistrements de prospects
- qualifier et disqualifier des prospects.
- Réactiver des enregistrements de prospects

### Exercice 1 : gérer les clients

#### Tâche 1 : création de prospects
Dans cette tâche, vous allez créer trois prospects, un sans informations sur la société et deux avec informations sur la société.
1. Accédez à votre application Centre des ventes Dynamics 365. Assurez-vous de vous trouver dans la zone Ventes ; si ce n’est pas le cas, utilisez le menu déroulant inférieur gauche pour y accéder.
2. Dans le volet de navigation de gauche, sélectionnez **Prospects** sous le groupe Ventes.
3. Dans le volet Éléments de travail, sélectionnez **Grille en lecture seule** pour modifier le type de vue.
4. Dans le menu qui s’affiche, sélectionnez le bouton **+ Nouveau**.
5. Entrez *Prospect machine à café sans société* pour Rubrique, *Jane* pour Prénom, *Doe* pour Nom.
6. Acceptez la suggestion **Responsable de la cafétéria** qui a été renseignée dans le champ Fonction.
7. Sélectionnez le bouton **Enregistrer**. Dans la barre de commandes du haut, sélectionnez encore **+ Nouveau**.
8. Entrez *Prospect machine à café avec société* pour Rubrique, *Jon* pour Prénom, *Doe* pour Nom, *Doe Inc.* pour Société, puis cliquez sur **Enregistrer**.
9. Dans la barre de commandes, cliquez sur le bouton **+ Nouveau** encore une fois.
10. Entrez *Autre prospect machine à café* pour Rubrique, *Jack* pour Prénom, *Rogers* pour Nom, *Test Coffee Shop, Inc.* pour Société, puis cliquez sur **Enregistrer**.

### Exercice 2 : qualification des prospects
Dans cet exercice, vous allez qualifier/disqualifier les prospects et voir quels enregistrements sont créés lors du processus de qualification.

#### Tâche 1 : qualifier le prospect machine à café sans informations sur la société
1. Accédez à votre application Centre des ventes.
2. Sélectionnez **Prospects**.
3. Dans le volet Éléments de travail, cliquez sur le bouton **Grille en lecture seule**.
4. Recherchez **Prospect machine à café sans société** et sélectionnez-le.
5. Cliquez sur **Qualifier** dans le menu supérieur.
6. Le prospect sera qualifié dans un nouvel enregistrement Opportunité.
   - **REMARQUE :** si la nouvelle opportunité ne s’ouvre pas automatiquement, sélectionnez Opportunités dans le menu de gauche pour afficher toutes les opportunités ouvertes. Ouvrez ensuite l’opportunité Prospect machine à café sans société.
7. Recherchez le champ Contact. Vous constaterez que Jane Doe est maintenant un enregistrement Contact dans l’application et que vous pouvez l’ouvrir.
8. Recherchez le champ Compte (dans l’en-tête de l’enregistrement d’opportunité). Notez que le champ est vide.
9. Cliquez sur **Enregistrer**.

#### Tâche 2 : qualifier le prospect machine à café avec société
1. Accédez à votre application Centre des ventes.
2. Sélectionnez **Prospects**.
3. Recherchez Prospect machine à café avec société et ouvrez-le.
4. Cliquez sur **Qualifier** dans le menu supérieur.
5. Le prospect est qualifié comme le prospect précédent, et vous êtes dirigé vers l’enregistrement Opportunité nouvellement créé à partir du prospect qualifié.
6. Recherchez le champ Contact. Vous constaterez que Jon Doe est maintenant un enregistrement Contact.
7. Recherchez le champ Compte. Vous constaterez que Doe, Inc. est maintenant un enregistrement de compte.

#### Tâche 3 : disqualifier un prospect
1. Si nécessaire, accédez à votre application Centre des ventes.
2. Sélectionnez **Prospects**.
3. Localisez le prospect d’autre machine à café et ouvrez-le.
4. Cliquez sur **Disqualifier** (vous devrez peut-être sélectionner le bouton de points de suspension verticaux pour qu’il s’affiche).
5. Dans le menu qui apparaît, sélectionnez **Plus intéressé**.
6. Le prospect est disqualifié, le statut passe à Plus intéressé et l’enregistrement devient en lecture seule.

#### Tâche 4 : réactiver un prospect
1. Si nécessaire, accédez à votre application Centre des ventes.
2. Dans la navigation du site, sous le groupe Ventes, sélectionnez **Prospects.**
3. Le prospect que vous avez disqualifié n’est plus dans la vue Mes prospects ouverts. Sélectionnez la flèche vers le bas en regard de Mes prospects ouverts et modifiez la vue en **Prospects fermés.**
4. Localisez le prospect d’autre machine à café et ouvrez-le.
5. Cliquez sur **Réactiver le prospect**.
6. Le prospect est réactivé, le statut repasse à Nouveau et l’enregistrement devient modifiable.

### Exercice 3 : utiliser des opportunités
Dans cet exercice, vous allez parcourir le processus d’utilisation d’une opportunité à travers le processus de vente.

#### Tâche 1 : gérer le prospect de la machine à café avec l’entreprise
1. Si nécessaire, accédez à votre application Centre des ventes.
2. Dans la barre de navigation à gauche, sélectionnez **Opportunités** sous le Groupe de ventes.
3. Localisez et ouvrez l’opportunité **Prospect de machine à café avec l’entreprise**.
4. Dans le volet Opportunité qui s’affiche, sélectionnez le bouton **Accéder à la page principale** (situé en regard du bouton X [Fermer]).
5. Remplissez les informations sur l’opportunité comme suit :
   - Montant budgété : 17 000 $
   - Délai d’achat : ce trimestre
   - Procédure d’achat : Comité
   - Description : volonté de mise à niveau de leurs machines à café actuelles à plusieurs emplacements.
6. Développez l’en-tête d’enregistrement en haut et remplissez les informations comme suit :
   - Disponibilité Date de clôture : saisissez la date de demain.
   - Disponibilité chiffre d’affaires : 16 500 $
7. Dans la Chronologie, sélectionnez **+** (ajouter un enregistrement de chronologie).
8. Dans le menu qui s’affiche, sélectionnez **Appel téléphonique**.
9. Complétez l’appel téléphonique comme suit :
   - Objet : premier appel de Jon.
   - Délai : saisissez la date d’aujourd’hui à 16h30.
10. Sélectionnez le bouton **Enregistrer et fermer**.
11. Alors que l’opportunité est ouverte, sélectionnez la **phase Développer** dans le flux des processus d’entreprise Prospect-opportunité. Procédez comme suit :
   - Besoin du client : volonté de mise à niveau de ses machines à café à plusieurs emplacements.
   - Solution proposée : recommandation de plusieurs machines AirPot Duo.
   - Identifier les parties prenantes : terminé
   - Identifier les concurrents : terminé
12. Sélectionnez le bouton **Phase suivante**.
13. Dans la phase Proposer, définissez tous les champs sur **Terminé**.
14. Sélectionnez le bouton **Phase suivante**.
15. Sélectionnez n’importe où en dehors de la phase de processus d’entreprise pour la fermer.
16. Dans la section Assistant, sous Notifications, sélectionnez l’élément **Appel téléphonique** que vous avez créé précédemment pour l’ouvrir.
17. Sélectionnez **Terminer**. (Notez que l’élément disparaît de vos notifications.)
18. Dans le processus de vente Prospect-opportunité, sélectionnez la **phase de clôture**.
19. Marquez tous les éléments de la phase de clôture comme **Terminé.**
20. Sélectionnez le bouton **Terminer**.
21. Dans la barre de commandes affichée en haut de l'écran, sélectionnez le bouton **Clôturer comme conclu**.
22. Dans l’écran Fermer l’opportunité, sélectionnez le bouton **OK**.

Félicitations, vous avez créé et géré des prospects et des opportunités dans Dynamics 365 Sales.
