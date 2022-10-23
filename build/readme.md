Packaging et Intégration Continue.

Ajoutez vos scripts et configurations du cloud (AMI), conteneur (Docker), OS (deb, rpm, pkg) et package dans le dossier /build/package

Placez vos scripts et configurations de CI(travis, circle, drone) dans le dossier /build/ci .

Prenez garde au fait que certains outils de CI( ex: Tavis CI) sont très contraignants vis à vis de l'emplacement de leurs fichiers de configuration.

Essayez donc, lorsque c'est possible, de créer des liens entre le dossier /build/ci et les endroits où les outils de CI s'attendent à trouver ces fichiers.