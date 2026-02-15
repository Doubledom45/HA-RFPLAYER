# Pour les logs dans les Journaux de HA 
## [Méthode du Bouton plus Bas dans cette info]

<img width="1400" height="465" alt="image" src="https://github.com/user-attachments/assets/fd9f134a-84f9-45dc-af94-0be26cc4a56e" />


<img width="1162" height="330" alt="image" src="https://github.com/user-attachments/assets/da9b82cd-1f17-4030-8d46-cc99f80b6119" />

Passer en YAML car pas de sélection possible <img width="144" height="62" alt="image" src="https://github.com/user-attachments/assets/4cfc548a-d569-471d-b315-6be2473cbf81" />

Fonction debug en mode debug
```
action: logger.set_level
alias: Mode Debug
data:
  custom_components.rfplayer: debug
```

<img width="1134" height="408" alt="image" src="https://github.com/user-attachments/assets/a3a48c57-cee1-4faa-9640-096f051316e4" />
<img width="165" height="61" alt="image" src="https://github.com/user-attachments/assets/dcf0a5a8-187f-4d18-9140-acc54971eb0b" />

## POUR INFORMATION
Fonction debug en mode normal (erreur) 

```
action: logger.set_level
alias: Mode Debug
data:
  custom_components.rfplayer: error
```

# ON VA VOIR DANS LES JOURNAUX DE HA
<img width="1665" height="169" alt="image" src="https://github.com/user-attachments/assets/ff861b3e-e37a-441d-9723-d98d6eb8a634" />


On va tout à droite sur <img width="37" height="42" alt="image" src="https://github.com/user-attachments/assets/10b7b2e2-494c-4de8-9ce5-4016020fe190" />


Pour passer en mode Brut [live] <img width="231" height="72" alt="image" src="https://github.com/user-attachments/assets/c67ede73-2c78-47db-9bbf-897b32d4e8ff" />


Et là ça cause !
<img width="1627" height="573" alt="image" src="https://github.com/user-attachments/assets/f1cf2957-d21d-4617-879b-231c98d52f91" />

Et évidemment on peux repasser en mode Erreur moins bavard !


Moi j’ai fait une création d’un Template commutateur avec ces Fonctions, directement dans Rfplayer Dashboard

# Méthode du Bouton Log

👉<img width="146" height="34" alt="image" src="https://github.com/user-attachments/assets/a5ad48ff-6663-47fc-a5c4-584a4fd138f5" />


👉<img width="553" height="63" alt="image" src="https://github.com/user-attachments/assets/f1804d3d-b0ee-4a80-bdc9-e8fea104bcae" />


👉<img width="1103" height="46" alt="image" src="https://github.com/user-attachments/assets/1b76f252-0f6e-4793-a6b4-e02b1a51d691" />

Ajout par <img width="204" height="65" alt="image" src="https://github.com/user-attachments/assets/a9cdfcad-77ce-4762-8f0f-f18d40f7edea" />

👉<img width="428" height="585" alt="image" src="https://github.com/user-attachments/assets/675690dd-0734-4ac2-bb55-53a178bb9698" />

Choisir template 👉<img width="442" height="62" alt="image" src="https://github.com/user-attachments/assets/b9be966d-51af-4985-9a26-19e453f63c62" />

<img width="548" height="727" alt="image" src="https://github.com/user-attachments/assets/d99949a7-4df1-4e35-8a41-7f1484567f2d" />


Choisir Commutateur <img width="546" height="51" alt="image" src="https://github.com/user-attachments/assets/5882dc2c-981b-420a-a515-1b1ce232dfbb" />


<img width="549" height="731" alt="image" src="https://github.com/user-attachments/assets/3fa4acc9-e353-4d60-a2bb-d84f1abeb136" />


On rempli avec le Nom, les fonctions On et OFF , et la sélection de l'appareil !
Pour moi le Nom 👉    Log ❌Erreur / Debug✅

On va ajouter les actions 
<img width="204" height="62" alt="image" src="https://github.com/user-attachments/assets/726f24fb-e5ed-4eb7-8595-1b3ec5a4d200" />


On cherche action
<img width="910" height="309" alt="image" src="https://github.com/user-attachments/assets/3563b398-4bfc-4481-aa45-b9939cdc3c31" />

<img width="500" height="372" alt="image" src="https://github.com/user-attachments/assets/d40c20df-19c2-4ea6-bd76-c8f38895139b" />

<img width="497" height="112" alt="image" src="https://github.com/user-attachments/assets/2ea3b5a7-2543-4b63-b31b-c3e643660f66" />

[ il y a bug dans HA , on ne peut pas sélectionner l'intégration] 
On sélectionne puis il faut passer en mode YAML par les 3pts verticaux <img width="495" height="463" alt="image" src="https://github.com/user-attachments/assets/f6812136-7edf-4c73-a189-576a82bce41c" />

On remplace par :
```
action: logger.set_level
data:
  custom_components.rfplayer: debug
alias: Mode Debug
```

On va sur la partie Actions lors de la désactivation

Et on fait presque la même chose ! avec remplacement par :
```
action: logger.set_level
data:
  custom_components.rfplayer: error
alias: Mode Erreur
```
On ajoute le lien vers le Rfplayer<img width="511" height="103" alt="image" src="https://github.com/user-attachments/assets/3cffc84d-193f-4811-be35-26fcf2da7b94" />


<img width="551" height="1066" alt="image" src="https://github.com/user-attachments/assets/06545110-8c49-4a9a-9860-c94ff98c22ed" />


Message en rouge [Normal car HA à le Bug cité avant]

<img width="499" height="56" alt="image" src="https://github.com/user-attachments/assets/61d5eaa3-0cf1-421a-acce-cf09cec50f8a" />


On valide 👉<img width="88" height="54" alt="image" src="https://github.com/user-attachments/assets/d75fdcdc-97e0-4edc-a1a0-f04c513800a7" />


Si pas d'erreur

<img width="366" height="186" alt="image" src="https://github.com/user-attachments/assets/d21d790d-ab1d-489f-814c-33dafc7f44d5" />


👉 <img width="130" height="76" alt="image" src="https://github.com/user-attachments/assets/44eec390-eab7-48f9-b1be-91d7557569dc" />


On devrait l'avoir dans les entrées <img width="1353" height="48" alt="image" src="https://github.com/user-attachments/assets/e8b466de-6b17-4916-b9f8-020209ee9bfc" />


Et dans le menu du RFPLAYER

<img width="287" height="221" alt="image" src="https://github.com/user-attachments/assets/111d2f03-d1ef-458a-a3f4-323442beaf6c" />


Si je sélectionne le ON [Debug] je devrais voir les log dans la partie Journaux de HA

# ON VA VOIR DANS LES JOURNAUX DE HA
<img width="1665" height="169" alt="image" src="https://github.com/user-attachments/assets/ff861b3e-e37a-441d-9723-d98d6eb8a634" />


On va tout à droite sur <img width="37" height="42" alt="image" src="https://github.com/user-attachments/assets/10b7b2e2-494c-4de8-9ce5-4016020fe190" />


Pour passer en mode Brut [live] <img width="231" height="72" alt="image" src="https://github.com/user-attachments/assets/c67ede73-2c78-47db-9bbf-897b32d4e8ff" />


Et là ça cause !
<img width="1627" height="573" alt="image" src="https://github.com/user-attachments/assets/f1cf2957-d21d-4617-879b-231c98d52f91" />

Et évidemment on peux repasser en mode Erreur moins bavard !


Il peut y avoir des warnings sur le retour d'informations en mode autre que ZIA33 du type ZIA66.

Je ne décode pas , je mets l'information


Peut-être dans une new version 😎🙄👀



