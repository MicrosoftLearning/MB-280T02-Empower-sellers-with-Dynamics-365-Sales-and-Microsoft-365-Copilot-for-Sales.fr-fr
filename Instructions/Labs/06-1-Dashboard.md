---
lab:
  title: "Labo\_6.1\_: configurer un tableau de bord"
---

# Module 6 : analyser les données Dynamics 365 Sales

## Labo pratique 6.1 : configurer un tableau de bord

### Scénario
Les responsables commerciaux de Contoso Coffee souhaitent surveiller plus efficacement le succès de leur équipe commerciale, en particulier en lien avec les opportunités fermées. Un responsable commercial a demandé un tableau de bord personnel fournissant une présentation des opportunités récemment fermées et des actions connexes des vendeurs. En outre, il souhaite que ce tableau de bord s’affiche par défaut lorsqu’il ouvre la section Tableaux de bord de l’application.

À l’issue de ce labo, vous pourrez :
- Créer des tableaux de bord personnels
- Ajouter des composants aux tableaux de bord

## Exercice 1 : configurer un tableau de bord 
### Tâche 1 : créer un tableau de bord
1. Vérifiez que vous êtes bien dans la zone Ventes de l’application. Si tel n’est pas le cas, utilisez le menu déroulant en bas à gauche pour accéder à la zone **Ventes**.
2. Dans le groupe Mon travail, sélectionnez **Tableaux de bord** dans le menu de navigation de gauche.
3. Par défaut, le tableau de bord social de l’activité des ventes s’affiche. N’hésitez pas à explorer les différents composants. En outre, vous pouvez utiliser l’icône de liste déroulante <bpt ctype="x-unknown" id="1" rid="1"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">**</bpt></bpt>˅<ept id="2" rid="1"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">**</ept></ept> en regard du titre du tableau de bord pour explorer les autres tableaux de bord du système.
4. Pour créer votre tableau de bord, sélectionnez **+ Nouveau**, puis **Tableau de bord Dynamics 365**.
5. Explorez les différentes dispositions du tableau de bord. Dans cette tâche, nous allons créer un tableau de bord standard à 2 colonnes. Lorsque vous êtes prêt, sélectionnez-le dans la liste, puis sélectionnez **Créer**.

### Tâche 2 : ajouter des composants
1. Le concepteur de tableaux de bord s’ouvre dans une nouvelle fenêtre. Si tel n’est pas le cas, vérifiez que le bloqueur de fenêtres publicitaires est désactivé. Le concepteur peut prendre une minute pour se charger.
2. Dans la zone de texte Nom, tapez *Tableau de bord du responsable commercial*.
3. Ajoutons un composant à la section supérieure gauche. Les responsables commerciaux demandent un moyen simple de voir montant des revenus gagnés par rapport aux revenus perdus pour les opportunités. Ils souhaitent que ces informations s’affichent dans un graphique. Pour ce faire, nous allons ajouter un graphique en sélectionnant l’icône **Insérer un graphique** au milieu de la section supérieure gauche.
4. Sélectionnez les détails suivants de votre graphique :
   - Type d’enregistrement : Opportunité.
   - Vue : Opportunités fermées
   - Graphique : transactions gagnées et transactions perdues
   - Sélectionnez **Ajouter**.
5. Votre graphique apparaît dans la section supérieure gauche.
6. Ensuite, nous allons ajouter un composant à la section supérieure droite. Les responsables commerciaux demandent un moyen de visualiser facilement les opportunités récemment fermées, afin qu’ils puissent vérifier auprès des vendeurs les leçons qu’ils en ont tirées. Ils souhaiteraient que la vue affiche les opportunités gagnées et perdues, avec seulement les opportunités fermées au cours de l’exercice financier actuel. Sélectionnez l’icône **Insérer une liste** pour la section supérieure droite.
7. Sélectionnez les détails suivants pour votre liste :
   - Type d’enregistrement : Opportunités.
   - Vue : opportunités fermées dans l’exercice financier actuel
   - Cliquez sur **Ajouter**.

### Tâche 3 : enregistrer et modifier le tableau de bord
1. Sélectionnez **Enregistrer**, puis **Fermer**. Votre fenêtre se ferme et vous êtes renvoyé au formulaire Tableaux de bord, où votre nouveau tableau de bord s’affiche.
2. Dans la barre de commandes, sélectionnez **Définir comme valeur par défaut**. Ce tableau de bord est désormais votre tableau de bord par défaut lorsque vous accédez à la section Tableaux de bord.
3. Cliquez sur **Modifier** dans le menu supérieur. Le concepteur de tableaux de bord s’affiche dans une nouvelle fenêtre. Ajoutez deux autres composants sous votre graphique. Les composants que vous sélectionnez doivent résoudre les exigences métier suivantes demandées par les responsables commerciaux :
   - Les responsables commerciaux aimeraient avoir une idée de la façon dont chaque vendeur agit en fonction de son revenu d’opportunités fermées. Ils aimeraient un graphique qui affiche les noms des vendeurs et leur revenu total d’opportunités fermées.
   - Les responsables commerciaux aimeraient surveiller les tâches quotidiennes des vendeurs de leur équipe. Ils souhaitent voir une liste qui affiche les activités de leurs équipes commerciales.
