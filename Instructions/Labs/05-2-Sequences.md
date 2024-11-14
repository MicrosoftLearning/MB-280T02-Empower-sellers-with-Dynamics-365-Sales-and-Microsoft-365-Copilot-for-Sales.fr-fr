---
lab:
  title: "Labo\_5.2\_: générer une séquence"
---

# Module 5 : utiliser Dynamics 365 Sales Insights et l’accélérateur des ventes 

## Labo pratique 5.2 : générer une séquence

### Scénario
Les vendeurs de Contoso Coffee suggèrent que les ventes pourraient être améliorées si les « meilleures pratiques » organisationnelles étaient plus faciles à suivre. Après examen, les responsables commerciaux de Contoso ont déterminé une séquence idéale d’événements de vente que les vendeurs doivent suivre. Ils veulent appliquer les meilleures pratiques en configurant une série d’activités consécutives que les vendeurs doivent suivre pour qualifier leurs prospects. Vous devez faire en sorte que ces meilleures pratiques soient aussi simples à suivre que possible tout au long du processus. Vous avez déterminé qu’une séquence est la meilleure façon d’y parvenir.

À l’issue de ce labo, vous pourrez :

-   Créer un segment
-   Créer une séquence
-   Définir des activités de séquence
-   Activer et connecter des séquences à des enregistrements

## Exercice 1 : créer et attacher des séquences à des enregistrements

### Tache 1 : activer l’accélérateur des ventes

1.  Dans le groupe Sales Insights, sélectionnez **Paramètres globaux**.
2.  Dans le sous-groupe Accélérateur des ventes, sélectionnez l’onglet **Séquences**.
3.  Vous êtes invité à configurer l’espace de travail pour pouvoir utiliser des séquences. Sélectionnez le bouton **Configurer un espace de travail**.
4.  Sélectionnez le bouton **Installation rapide**.
5.  Dans la section Type d’enregistrement et formulaire, sélectionnez **+ Ajouter un type d’enregistrement**. Sélectionnez **Opportunités**.
6.  Pour le formulaire par défaut de chaque type d’enregistrement, procédez à la configuration comme suit :
    -   Prospects : Sales Insights
    -   Opportunités : Sales Insights
7.  Cliquez sur le bouton **Publier**.
    -   Remarque : l’application de vos modifications peut prendre plusieurs minutes.

### Tâche 2 : créer un segment

1.  Si vous ne l’avez pas déjà fait, choisissez la zone **Paramètres Sales Insights**.
2.  Dans le groupe Sales Insights, sélectionnez **Paramètres globaux**.
3.  Dans le sous-groupe Accélérateur de ventes, sélectionnez l’onglet **Affectation de travail**.
4.  Vérifiez que le **type d’enregistrement** est défini sur **Prospects** et sélectionnez le bouton **Nouveau segment**.
5.  Dans le champ **Nom**, entrez le texte **Prospects du salon commercial**, puis sélectionnez le bouton **Suivant**.
6.  Sous l’onglet **Définition de segment**, sélectionnez le bouton **Ajouter**.
7.  Dans le menu qui s’affiche, sélectionnez **Ajouter une ligne**.
8.  Configurez la condition comme suit :
    1.  **Source de prospect** – **Égal à** – **Salon commercial**
9.  Sélectionnez **Simuler les résultats**.

    Un écran de simulation des membres du segment s’affiche, qui inclut tous les prospects répondant à vos critères.

10. Fermez la fenêtre **Simulation des membres du segment**.
11. Sélectionnez le bouton **Enregistrer**.
12. Sélectionnez le bouton **Activer**.

## Exercice 2 : créer et attacher des séquences à des enregistrements

### Tâche 1 : créer une séquence

1.  Si vous ne l’avez pas déjà fait, choisissez la zone **Paramètres Sales Insights**.
2.  Dans le groupe Sales Insights, sélectionnez **Paramètres globaux**.
3.  Dans le sous-groupe Accélérateur des ventes, sélectionnez l’onglet **Séquences**.
4.  Si nécessaire, sélectionnez **Activer** sur la notification pour permettre au flux de travail des séquences de fonctionner correctement.
5.  Sur la page Séquences, sélectionnez **+ Nouvelle séquence**.
6.  Vous avez la possibilité de créer une séquence à partir d’un certain nombre de modèles courants. Vous pouvez explorer les modèles disponibles. Une fois que vous êtes prêt, sélectionnez **Démarrer de zéro**.
7.  Ensuite, vous attribuez un nom et une description, puis choisissez le type de tableau pour lequel la séquence est disponible. Dans la zone de texte Nom de séquence, tapez le nom de séquence *Suivi du salon commercial*.
8.  Dans la zone de texte Description, entrez la description de la séquence : « Il s’agit d’une séquence de test pour le café test. Cette séquence sera utilisée pour suivre les clients potentiels après les salons commerciaux. »
9.  Dans Type d’enregistrement, sélectionnez **Prospect** si ce n’est pas déjà fait.
10. Sélectionnez **Suivant**.

### Tâche 2 : choisir la première activité à effectuer par le vendeur

Choisissez la première étape à suivre par vos vendeurs. Cela peut être l’envoi d’un e-mail, un appel téléphonique ou l’ajout d’une tâche de votre choix. Dans notre exemple, nous allons commencer par un e-mail.

1.  Sous la vignette de démarrage de la séquence, sélectionnez le bouton **+** pour ajouter une action ou un autre élément.
2.  Cliquez sur **Envoyer un e-mail**.
3.  En guise de titre, entrez : *e-mail d’introduction*.
4.  Dans Description, entrez une description facultative : *Présenter le prospect à l’équipe commerciale*.
5.  Si des modèles d’e-mail (modèles spécifiques à un tableau ou modèles globaux) sont disponibles dans votre organisation, vous pouvez en choisir un. Dans ce cas, nous partons du principe que le vendeur écrit son propre e-mail d’introduction.
6.  Sélectionnez le **X** pour sortir du volet Activité.
7.  Dans la barre de commandes de la séquence, cliquez sur l’icône **Enregistrer**.

### Tâche 3 : ajouter des activités supplémentaires à effectuer par votre vendeur

Ajoutez d’autres activités que vos vendeurs devront effectuer dans l’ordre. Par exemple, le vendeur doit d’abord réaliser la première activité, la deuxième, la troisième, et ainsi de suite.

1.  Cliquez sur le bouton **+**.
2.  Choisissez l’activité suivante que le vendeur doit effectuer. Cela peut être l’envoi d’un e-mail, un appel téléphonique ou l’ajout d’une tâche de votre choix. Sélectionnez **Définir le temps d’attente** pour définir un intervalle de temps entre les activités. Dans notre exemple, nous allons ajouter un intervalle de temps de 1 heure.
3.  Cliquez sur Enregistrer.
4.  Cliquez sur le bouton **+**.
5.  Sélectionnez **Appel téléphonique**.
6.  Dans le titre, entrez *Appel de suivi*. Vous pouvez choisir d’ajouter une description si vous le souhaitez.
7.  Sélectionnez **Enregistrer** sur la barre de commandes.

### Tâche 4 : activer la séquence

Pour rendre la séquence utilisable par les vendeurs, vous devez l’activer.

1.  Sélectionnez **Activer** dans la barre de commandes.
2.  Sélectionnez **Je comprends**, puis **Activez** dans la fenêtre contextuelle.
3.  Votre séquence affiche à présent une barre verte en haut, vous indiquant qu’elle a été correctement activée.

### Tâche 5 : connecter la séquence à un segment

1.  Vérifiez que vous êtes dans la zone **Paramètres Sales Insights**.
2.  À l’aide de la barre de navigation à gauche, cliquez sur **Séquences**.
3.  Ouvrez la séquence **Suivi du salon commercial** que vous avez créée précédemment.
4.  Sélectionnez l’onglet **Prospects connectés**.
5.  Sélectionnez **+ Connecter des segments**.
6.  Recherchez et sélectionnez le segment Trade **Prospects du salon** que vous avez créé précédemment.
7.  Sélectionnez **Connecter**.

### Tâche 6 : connecter la séquence à enregistrer (à partir de l’enregistrement)

1.  Définissez la zone sur **Ventes** à l’aide du menu déroulant inférieur gauche.
2.  Dans le menu de navigation du site, sélectionnez **Prospects**.
3.  Sélectionnez un prospect créé précédemment.
4.  Dans la barre de commandes, sélectionnez la flèche **vers le bas** en regard des séquences. Dans le menu qui s’affiche, sélectionnez **Connecter la séquence** dans la barre de commandes.
5.  Sélectionnez la séquence que vous avez créée précédemment, puis sélectionnez **Connecter**.
6.  Un message de confirmation apparaît en bas de la page et la séquence est connectée à l’enregistrement du prospect sélectionné.
7.  Si vous êtes invité à affecter un vendeur, sélectionnez le bouton **Affecter**. Désormais, les vendeurs qui ont accès à l’enregistrement du prospect peuvent voir les activités qui y sont associées.
8.  Actualisez la page. Vous devez voir les tâches que vous avez créées dans la section **Suivant**.

