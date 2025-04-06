c'est quoi le cache ?  

--->site web >>> ecommerce >>> affiche les produits
---> chaque fois >>. user>> siteweb >>> request dans db >>
---> tu affiche les produits >>> le pb >>> tu le fais pour tous les users 

--->> dashboard ou tu affiche des stats
===> si il ya pas de cache il >>> lanteur du system 

---> trop de requestes >> lenteur de l'application >> faire fuire les user 
----> trop de requestes >> coute cher 


--->> 1000 sans cache 
---->> sql 
---> le temps de reponse tres eleve 
---> la charge server tres lourde


avec le cache 
requetes 1er >> enregister dans le cache pour 10min 
la prochaine fois >>> repere plutot le cache 


---> Performance 
         seo , ux (score lighthouse)

----> economie des resources 
    - moin de requeste 
    - moins de calcul serveur  

---> 

qu'est qu'il faut reeleement mettre en cache? 

--> request sql complexe 
--> api exchange rate ( mettre cache )
--> rendu html d'un page 

qu'est ce qu'il ne faut pas mettre en cache 
--> donnees user sensible 
---> formulaire 

memoire, fichier, redis
cache (cache.set(), cache.get())

--cache une vue complete 
--cacher un fragment(sidebar dans un fichier html)
--cache manuel(low level)
