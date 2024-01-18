## Section 1:

### 1.0.1 Installations et configurations nécessaires:

![Image1](/Users/user/GL4/ProjetSec/Projet-Securite-GL4/Authentication with OpenLDAP, SSH, Apache, OpenVPN/Demo/1.png)
![Image2](/Users/user/GL4/ProjetSec/Projet-Securite-GL4/Authentication with OpenLDAP, SSH, Apache, OpenVPN/Demo/2.png)
![Image3](/Users/user/GL4/ProjetSec/Projet-Securite-GL4/Authentication with OpenLDAP, SSH, Apache, OpenVPN/Demo/3.png)

### 1.0.2 Vérification de la configuration initiale: 

#### Bash Script

![Image4](/Users/user/GL4/ProjetSec/Projet-Securite-GL4/Authentication with OpenLDAP, SSH, Apache, OpenVPN/Demo/4.png)

```
root@server:~# slapcat
```
![Image5](/Users/user/GL4/ProjetSec/Projet-Securite-GL4/Authentication with OpenLDAP, SSH, Apache, OpenVPN/Demo/5.png)

```
root@server:~# ldapsearch -H ldapi:/// -x -b dc=insat,dc=tn
```
![Image6](/Users/user/GL4/ProjetSec/Projet-Securite-GL4/Authentication with OpenLDAP, SSH, Apache, OpenVPN/Demo/6.png)
### 1.1.1 Configurez un serveur OpenLDAP avec deux utilisateurs et deux groupes:

Le fichier **`add_content.ldif`** est un fichier LDIF (LDAP Data Interchange Format) qui est utilisé pour ajouter des données à un serveur LDAP, tel qu'OpenLDAP. Dans le contexte de la configuration d'un serveur OpenLDAP avec deux utilisateurs et deux groupes, ce fichier contiendra des entrées LDIF décrivant ces utilisateurs et groupes.

Contenu du fichier **add_content.ldif :**
![Image7](/Users/user/GL4/ProjetSec/Projet-Securite-GL4/Authentication with OpenLDAP, SSH, Apache, OpenVPN/Demo/7.png)
> [!NOTE]  
> Cependant, le simple fait de créer et d'éditer le fichier LDIF ne suffit pas à les intégrer dans le serveur LDAP. Nous allons utiliser la commande ldapadd pour importer ces données dans le serveur LDAP. La commande ldapadd prend en entrée un fichier LDIF et l'ajoute au serveur LDAP.

![Image8](/Users/user/GL4/ProjetSec/Projet-Securite-GL4/Authentication with OpenLDAP, SSH, Apache, OpenVPN/Demo/8.png)

Nous pouvons vérifier les entrées comme suit:

![Image9](/Users/user/GL4/ProjetSec/Projet-Securite-GL4/Authentication with OpenLDAP, SSH, Apache, OpenVPN/Demo/9.png)![Image3](/Users/user/GL4/ProjetSec/Projet-Securite-GL4/Authentication with OpenLDAP, SSH, Apache, OpenVPN/Demo/1.png)

Nous avons changé les mots de passe de nos 2 utilisateurs:

![Image10](/Users/user/GL4/ProjetSec/Projet-Securite-GL4/Authentication with OpenLDAP, SSH, Apache, OpenVPN/Demo/10.png)
