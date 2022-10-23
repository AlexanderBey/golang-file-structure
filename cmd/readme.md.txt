Les applications principales de ce projet.

Le nom de répertoire de chaque application doit correspondre au nom de l'exécutable que vous souhaitez avoir (p. ex., /cmd/myapp).

Ne mettez pas trop de code dans le répertoire de votre application. 
Si vous pensez que le code peut être importé et réutilisé dans d'autres projets, 
déplacez le dans le dossier /pkg. 
Si le code n'est pas réutilisable, ou si vous ne souhaitez pas que d'autres personnes l'utilisent, 
placez le dans le dossier /internal. 
Soyez explicite quant à vos intentions, 
vous seriez surpris de l'utilisation que d'autres développeurs pourraient faire de votre code !

Il est habituel d'avoir une petite fonction main qui importe et appelle du code contenu dans les dossiers /internal et /pkg, 
et rien de plus.

Voir le dossier /cmd pour des exemples.

https://github.com/heptio/ark/tree/master/cmd (just a really small main function with everything else in packages)
https://github.com/moby/moby/tree/master/cmd
https://github.com/prometheus/prometheus/tree/master/cmd
https://github.com/influxdata/influxdb/tree/master/cmd
https://github.com/kubernetes/kubernetes/tree/master/cmd
https://github.com/dapr/dapr/tree/master/cmd
https://github.com/ethereum/go-ethereum/tree/master/cmd