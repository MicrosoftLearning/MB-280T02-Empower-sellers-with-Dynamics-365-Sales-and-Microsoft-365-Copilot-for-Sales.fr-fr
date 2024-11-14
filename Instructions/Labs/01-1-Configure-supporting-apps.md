---
lab:
  title: "Labo\_1.1\_: configurer des applications supports"
---

# Module 1 : Configurer Dynamics 365 Sales

## Labo pratique 1.1 : configurer des applications supports

## Scénario

Les vendeurs de Contoso Coffee indiquent que si Dynamics 365 Sales est très utile pour augmenter leur productivité, l’application semble très cloisonnée par rapport à leur flux quotidien de travail. Ils demandent les fonctions suivantes à leur service informatique :

-   Les vendeurs souhaitent suivre et gérer la correspondance par e-mail liée aux ventes dans CRM.
-   Les vendeurs souhaitent stocker des documents liés aux ventes (comme les articles de base de connaissances sur les produits, la recherche sur les clients et les rapports de tendances du marché) dans CRM. Ils souhaitent pouvoir accéder à ces documents, ainsi que les partager et les gérer directement à partir de l’application Sales.
-   Les vendeurs souhaitent collaborer avec d’autres services, tels que l’inventaire, le traitement des commandes et le marketing, pendant qu’ils exploitent leurs opportunités de vente. Ils souhaitent que ces autres services puissent collaborer au sujet d’un enregistrement client au sein d’une conversation ou d’un canal Teams.
-   Les vendeurs ont beaucoup entendu parler des fonctionnalités Copilot dans Dynamics 365 Sales, comme la possibilité d’obtenir un résumé des enregistrements, de se tenir au courant des modifications apportées aux enregistrements, de préparer des réunions et de rédiger des messages. Ils veulent s’assurer que les fonctionnalités de Copilot sont activées dans leur environnement afin de pouvoir commencer à tirer parti de l’IA au sein de l’application et améliorer leur productivité.

Dans ce labo, nous allons activer et configurer les fonctionnalités qui aideront notre organisation CRM à répondre aux demandes de ces vendeurs.

## Exercice 1 : configurer l’intégration de la messagerie, SharePoint et OneDrive

### Tâche 1 : configurer l’intégration de la messagerie

1.  Dans un navigateur web, accédez à [admin.powerplatform.microsoft.com](https://admin.powerplatform.microsoft.com/).
2.  Dans la navigation du site sur le côté gauche de l’écran, sélectionnez **Environnements**.
3.  Sélectionnez l’environnement **Évaluation des ventes** pour l’ouvrir.
4.  Recherchez et sélectionnez **Paramètres** dans les commandes répertoriées en haut.
5.  Sélectionnez le titre E-mail pour le développer et sélectionnez **Boîtes aux lettres**.
6.  Ouvrez l’enregistrement Boîte aux lettres pour **Administrateur MOD**.
7.  Configurez la **boîte aux lettres administrateur MOD** comme suit :
    -   **Profil de serveur** : Microsoft Exchange Online
    -   **Courrier électronique entrant** : synchronisation côté serveur ou E-mail Router
    -   **Courrier électronique sortant** : synchronisation côté serveur ou E-mail Router
    -   **Rendez-vous, Contacts et Tâches** : Synchronisation côté serveur
8.  **Enregistrez** les changements apportés. Cliquez ensuite sur **Approuver l’adresse e-mail**. (**Remarque :** vous devez approuver la boîte aux lettres avant de pouvoir envoyer et recevoir des e-mails.)
9.  Vous serez invité à approuver l’adresse e-mail principale. Cliquez sur **OK**.
10. Cliquez sur le bouton **Tester et activer la boîte aux lettres**.
11. Sur la fenêtre contextuelle Tester et activer, assurez-vous que si cette boîte aux lettres a été précédemment configurée pour se synchroniser avec une autre organisation, l’activation de cette option permet de basculer vers la synchronisation avec cette organisation.
12. Cliquez sur **OK**.

**IMPORTANT :** ne quittez pas cette page tant que les tests ne sont pas terminés. Si vous souhaitez travailler sur la tâche 2 pendant que les tests s’effectuent, vous pouvez ouvrir un autre onglet ou navigateur.

## Tâche 2 : activer l’intégration SharePoint basée sur un serveur

Dans cette tâche, vous allez activer l’intégration SharePoint basée sur un serveur pour votre organisation Dynamics 365.

1.  Dans un navigateur web, accédez à [admin.powerplatform.microsoft.com](https://admin.powerplatform.microsoft.com/).
2.  Dans la navigation du site sur le côté gauche de l’écran, sélectionnez **Environnements**.
3.  Ouvrez l’environnement **Évaluation des ventes** dans lequel vous avez travaillé pour l’ouvrir.
4.  Recherchez et sélectionnez **Paramètres** dans les commandes répertoriées en haut.
5.  Sous le titre Intégration, sélectionnez **Paramètres de gestion des documents**.
6.  Vous devez voir l’option **Activer l’intégration SharePoint basée sur un serveur**. (Si l’option n’est pas visible, l’intégration SharePoint a déjà été activée et vous pouvez passer à l’étape onze.)
    -   Si l’intégration SharePoint n’est pas configurée, sélectionnez **Activer l’intégration SharePoint basée sur un serveur**.
7.  Sur l’écran Activer l’intégration SharePoint basée sur un serveur, cliquez sur **Suivant**.
8.  Sélectionnez **En ligne** pour le type de déploiement, puis cliquez sur le bouton **Suivant**.
9.  Saisissez l’URL du site SharePoint à utiliser. (Exemple : https://« Orgname ».sharepoint.com), cliquez sur le bouton **Suivant**.

    **Remarque :***vous pouvez trouver votre URL SharePoint en sélectionnant l’icône du vérificateur d’application dans le coin supérieur gauche de l’écran. (Ressemble à un carré de 3 x 3.) Maintenez la touche Ctrl enfoncée et sélectionnez SharePoint.*

10. Une fois le site validé, cliquez sur le bouton **Activer**.
11. Cliquez sur **Paramètres de gestion des documents**.
12. Sélectionnez les entités pour lesquelles vous souhaitez activer la gestion des documents, telles que prospects, comptes, opportunités, puis cliquez sur **Suivant**.
    -   **IMPORTANT** : si vous envisagez de configurer l’engagement lié au courrier électronique dans Sales Insights, sélectionnez l’entité e-mail.
13. Dans le champ URL du site SharePoint, entrez l’URL du site SharePoint que vous avez utilisé dans la tâche précédente.
14. Cliquez sur le bouton **Suivant**.
15. Cliquez sur le bouton **Terminer** pour terminer la configuration.

### Tâche 3 : configurer l’intégration OneDrive Entreprise

Dans cette tâche, vous allez configurer l’intégration de OneDrive pour votre organisation Dynamics CRM. (À partir de la publication de ce cours, les paramètres de gestion des documents n’étaient pas disponibles dans le Centre d’administration Power Platform. Vous devez configurer l’intégration de OneDrive Entreprise à partir de la zone Paramètres de Dynamics 365 classiques.)

1.  Dans un navigateur web, accédez à [admin.powerplatform.microsoft.com](https://admin.powerplatform.microsoft.com/).
2.  Dans la navigation du site sur le côté gauche de l’écran, sélectionnez **Environnements**.
3.  Ouvrez l’environnement **Évaluation des ventes** dans lequel vous avez travaillé pour l’ouvrir.
4.  Recherchez et sélectionnez **Paramètres** dans les commandes répertoriées en haut.
5.  Sous le titre Intégration, sélectionnez **Paramètres de gestion des documents**.
6.  Cliquez sur l’icône **Activer OneDrive Entreprise**.
7.  Cochez la case **Activer OneDrive Entreprise**, puis cliquez sur **OK**.
8.  Une fois l’écran actualisé, cliquez sur les **paramètres de dossier OneDrive Entreprise**.
9.  Acceptez le nom de dossier par défaut ou saisissez le nom de votre choix, puis cliquez sur **OK**.

## Exercice 2 : configurer Teams et Copilot

### Tâche 1 : configurer l’intégration de Teams

1.  Si nécessaire, ouvrez l’application Centres des ventes.
2.  À l’aide de la barre de navigation à gauche, sélectionnez la zone **Ventes** en bas de l’écran.
3.  Dans le menu qui s’affiche, sélectionnez **Paramètres de l’application**.
4.  Sous le groupe Paramètres généraux, sélectionnez **Discussion et collaboration**.
5.  Définissez **Activer la liaison des enregistrements Dynamics 365 aux canaux Microsoft Teams** sur **Oui**.
6.  Définissez **Activer l’intégration Microsoft Teams avancée** sur **Oui**. (Vous devrez peut-être sélectionner votre compte Administrateur MOD. Si vous êtes invité à obtenir des autorisations, sélectionnez **Accepter**.)
7.  Sous **Activer les conversations Microsoft Teams dans Dynamics 365**, sélectionnez **Activer pour toutes les applications Dynamics 365**.
8.  Sélectionnez le bouton **Enregistrer**.  
    **IMPORTANT** : l’enregistrement des modifications peut prendre plusieurs minutes.

### Tâche 2 : configurer Copilot

1.  Vérifiez que vous êtes dans la zone **Paramètres de l’application**.
2.  Sous le groupe Paramètres généraux, sélectionnez **Copilot**.
3.  Cochez la case en regard de **Essayer nos nouvelles fonctionnalités en version préliminaire avant qu’elles ne soient mises à la disposition de tous** pour l’activer.
4.  Sous **Fonctionnalités de Copilot**, modifiez **toutes les applications Dynamics 365** comme suit :
    -   **Conversation** : activé
    -   **E-mail (version préliminaire)**  : activé
5.  Sélectionnez le bouton **Enregistrer**.

