---
lab:
  title: "Labo\_3.2\_: créer des devis"
---

# Module 3 : gérer les commandes et le catalogue de produits avec Dynamics 365

## Labo pratique 3.2 : créer des devis

### Scénario
En tant qu’analyste des ventes pour l’implémentation Dynamics 365 Sales chez Contoso Coffee, vous souhaitez vous assurer que les vendeurs pourront tirer parti des améliorations du catalogue de produits tout au long du cycle de vie des ventes. Pour vous assurer que la fonctionnalité fonctionne correctement, vous allez tester le processus de création de devis à partir d’une nouvelle opportunité.

À l’issue de ce labo, vous pourrez :
- Créer des opportunités et ajouter des éléments de ligne d’opportunité
- Génèrer un devis à partir d’une opportunité

### Exercice 1 : créer un devis

#### Tâche 1 : ajouter des éléments de ligne de produits
Dans cette tâche, vous allez créer une opportunité et ajouter des éléments de ligne de produits.
1. Accédez à votre application Centre des ventes Dynamics 365.
2. Dans le menu de gauche, dans le groupe Ventes, sélectionnez **Opportunités.**
3. Cliquez sur **+ Nouveau**.
4. Entrez *Intéressé par les accessoires Airpot XL* pour rubrique, puis sélectionnez **Jon Doe** pour contact.
5. Dans l’en-tête d’enregistrement en haut, sélectionnez la **flèche vers le bas** en regard du champ Propriétaire, puis choisissez **Test Coffee Shop, Inc.** pour le compte. Cliquez sur **Enregistrer**.
6. Cliquez sur l’onglet **Produits**.
7. Vous devez sélectionner des tarifs avant de pouvoir ajouter des produits d’opportunité. Sélectionnez **Filtrer directement** pour les tarifs.
8. Sélectionnez **Calculé par le système** pour le revenu.
9. Au-dessus de la sous-grille, cliquez sur **+ Ajouter des produits.**
10. Dans la liste Tous les produits, recherchez **Filtre 6 mois Airpot XL**, entrez *6* pour la quantité, puis sélectionnez **Ajouter.**
11. Recherchez le **module d’extension Airpot XL** dans la liste des produits, entrez *1* pour la quantité, puis sélectionnez **Ajouter.**
12. Recherchez **l’extension de réservoir Airpot XL** dans la liste des produits, entrez *1* pour la quantité et sélectionnez **Ajouter.**
13. Vous verrez que trois produits sont ajoutés. Cliquez sur **Enregistrer**.
14. Double-cliquez sur le produit **Filtre 6 mois Airpot XL**.
15. Recherchez le champ Remise sur la quantité. Vous constaterez qu’il n’y a pas de remise.
16. Définissez la quantité sur *15*, puis cliquez en dehors du champ. La remise est désormais lancée et le champ Remise sur la quantité affiche la valeur de la remise.
17. Cliquez sur **Enregistrer et fermer**.

#### Tâche 2 : créer un devis
Dans cette tâche, vous allez créer un devis à partir de l’opportunité que vous avez créée dans la tâche 1.
1. Ouvrez l’application Hub de Dynamics 365 Sales si elle n’est pas déjà ouverte.
2. Si nécessaire, ouvrez l’opportunité que vous avez créée dans la tâche précédente. Elle sera appelée **Intéressé par les accessoires Airpot XL**.
3. Sélectionnez l’onglet **Devis**.
4. Au-dessus de la sous-grille, cliquez sur **+ Nouveau devis.**
5. Le formulaire Devis s’ouvre et les informations pertinentes sont copiées à partir de l’opportunité.
6. Sur la page du devis Intéressé par les accessoires Airpot XL, examinez la sous-grille Produits et assurez-vous que les produits et leurs quantités correspondent à ce qui est attendu. Vous pouvez modifier les quantités et réduire le prix de chaque article de ligne.
7. Dans la barre de commandes, sélectionnez **Activer le devis**. (Selon la taille de votre navigateur, vous devrez peut-être sélectionner les points de suspension pour afficher cette option.)
8. Cliquez sur le bouton **Exporter au format PDF** situé dans la barre de commandes, puis sélectionnez **Imprimer le devis pour le client.** Cliquez sur **Télécharger**.
9. Ouvrez le document généré et voyez à quoi ressemble le devis.
10. Fermez le fichier PDF.
11. Fermez la fenêtre Exporter au format PDF.

