backend de cache 
determine ou et comment les donnees en cache sont stockees 

django >> plusieurs solution:
    -1 selon le volume de donnee a stocker 
    -2 selon le context d'execution(dev, prod, cicd)
    -3 des performance attendues


LES PRINCIPAUX BACKEND DE DJANGO 

1- LocMemCache: le cache en memoire locale
    avantage : super rapide, facile a conf
    inconv: cache vide au redemarage du serveur, non partage entre plusierus serveurs ou processus


2- FileBasedCache ---> cache sur le disque
    avantage: persistance au redemarage , facile a deployer sur un petit vps (vitual private server)
    inconv: access disque=lent, gestion de fichier

3- DatabaseCache: cache via la base de donnees 
    avantage: facile a mettre en place, pas de depense externe
    incov: lent(sql request), chargement de la base de donnee

    python mangae.py createcachetable 


4-Mencache cache distribue haute performance
    avantage: ultra rapide, distribue, mature et robute 

    incov: ne supporte pas des type complexe
    pip install python-memecached


5- REDIS 
pip install django-redis


