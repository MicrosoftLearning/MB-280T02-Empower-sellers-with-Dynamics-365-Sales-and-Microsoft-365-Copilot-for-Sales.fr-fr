---
lab:
  title: "Labo\_3.1\_: configurer le catalogue de produits"
---

# Module 3 : gérer les commandes et le catalogue de produits avec Dynamics 365

## Labo pratique 3.1 : gérer le catalogue de produits

### Scénario
En pleine croissance, Contoso Coffee souhaite normaliser sa structure tarifaire et faciliter la création des devis, des commandes et des factures avec des détails de prix et de produits plus précis. Contoso Coffee a récemment lancé sa nouvelle machine à café intelligente. En tant que consultant fonctionnel pour son implémentation de Dynamics 365 Sales, vous avez été invité à configurer le catalogue de produits.

À l’issue de ce labo, vous pourrez :
- Créer des groupes d’unités
- Définir des tarifs
- Créer des types de remises
- Définir des produits et des familles de produits

### Exercice 1 : catalogue de produits

#### Tâche 1 : créer un groupe d’unités
Dans cette tâche, vous allez créer des groupes d’unités pour une gamme de filtres de machine à café.
1. Accédez à votre application Centre des ventes Dynamics 365.
2. Cliquez dans le menu Changer de zone (situé en bas à gauche de l’écran). Par défaut, Ventes s’affiche en bas du menu de gauche.
3. Dans le menu qui s’affiche, sélectionnez **Paramètres de l’application**.
4. Sélectionnez **Groupes d’unités** dans la section Catalogue de produits du menu de gauche.
5. Cliquez sur **+ Nouveau**.
6. Entrez **Filtres** pour Nom, entrez **Chacun** pour Unité principale, puis cliquez sur **OK**.
7. Une fois le groupe d’unités ouvert, sélectionnez l’onglet Association et choisissez **Unités**.
8. Vous constaterez que vous n’avez pour le moment que l’unité par défaut Chacun ; vous allez ajouter trois unités supplémentaires. Cliquez sur **+ Nouvelle unité**.
9. Entrez <bpt ctype="x-unknown" id="1" rid="1"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">*</bpt></bpt>Filtre<ept id="2" rid="1"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">*</ept></ept> pour Nom, <bpt ctype="x-unknown" id="3" rid="2"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p2">*</bpt></bpt>1<ept id="4" rid="2"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p2">*</ept></ept> pour Quantité, sélectionnez <bpt ctype="x-unknown" id="5" rid="3"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p3">**</bpt></bpt>Chacun<ept id="6" rid="3"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p3">**</ept></ept> pour Unité de base, puis cliquez sur <bpt ctype="x-unknown" id="7" rid="4"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p4">**</bpt></bpt>Enregistrer et créer<ept id="8" rid="4"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p4">**</ept></ept> en sélectionnant l’icône de liste déroulante <bpt ctype="x-unknown" id="9" rid="5"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p5">**</bpt></bpt>˅<ept id="10" rid="5"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p5">**</ept></ept> à droite du bouton Enregistrer et fermer.
10. Entrez *Paquet* pour Nom, *2* pour Quantité, sélectionnez **Filtre** pour Unité de base, puis cliquez sur **Enregistrer et créer**.
11. Entrez *Paquet économique* pour Nom, *2*pour Quantité, sélectionnez **Paquet** pour Unité de base, puis cliquez sur **Enregistrer et fermer**.
12. Vous devez maintenant avoir quatre groupes d’unités dans la liste.

#### Tâche 2 : créer un type de remise
Dans cette tâche, vous allez créer un type de remise pour les personnes qui achètent 15 ou 20 filtres ou plus. Pour 15 filtres, elles bénéficieront d’une remise de 15 % et pour 20 à 50 filtres, elles bénéficieront d’une remise de 25 %.
1. Sélectionnez **Types de remises** dans la section Catalogue de produits du menu de gauche.
2. Cliquez sur **+ Nouveau**.
3. Entrez *Remise sur quantité* pour Nom, sélectionnez **Pourcentage** pour Type, puis cliquez sur **Enregistrer**.
4. Cliquez sur **Association** et choisissez **Remises**.
5. Cliquez sur **+ Nouvelle remise**.
6. Assurez-vous que l’option Remise sur quantité est sélectionnée pour Type de remise, entrez *15* pour Quantité initiale, *19* pour Quantité finale, *15* pour Pourcentage, puis cliquez sur **Enregistrer**.
7. Cliquez à nouveau sur **+ Nouveau**.
8. Sélectionnez **Remise sur quantité** pour Type de remise. Entrez ensuite *20* pour Quantité initiale, *50* pour Quantité finale, entrez *25* pour Pourcentage, puis cliquez sur **Enregistrer**.

#### Tâche 3 : créer un tarif
Dans cette tâche, vous allez créer un tarif pour les filtres.
1. Sélectionnez **Tarifs** dans la section Catalogue de produits du menu de gauche.
2. Cliquez sur **+ Nouveau**.
3. Entrez *Filtre Direct* pour Nom, sélectionnez **US Dollar** pour Devise, puis cliquez sur **Enregistrer et fermer**.

#### Tâche 4 : créer des produits
Dans cette tâche, vous allez créer des produits.
1. Cliquez sur la zone de modification **Paramètres de l’application**.
2. Sélectionnez **Ventes**.
3. Sélectionnez **Produits** dans la section Collatéral du menu de gauche.
4. Cliquez sur **Ajouter un produit**.
5. Entrez *Filtre 6 mois Airpot XL* pour le nom, entrez *AXL6MF-1234* pour l’ID produit, sélectionnez **Filtres** pour le groupe d’unités, sélectionnez **Filtrer** pour l’unité par défaut, entrez *2* pour les décimales prises en charge, puis cliquez sur **Enregistrer.** (Vous devrez peut-être sélectionner la coche bleue en regard des décimales prises en charge pour accepter la suggestion.)
6. Sélectionnez l’onglet **Détails supplémentaires**.
7. Cliquez sur les **points de suspension verticaux** en haut à droite de la section Éléments tarifaires. Cliquez sur **+ Nouvel élément tarifaire**.
8. Sélectionnez **Filtrer directement** pour les tarifs, sélectionnez **Remise de quantité** pour les types de remises, puis sélectionnez **Entier** pour l’option de quantité de vente.
9. Sélectionnez l’onglet **Informations de tarification**, entrez *25* pour le montant, puis sélectionnez **Enregistrer et Fermer.**
10. Si la publication automatique est activée, ignorez cette étape. (La publication n’apparaît pas dans la barre de commandes.) Sinon, sélectionnez **Publier** et **Confirmer** pour publier le produit.
11. Dans le menu de gauche, sélectionnez **Produits** dans le groupe Collatéral.
12. Cliquez sur **Ajouter un produit**.
13. Entrez l’*extension de réservoir Airpot XL* pour le nom, entrez *AXLRE-4321* pour l’ID produit, sélectionnez **Unité par défaut** pour le groupe d’unités, sélectionnez **Unité primaire** pour unité par défaut, cochez la coche bleue en regard de 2 pour les décimales prises en charge, puis cliquez sur **Enregistrer.**
14. Sélectionnez l’onglet **Détails supplémentaires**.
15. Cliquez sur les **points de suspension verticaux** en haut à droite de la section Éléments tarifaires. Cliquez sur **+ Nouvel élément tarifaire**.
16. Sélectionnez **Filtrer directement** pour les tarifs. Sélectionnez **Entier** pour l’option de quantité de vente.
17. Sélectionnez l’onglet **Informations de tarification**, entrez *299 $* pour le montant, puis sélectionnez **Enregistrer et Fermer.**
18. Si la publication automatique est activée, ignorez cette étape. Sinon, sélectionnez **Publier** et **Confirmer** pour publier le produit.
19. Sélectionnez **Produits** dans le menu de gauche.
20. Cliquez sur **Ajouter un produit**.
21. Entrez *Module d’extension Airpot XL* pour le nom, entrez *AXPLE-7894* pour l’ID produit, sélectionnez **Unité par défaut** pour le groupe d’unités, sélectionnez **Unité principale** pour l’unité par défaut, sélectionnez la coche bleue en regard de 2 pour les décimales prises en charge, puis cliquez sur **Enregistrer.**
22. Sélectionnez l’onglet **Détails supplémentaires**.
23. Cliquez sur les **points de suspension verticaux** en haut à droite de la section Éléments tarifaires. Cliquez sur **+ Nouvel élément tarifaire**.
24. Sélectionnez **Filtrer directement** pour les tarifs. Sélectionnez **Entier** pour l’option de quantité de vente.
25. Sélectionnez l’onglet **Informations de tarification**, entrez *199 $* pour le montant, puis sélectionnez **Enregistrer et Fermer.**
26. Si la publication automatique est activée, ignorez cette étape. Sinon, sélectionnez **Publier** et **Confirmer** pour publier le produit.
27. Dans le menu de gauche, sélectionnez **Produits**.
28. Les produits que vous avez créés doivent apparaître dans la vue Tous les produits, familles et offres groupées. Vous pouvez basculer vers cette vue en sélectionnant l’icône de liste déroulante <bpt ctype="x-unknown" id="1" rid="1"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">**</bpt></bpt>˅<ept id="2" rid="1"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">**</ept></ept> en regard du titre de vue par défaut. 
