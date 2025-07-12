##Tutorial
How to make push with ssh key an d haw this work?
Comment faire un push vers github en utilisant un clé ssh et comment ça fonctionne?

Pour ce fair c'est simple il suffit de suivre les étapes suivantes:
	1- Création de la clé SSH
		Créer une clé ssh propre à ton utilisateur en tapant la commende "ssh-keygen -t "type" -C "commentaire"
	"type" : représente l'algoritme de chiffrement qui sont:
		-rsa (Revet-Shamir-Adleman) est un algoritme de chiffrement asymétrique largement utilisé et bien établi. On peut utiliser l'option -b avec suivie de la taille de la clé en bit "ssh-keygen -t rsa -b 4096 -C "commentaire" par exemple.
		-ed25519 est un algorithme basé sur des courbes eliptiques, plus moderne,rapide et sécurisé avec une taille de clé plus petite.
	
	2-Liason de la clé ssh avec github
		-Aller dans le dossier .ssh et on copie tout le contenu du fichier .pub concerner
		-Allez sur votre compte GITHUB, dans les settings->SSH and GPG keys->New ssh key
		-Donner un titre à votre clé
		-Coller dans la section key ce que vous avez copier
		-Clicker sur Add SSH key, entrez votre mot de passe et c'est finit

