# Pour les logs dans les Journaux de HA 
## [Méthode du Bouton plus Bas dans cette info]

<img width="236" height="54" alt="image" src="https://github.com/user-attachments/assets/b84cec6b-707a-4d09-aff1-2a12ca874e18" />

<img width="546" height="49" alt="image" src="https://github.com/user-attachments/assets/f2b4f16c-6aff-48c7-b6af-a59977b4e416" />

<img width="534" height="63" alt="image" src="https://github.com/user-attachments/assets/5d8d5c96-147b-45ab-9332-fe4203685000" />

<img width="1650" height="70" alt="image" src="https://github.com/user-attachments/assets/f65815eb-6639-44f3-b88e-70c8518f4231" />

On va tout à droite sur <img width="44" height="54" alt="image" src="https://github.com/user-attachments/assets/35bebbcf-aa36-4293-9d0f-635d25df5a3c" />

Pour passer en mode Brut [live] <img width="217" height="55" alt="image" src="https://github.com/user-attachments/assets/122ecfad-7372-4d2b-b588-7fd5ef480943" />

Et là ça cause !
<img width="1630" height="281" alt="image" src="https://github.com/user-attachments/assets/89c6c886-d702-4854-9bb9-0c975a624d71" />

Et évidemment on peux repasser en mode Erreur moins bavard !

## Il faut accéder au mode développement .

<img width="165" height="46" alt="image" src="https://github.com/user-attachments/assets/8021e6ff-7118-42ea-ab84-80162d39a719" />

<img width="535" height="72" alt="image" src="https://github.com/user-attachments/assets/36cd6d5b-3888-47b7-b493-f1b29b60a305" />

<img width="570" height="72" alt="image" src="https://github.com/user-attachments/assets/e8784e7c-b990-46e4-ba27-fca56ac181bc" />

Rechercher log

<img width="1078" height="247" alt="image" src="https://github.com/user-attachments/assets/3e7b613a-7163-46c4-9123-928a2e508177" />

Prendre le deuxième <img width="1034" height="79" alt="image" src="https://github.com/user-attachments/assets/b2d3453b-f9ba-43a7-876b-ee0e65c5a8ca" />

<img width="1135" height="302" alt="image" src="https://github.com/user-attachments/assets/dc9ddbd2-3518-462b-a289-a9f11af3c63d" />

Passer en Mode YAML [ il y a bug dans HA , on ne peut pas sélectionner l'intégration] <img width="135" height="60" alt="image" src="https://github.com/user-attachments/assets/09cc9f3c-cb6a-448a-99ea-26a0ffa87ed1" />

# Et remplacer par

Pour le mode debug

```
action: logger.set_level
data:
  custom_components.rfplayer: debug
alias: Mode Debug
```

Pour le mode Erreur

```
action: logger.set_level
data:
  custom_components.rfplayer: error
alias: Mode Erreur
```

Moi j’ai fait une création d’un Template commutateur avec ces Fonctions, directement dans Rfplayer Dashboard

# Méthode du Bouton Log

👉<img width="228" height="39" alt="image" src="https://github.com/user-attachments/assets/e72350e1-6495-4996-b9ba-9d4770d9e7d3" />

👉<img width="528" height="53" alt="image" src="https://github.com/user-attachments/assets/640eb9f6-e714-42fa-91b8-e2a817bd0619" />

👉<img width="137" height="53" alt="image" src="https://github.com/user-attachments/assets/e300d31a-24ac-4247-9ec5-d714dbc3f100" />

👉<img width="193" height="59" alt="image" src="https://github.com/user-attachments/assets/2834a674-4183-4687-9080-2feb16d9d4d7" />

👉<img width="441" height="621" alt="image" src="https://github.com/user-attachments/assets/2fdc8b24-bd21-46a1-b1cc-fb7c03ca980d" />

Choisir template 👉<img width="427" height="41" alt="image" src="https://github.com/user-attachments/assets/852f7e7f-45ca-4715-95fd-39aa8f8a9043" />

<img width="549" height="844" alt="image" src="https://github.com/user-attachments/assets/dabf70e5-c059-4cfd-a2a1-7c4b4cba1438" />

Choisir Commutateur <img width="525" height="45" alt="image" src="https://github.com/user-attachments/assets/c9bdd16f-d4e4-4660-abab-d0aac578117d" />

<img width="548" height="733" alt="image" src="https://github.com/user-attachments/assets/2b43b433-fec7-47a1-92d9-5a69fea71a86" />

On rempli avec le Nom, les fonctions On et OFF , et la sélection de l'appareil !
Pour moi le Nom 👉    Log ❌Erreur / Debug✅

On va ajouter les actions 
<img width="183" height="61" alt="image" src="https://github.com/user-attachments/assets/75629124-7f72-42e5-ab84-805b58547c55" />

On cherche action
<img width="917" height="260" alt="image" src="https://github.com/user-attachments/assets/b265c2df-b404-4624-a9d1-c0d381e2b46b" />


[ il y a bug dans HA , on ne peut pas sélectionner l'intégration] 
On sélectionne puis il faut passer en mode YAML par les 3pts verticaux <img width="25" height="30" alt="image" src="https://github.com/user-attachments/assets/cd920619-904e-4e4a-ac2a-bdf6cf4d688d" />

<img width="519" height="240" alt="image" src="https://github.com/user-attachments/assets/cfe67a64-f112-415d-893d-f044b45f9fb2" />

puis sélection de <img width="185" height="37" alt="image" src="https://github.com/user-attachments/assets/47bcc004-0979-44d8-9e9f-5632767139eb" />

 <img width="534" height="515" alt="image" src="https://github.com/user-attachments/assets/d09fd3f7-7a81-46f4-946a-37387516c279" />
 
<img width="529" height="182" alt="image" src="https://github.com/user-attachments/assets/f592ba49-91f6-48b8-ab06-e9745a73051f" />

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
On ajoute le lien vers le Rfplayer<img width="500" height="83" alt="image" src="https://github.com/user-attachments/assets/23a617c5-4398-45eb-9741-5b4d833fde85" />

<img width="463" height="135" alt="image" src="https://github.com/user-attachments/assets/2c4d2524-d0cb-4745-8ad3-5f85d3bcf0ce" />


<img width="545" height="1029" alt="image" src="https://github.com/user-attachments/assets/6329fc25-9ab0-4709-82c5-3e76428e73cb" />

Message en rouge [Normal car HA à le Bug cité avant]

<img width="560" height="181" alt="image" src="https://github.com/user-attachments/assets/4ac66a5c-9b38-436c-bf2b-3a8342dbcda8" />

On valide 👉<img width="90" height="62" alt="image" src="https://github.com/user-attachments/assets/869d29eb-b8e9-497c-bbde-83881637f090" />

Si pas d'erreur

<img width="377" height="190" alt="image" src="https://github.com/user-attachments/assets/9e6c39cc-881a-4f52-8df4-3d0df0ee3beb" />

👉 <img width="101" height="76" alt="image" src="https://github.com/user-attachments/assets/4f487b89-31e3-4139-bc0e-03e12dd738e9" />

On devrait l'avoir dans les entrées <img width="1685" height="100" alt="image" src="https://github.com/user-attachments/assets/a010857e-fbde-489c-800f-d76f358b1838" />

Et dans le menu du RFPLAYER

<img width="622" height="274" alt="image" src="https://github.com/user-attachments/assets/ac3656c5-7128-40b4-b708-0c966cf1a757" />

Si je sélectionne le ON [Debug] je devrais voir les log dans la partie Journaux de HA

<img width="236" height="54" alt="image" src="https://github.com/user-attachments/assets/b84cec6b-707a-4d09-aff1-2a12ca874e18" />

<img width="546" height="49" alt="image" src="https://github.com/user-attachments/assets/f2b4f16c-6aff-48c7-b6af-a59977b4e416" />

<img width="534" height="63" alt="image" src="https://github.com/user-attachments/assets/5d8d5c96-147b-45ab-9332-fe4203685000" />

<img width="1650" height="70" alt="image" src="https://github.com/user-attachments/assets/f65815eb-6639-44f3-b88e-70c8518f4231" />

On va tout à droite sur <img width="44" height="54" alt="image" src="https://github.com/user-attachments/assets/35bebbcf-aa36-4293-9d0f-635d25df5a3c" />

Pour passer en mode Brut [live] <img width="217" height="55" alt="image" src="https://github.com/user-attachments/assets/122ecfad-7372-4d2b-b588-7fd5ef480943" />

Et là ça cause !
<img width="1630" height="281" alt="image" src="https://github.com/user-attachments/assets/89c6c886-d702-4854-9bb9-0c975a624d71" />

Et évidemment on peux repasser en mode Erreur moins bavard , avec le bouton en OFF !

<img width="605" height="263" alt="image" src="https://github.com/user-attachments/assets/e6cf8abc-a08b-4e0d-9796-76bedf27d975" />

Il peut y avoir des warnings sur le retour d'informations en mode autre que ZIA33 du type ZIA66.

Je ne décode pas , je mets l'information

<img width="943" height="37" alt="image" src="https://github.com/user-attachments/assets/fd17f224-9cfc-44c4-8f3c-89918422df1d" />

Peut-être dans une new version 😎🙄👀



