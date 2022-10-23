Les dépendances de votre application (gérées manuellement ou via votre gestionnaire de dépendances favori tel que la fonctionnalité incluse dans les Go Modules). La commande go mod vendor créera un dossier /vendor pour vous. Notez que vous devrez peut-être utiliser le flag -mod=vendor avec votre commande go build si vous n'utilisez pas Go 1.14 qui le définit par défaut.

Ne commitez pas vos dépendances si vous développez une bibliothèque.

Depuis sa version 1.13, Go active la fonctionnalité de proxy de module (en utilisant https://proxy.golang.org comme serveur de proxy par défaut). Plus d'infos ici afin de définir si cela correspond à votre obligations et contraintes. Si c'est le cas, vous n'aurez pas besoin du dossier vendor.