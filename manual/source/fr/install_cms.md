<!--toc=getting_started-->
#Installation du CMS
Le CMS de [[PRODUCTNAME]] est une application web PHP s'appuyant sur une base de donn�es MySQL. La combinaison PHP / MySQL est tr�s courante en tant que plateforme web et peut fonctionner sur des serveurs Linux ou Windows.

Nous vous donnons quelques instructions de base pour installer votre propre serveur web [here](install_environment.html), mais nous vous recommandons une solution bas�e sur le Cloud ou g�r�e par un service informatique si l'application d'affichage dynamique est primordiale.

## Installation
� partir de maintenant nous consid�rons que vous disposez d'un serveur web avec PHP et MySQL et que l'archive compress�e (ZIP ou Tarball) du pack d'installation du CMS a �t� transf�r�e sur le serveur.

Le processus de base est le suivant:
1. T�l�chargement et extraction de l'archive
2. D�marrage de l'installation
3. Configurations requises
4. Cr�ation de la base de donn�es
5. Informations sur la base de donn�es
6. Installation de la base de donn�es
7. Configuration finale
8. Termin�

###T�l�chargement et extraction de l'archive
L'archive CMS contient un sous-dossier nomm� [[PRODUCTNAME]]-server-[[PRODUCTVERSION]], les contenus de ce dossier doivent �tre copi�s sur un emplacement appropri� du web accessible par votre serveur. Pour les configurations les plus simples de serveur web, le nom de ce dossier correspondra au nom de l'url que vous utilisez pour acc�der au CMS. Par exemple: `http://localhost/[[PRODUCTNAME]]`.

L'archive extraite doit ressembler � la capture d'�cran ci-dessous:

![Extracted Archive](img/win32_install_extracted.png)

Il conviendra de cr�er un dossier pour la biblioth�que de [[PRODUCTNAME]]. Il servira � stocker des images, des vid�os et autres supports bas�s sur fichiers �tant transf�r�s sur le CMS. _Cette information sera n�cessaire pour les �tapes ult�rieures de l'installation._

###D�marrage de l'Installation
Le fait de se rendre sur `http://localhost/[[PRODUCTNAME]]` d�marrera automatiquement l'installation.

L'installation se fait par le biais d'un "assistant" comprenant en tout six �tapes. Il vous guidera tout au long du processus d'installation de [[PRODUCTNAME]].

### �tape 1 - Configuration requise
Le programme d'installation contient une liste d�taill�e des contr�les de tous les �l�ments indispensables pour une installation r�ussie. Chaque �l�ment comporte soit:

* Une coche - l'�l�ment est pr�sent et correct
* Un point d'exclamation - l'�l�ment est pr�sent mais peut ne pas �tre correctement configur�.
* Une croix - l'�l�ment est manquant.

Tout �l�ment avec un point d'exclamation ou une croix doit �tre v�rifi� et on utilisera ensuite le bouton r�essayer pour recommencer cette �tape.

![Installer Step 1](img/install_cms_step1.png)

Ici, les probl�mes les plus courants sont l'absence des modules PHP, les param�tres de configuration PHP et les difficult�s li�es aux fichiers d'autorisation d'acc�s � la biblioth�que.

D�s que tous les �l�ments sont coch�s appuyez sur suivant.

###Cr�ation de la base de donn�es
Le CMS peut faire l'installation dans une nouvelle base de donn�es ou dans une d�j� existante. Nous recommandons une nouvelle base.

[[PRODUCTNAME]] ne pr�fixe pas ses noms de table ce qui peut g�n�rer des conflits avec du contenu dans une base existante.

Le choix entre une base nouvelle ou existante se fera en commutant entre les deux onglets disponibles.

###Informations sur la base de donn�es
Que vous ayez opt� pour une base de donn�es existante ou pour une nouvelle, le programme d'installation aura besoin de certaines informations la concernant pour permettre au CMS de se connecter, de lire et d'�crire.

![Installer Step 2](img/install_cms_step2.png)

Le programme d'installation aura besoin des informations suivantes:

**H�te**
Le nom de votre serveur MySQL - dans la plupart des cas ce sera "localhost".

**Nom d'utilisateur administrateur**
Le nom d'utilisateur "root" de votre installation MySQL. Il ne sert que lors de l'installation et n'est utile que si vous avez demand� au programme d'installation de cr�er une nouvelle base de donn�es.

**Mot de passe administrateur**
Le mot de passe "root". Il ne sert que pour l'installation et n'est utile que si vous avez demand� au programme d'installation de cr�er une nouvelle base de donn�es.

**Nom de la base de donn�es**
Le nom de la base de donn�es.

**Nom d'utilisateur de la base de donn�es**
Le nom d'utilisateur du CMS utilis� pour se connecter � la base de donn�es - g�n�ralement le m�me.

**Mot de passe de la base de donn�es**
Le mot de passe utilis� pour se connecter � la base de donn�es.


###Installation de la base de donn�es
Le programme d'installation va maintenant cr�er / compl�ter la base de donn�es de [[PRODUCTNAME]]. Une s�rie de points doit appara�tre sur l'�cran durant le processus. Cela peut prendre quelque temps. Si tout s'est bien pass�, cliquez sur "suivant".

_Si � ce stade il y a des erreurs, veuillez vous reporter � la section (r�solution des probl�mes" de ce manuel._

###Mot de passe administrateur
Pour chaque installation au moins un niveau administrateur "superutilisateur" est n�cessaire pour g�rer le syst�me, appliquer les mises � jour et configurer les param�tres avanc�s. Le programme d'installation vous demandera de cr�er cet utilisateur lors de l'�tape 3.

![Installer Step 3](img/install_cms_step3.png)

**Ce nom d'utilisateur et ce mot de passe doivent �tre conserv�s en lieu s�r car ils seront n�cessaires lorsque l'installation sera termin�e.**


###Param�trages
L'�cran suivant concerne la configuration de [[PRODUCTNAME]]. La premi�re case demande l'emplacement o� [[PRODUCTNAME]] stockera les supports que vous allez t�l�charger. Nous avons d�j� cr�� un dossier pour cela, saisissez en ici le nom par exemple `/home/[[PRODUCTNAME]]/library`.

La case suivante demande une cl� d'acc�s au CMS - celle-ci permet d'authentifier les afficheurs en lien avec celui-ci. choisissez quelque chose de compliqu�, et notez la. Elle ne sera pas utilis�e tr�s souvent. 

La derni�re case � cocher vous demande si vous acceptez d'envoyer des statistiques anonymes au projet [[PRODUCTNAME]]. Nous vous en remercions vivement !

![Install Step 4](img/install_cms_step4.png)

###Termin�
L'installation est maintenant termin�e et le syst�me est pr�t � se connecter.

![Install Complete](img/install_cms_complete.png)
