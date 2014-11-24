<!--toc=getting_started-->
#Installation du client Windows
Le client windows de [[PRODUCTNAME]] est distribu� sous forme de fichier d'installation "MSI" correspondant � une installation standard par "double-clic".

Le processus comprend trois �tapes:
1. Pr�paration - conditions minimales et MSI
2. Installation - Double cliquez sur le MSI pour commencer l'installation.
3. Connexion - [Connectez votre client au CMS](#configuration)

##Conditions minimales
[[PRODUCTNAME]] est une solution d'affichage dynamique � faible consommation. Toutefois, avec les progr�s de la technologie il a �t� n�cessaire de fixer certaines conditions minimales. Celles-ci seront v�rifi�es par le programme d'installation mais elles sont cependant r�pertori�es ci-dessous pour plus de commodit�:

- Connexion r�seau au CMS (si possible par internet)
- Microsoft Windows XP SP3 / Windows Vista / Windows 7 (*Windows 7 recommand�*)
- Framework .NET v3.5 SP1
- Internet Explorer 7+ (*IE10 ou sup�rieur recommand�*)
- Flash Player Version 9 ou sup�rieure
- Windows Media Player 11 ou sup�rieur
- Pour les supports PowerPoint, Microsoft PowerPoint 2003 ou sup�rieur. *La visionneuse PowerPoint n'est pas adapt�e*.


###Installation
Pour commencer l'installation double cliquez sur le fichier `[[PRODUCTNAME]]-client-1.7.0-beta-x86.msi` que vous avez t�l�charg� avec le pack. Le programme d'installation vous guidera au fil des diff�rents �crans et vous demandera de confirmer � chaque �tape. Elles sont d�crites ci-dessous.

###�tape 1
Lors de l'installation de [[PRODUCTNAME]] il se peut que vous voyez l'avertissement de s�curit� suivant. Veuillez cliquer sur "Ex�cuter" pour commencer l'installation.

![Security Warning](img/windows_setup_security.png)

###�tape 2
Le programme d'installation affiche un �cran de bienvenue. Appuyez sur "Suivant".

![Welcome Screen](img/windows_setup1.png)

###�tape 3
Choisissez l'emplacement o� [[PRODUCTNAME]] doit �tre install�. Normalement, l'emplacement par d�faut doit convenir, cependant si vous souhaitez le changer, cliquez sur Parcourir. Apr�s l'avoir s�lectionn� (ou choisi la valeur par d�faut) cliquez sur "Suivant" pour continuer.

![Install Location](img/windows_setup2.png)

###�tape 4
Un messsage de confirmation appara�t. Si ces choix vous conviennent, cliquez sur "Install" pour commencer. Sinon cliquez sur "Pr�c�dent" pour corriger.

![Begin Installation Confirmation](img/windows_setup3.png)

###�tape 5
Fin de l'installation. Cliquez sur "Termin�" pour quitter le programme.

![Install Complete](img/windows_setup4.png)

<a name="configuration"></a>
##Connexion au CMS
Avant toute utilisation, les clients nouvellement install�s doivent �tre configur�s et enregistr�s aupr�s du CMS de [[PRODUCTNAME]]. Les options de configuration de [[PRODUCTNAME]] sont accessibles depuis chaque installation client dans le menu D�marrer, Tous les programmes.

S�lectionnez "Options client [[PRODUCTNAME]]" pour enregistrer cet afficheur sur le r�seau [[PRODUCTNAME]]; ou pour modifier la configuration de cet afficheur.

###�cran des options clients
La plupart des options clients sont d�finies sur le CMS et transmises au client par le r�seau. Ceci r�duit au minimum la configuration du client pour chaque nouvelle installation.

Pour que le CMS puisse envoyer ces options, il est indispensable d'enregistrer l'afficheur aupr�s de celui-ci. Cette t�che s'effectue � partir de l'�cran options clients, repr�sent� ci-dessous. 

![Client Options](img/windows_settings_gen.png)

Quelques autres param�tres ne peuvent �tre r�gl�s que depuis l'installation du client. Les voici ci-dessous.

###Param�trages
**Adresse du CMS**
Il s'agit de l'adresse compl�te de votre installation CMS. Par exemple `http://your.domain/cms/`.

**Cl�**
La cl� secr�te CMS qui authentifiera votre afficheur aupr�s de lui.

**Biblioth�que locale**
C'est l'emplacement o� ce client d'affichage stocke ses fichiers locaux. Ces fichiers sont t�l�charg�s depuis le CMS de sorte que le client reste op�rationnel m�me en cas de perte de la connexion avec le CMS.

**Identit� de l'afficheur**
C'est l'ID unique correspondant � cet afficheur. Un ID unique automatiquement g�n�r� est attribu� lors de l'installation mais il pourra �tre modifi�e s'il y a lieu.

**�cran d'accueil**
Il est possible de remplacer l'�cran d'accueil par une image stock�e en local sur le PC client.

###param�trage du proxy
Le client d'affichage doit avoir acc�s au CMS durant le processus d'enregistrement ainsi que pour recevoir du nouveau contenu. Si le client est derri�re un serveur proxy, saisissez les informations le concernant dans la section Proxy.

**Nom d'utilisateur**
Nom d'utilisateur vous authentifiant aupr�s du serveur proxy.

**Mot de passe**
Mot de passe vous authentifiant aupr�s du serveur proxy.

**Domaine**
Domaine vous authentifiant aupr�s du serveur Proxy.

###Le bouton Enregistrer et les messages d'�tats
Lorsque tous les r�glages ont �t� saisis (adresse minimum du CMS, cl�, biblioth�que locale et ID de l'afficheur), appuyez sur le bouton Enregistrer. Un message appara�t alors "Enregistrement sur le CMS... Veuillez patienter..."

S'il n'y a pas eu d'erreur de communication entre l'adresse du CMS et le client, l'afficheur est enregistr� et en attente d'approbation.

###Gestion de l'afficheur du CMS
Connectez-vous maintenant � l'interface web du serveur, rendez-vous sur la page "Afficheurs". Le client que vous venez d'enregistrer doit appara�tre dans la liste. Cliquez sur le bouton "Edit" � c�t� de l'afficheur. Le statut de la licence passera automatiquement � "yes". Il est possible d'opter pour une pr�sentation par d�faut diff�rente (il s'agit de la pr�sentation que verra le client si rien n'est programm�).

####D�finition des profils de l'afficheur
Lors de l'enregistrement un profil de configuration par d�faut est attribu� au client d'affichage. Pour plus d'information voir la section Profils d'affichage.

N'oubliez pas de cliquer sur Enregistrer avant de quitter les options clients.

##D�marrage du lecteur de contenus client
Vous pouvez maintenant lancer le client d'affichage [[PRODUCTNAME]]. Vous devriez voir l'�cran d'accueil de [[PRODUCTNAME]] pendant le chargement de la pr�sentation par d�faut et de ses contenus (ainsi que tout ce que vous avez programm�); ensuite commencera la diffusion des contenus.

##Modifications de Windows
Nous vous sugg�rons les r�glages suivants dans Windows / PowerPoint pour le client d'affichage:

- �teignez tous les �conomiseurs d'�cran.
- D�sactivez le mode �conomie d'�nergie de l'�cran.
- Chargez le profil "muet" (panneau de configuration -> Sons et p�riph�riques audio Propri�t�s).
- Choisissez un papier peint uni (Personne ne le verra, esp�rons-le, mais il peut �tre n�cessaire de r�initialiser le client ou de relancer [[PRODUCTNAME]], auquel cas un arri�re-plan sans fioriture sera plus pratique).
- Si le client est accessible � partir de l'endroit o� vous g�rez vos afficheurs, il peut �tre utile d'installer un serveur UltraVNC afin de vous y connecter pour contr�ler le client de temps � autre. Dans le client VNC utilisez l'option "visualisation seulement" pour ne pas perturber l'afficheur.
- Param�trez Windows pour qu'il se connecte automatiquement en tant qu'utilisateur du client d'affichage.
- D�sactivez les info-bulles dans la zone de notification.

- Pour du powerpoint, les afficheurs doivent suivre les consignes suivantes [preparation instructions](media_powerpoint.html#machine_preparation).

**Veuillez faire une sauvegarde avant de modifier la base de registre**
