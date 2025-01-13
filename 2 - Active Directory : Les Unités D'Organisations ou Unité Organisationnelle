# Création u**nités D'Organisations / groupe / user**

Depuis le Gestionnaire de serveur, cliquer sur le menu **Outils** et choisir **Utilisateurs et ordinateurs Active Directory** (tout en bas).

(Pour mieux s’en sortir et ne pas se mélanger avec les comptes intégrés, nous allons créer un dossier pour les utilisateurs de notre société (Unité d’Organisation, OU en anglais). Ce « super groupe » sera plus facile à gérer, par exemple avec des GPO.)

## **Créer une Unité d'Organisation (OU)**

Dans **Utilisateurs et ordinateurs Active Directory** :

1. **Navigue jusqu’au domaine** : Dans le panneau de gauche, tu devrais voir une liste de tes domaines. Dans ce cas, cherche **wilders.lan**.
2. **Clic droit sur le domaine** : Fais un clic droit sur **wilders.lan** et sélectionne **Nouveau** > **unité d’organisation**.
    - Une Unité d'Organisation (OU) est un conteneur dans Active Directory où tu peux organiser tes objets (utilisateurs, groupes, ordinateurs) de manière logique. Elle te permet de mieux gérer les objets au sein de l’Active Directory.
3. **Nom de l'OU** : Dans la boîte de dialogue qui apparaît, entre le nom de l’unité d’organisation. Ici, nomme-la **Wilders_students**.
4. **Valide** : Clique sur **OK**.

Cela crée une nouvelle unité d’organisation appelée **Wilders_students** dans ton domaine **wilders.lan**.

## **Créer un Groupe d'Utilisateurs "Students"**

Un groupe est utilisé pour regrouper des utilisateurs ayant des droits ou permissions similaires. Voici comment créer un groupe d’utilisateurs :

1. **Navigue dans l'OU** : Une fois l'OU "Wilders_students" créée, clique dessus dans le panneau de gauche pour la sélectionner.
2. **Clic droit sur l’OU** : Fais un clic droit sur **Wilders_students**, puis sélectionne **Nouveau** > **Groupe**.
3. **Nom du groupe** : Dans la fenêtre qui s'ouvre, entre **Students** comme nom du groupe.
4. **Sélectionner le type de groupe** :
    - **Scope** : Choisis "Global" si tu veux que ce groupe soit utilisé uniquement dans ce domaine.
    - **Category** : Choisis "Security" si tu veux que ce groupe serve à gérer des permissions (par exemple, l'accès à certains fichiers ou ressources). Si tu choisis "Distribution", le groupe sera utilisé uniquement pour l'envoi d’e-mails.
5. **Clique sur OK** : Une fois le groupe créé, il apparaîtra dans l'OU **Wilders_students**.

## **Créer un Utilisateur au sein du Groupe**

Maintenant, tu vas créer un utilisateur dans l'OU **Wilders_students** et l'ajouter au groupe **Students**.

1. **Clic droit sur l’OU "Wilders_students"** : Fais un clic droit sur l'OU, puis sélectionne **Nouveau** > **Utilisateur**.
2. **Remplir les informations de l'utilisateur** :
    - **First Name** : Le prénom de l'utilisateur (par exemple "flosh").
    - **Last Name** : Le nom de l'utilisateur (par exemple "Grenouille").
    - **User logon name** : Le nom de connexion de l'utilisateur (par exemple "floshg").
    
    Cela crée un compte utilisateur avec un nom d'utilisateur qui pourra se connecter à l'Active Directory.
    
3. **Mot de passe** : Après avoir cliqué sur **Next**, tu seras invité à définir un mot de passe pour l'utilisateur. Assure-toi que le mot de passe respecte les politiques de sécurité du domaine (par exemple, une longueur minimale de 8 caractères avec des majuscules, des minuscules, des chiffres, etc.).
4. **Options de mot de passe** :
    - Tu peux cocher "L’utilisateur doit changer de mot de passe a la prochaine connexion" pour forcer l'utilisateur à changer son mot de passe la première fois qu'il se connecte.
    - Clique sur **Next**, puis sur **Finish**.

Cela crée un utilisateur dans l'OU **Wilders_students**.

## **Ajouter l'Utilisateur au Groupe "Students"**

Maintenant, l'utilisateur créé doit être ajouté au groupe **Students** pour qu'il fasse partie de ce groupe.

1. **Accède aux propriétés de l'utilisateur** : Double-clique sur l’utilisateur que tu viens de créer dans l'OU **Wilders_students**.
2. **Onglet "Membre de"** : Une fois dans les propriétés de l'utilisateur, clique sur l'onglet **Membre de**. Cet onglet liste tous les groupes auxquels appartient l'utilisateur.
3. **Ajouter au groupe "Students"** : Clique sur **Add**, tape **Students** dans le champ, puis clique sur **Check Names** pour vérifier que le groupe existe bien.
4. **Valide** : Clique sur **OK** pour ajouter l'utilisateur au groupe **Students**.
