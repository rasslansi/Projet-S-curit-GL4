## Section 1:

### 1.0.1 Installations et configurations nécessaires:

![Image1](image_url1)
![Image2](image_url2)
![Image3](image_url3)

### 1.0.2 Vérification de la configuration initiale: 

#### Bash Script

![Image4](image_url4)

```
root@server:~# slapcat
```
![Image5](image_url5)

```
root@server:~# ldapsearch -H ldapi:/// -x -b dc=insat,dc=tn
```
![Image6](image_url6)
### 1.1.1 Configurez un serveur OpenLDAP avec deux utilisateurs et deux groupes:

Le fichier **`add_content.ldif`** est un fichier LDIF (LDAP Data Interchange Format) qui est utilisé pour ajouter des données à un serveur LDAP, tel qu'OpenLDAP. Dans le contexte de la configuration d'un serveur OpenLDAP avec deux utilisateurs et deux groupes, ce fichier contiendra des entrées LDIF décrivant ces utilisateurs et groupes.

Contenu du fichier **add_content.ldif :**
![Image3](image_url3)
> [!NOTE]  
> Cependant, le simple fait de créer et d'éditer le fichier LDIF ne suffit pas à les intégrer dans le serveur LDAP. Nous allons utiliser la commande ldapadd pour importer ces données dans le serveur LDAP. La commande ldapadd prend en entrée un fichier LDIF et l'ajoute au serveur LDAP.

![Image3](image_url3)

Nous pouvons vérifier les entrées comme suit:

![Image3](image_url3)![Image3](image_url3)

Nous avons changé les mots de passe de nos 2 utilisateurs:

![Image3](image_url3)
