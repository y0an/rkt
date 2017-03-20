
Présentation 
-> RKT by CoreOS 
rkt is written in Go and
container

-> AppC specification par l'Open Container Initiative 
--> On parlera aussi de l'ACI(App Container Image), ACE (App Container Executor), bref toutes les specs qui gravitent autour de l'OCI 

Let's try it! 
-> {Installation en 3 lignes} 

-> Construction d'une image from scratch pour un Ws-Rest 
--> ficher ACI + arborescence de fichier 
--> actool build / actool validate 
--> rkt run / run du premier container 

-> Registry d'image 
--> utilisation du fetch avec 
---> le registry coreos.com 
---> le registry docker 
---> github en registry 
---> serveur http 
---> ... 

-> Convertir une image docker en image ACI (ex :nginx) 
--> docker2aci pour convertir 
--> run de l'image 

-> Création d'une image avec une Webapp 
--> Introduction des volumes (ex : pour la configuration de la webapp) 

-> Faire communiquer les 3 containers entre eux 
--> Configuration du network 

#ici les 3 containers tournent l'appli fonctionne, applause!!! 

-> Intégration de rkt avec systemd 
-->systemctl, machinectl,journalctl etc.. 

-> {Rkt sur kubernetes} 

{L'outillage} 
-> les builder ACI, docker2aci,.. 
-> dgr, ggn .. 


En prod? 
->blablacar (90% de la prod / 3000 containers), XOOM (paypal) 

Pour continuer, les autres implémentation de l'appC 
-> JetPack 
-> Kurma 





#links

https://coreos.com/rkt/docs/latest/trying-out-rkt.html


https://medium.com/@adriaandejonge/moving-from-docker-to-rkt-310dc9aec938#.n3uotmpgu

https://dzone.com/articles/getting-started-with-rkt-via-codeship

https://coreos.com/rkt/docs/latest/using-rkt-with-systemd.html#systemd-run