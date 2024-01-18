## Section 1:

### 1.0.1 Installations et configurations nécessaires:

![Image1](Demo/1.png)
![Image2](Demo/2.png)
![Image3](Demo/3.png)
![Image4](Demo/4.png)

### 1.0.2 Vérification de la configuration initiale: 

```
root@server:~# slapcat
```
![Image5](Demo/5.png)

```
root@server:~# ldapsearch -H ldapi:/// -x -b dc=insat,dc=tn
```
![Image6](Demo/6.png)
### 1.1.1 Configurez un serveur OpenLDAP avec deux utilisateurs et deux groupes:

Le fichier **`add_content.ldif`** est un fichier LDIF (LDAP Data Interchange Format) qui est utilisé pour ajouter des données à un serveur LDAP, tel qu'OpenLDAP. Dans le contexte de la configuration d'un serveur OpenLDAP avec deux utilisateurs et deux groupes, ce fichier contiendra des entrées LDIF décrivant ces utilisateurs et groupes.

Contenu du fichier **add_content.ldif :**
![Image7](Demo/7.png)
> [!NOTE]  
> Cependant, le simple fait de créer et d'éditer le fichier LDIF ne suffit pas à les intégrer dans le serveur LDAP. Nous allons utiliser la commande ldapadd pour importer ces données dans le serveur LDAP. La commande ldapadd prend en entrée un fichier LDIF et l'ajoute au serveur LDAP.

![Image8](Demo/8.png)

Nous pouvons vérifier les entrées comme suit:

![Image9](Demo/9.png)![Image3](Demo/9.png)

Nous avons changé les mots de passe de nos 2 utilisateurs:

![Image10](Demo/10.png)
