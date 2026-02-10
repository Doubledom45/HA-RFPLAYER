[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=Doubledom45&repository=HA-RFPLAYER&category=integration)
# Installation depuis HACS
 
# VERSION MODIFIER 2026.2


Avec le lien https://github.com/Doubledom45/HA-RFPLAYER

Catégorie 

Choix :
Intégration

<img width="458" height="211" alt="image" src="https://github.com/user-attachments/assets/5cec8e15-3e24-4c58-a53a-13f2151fc84f" />




## Test avec new repos 👉<img width="67" height="30" alt="image" src="https://github.com/user-attachments/assets/2e9005bf-bb7c-4a4e-a9b5-96b2c698b25e" />

<img width="358" height="252" alt="image" src="https://github.com/user-attachments/assets/db83e44f-391b-4e35-afab-eaac83068ca1" />👈Clic sur l'addon

<img width="800" height="624" alt="image" src="https://github.com/user-attachments/assets/72b8f68b-e3d3-46d4-afe9-69c0f7465077" />



## Clic <img width="158" height="58" alt="image" src="https://github.com/user-attachments/assets/358b23b3-99db-4e92-8647-483f93e83174" />

<img width="509" height="382" alt="image" src="https://github.com/user-attachments/assets/cc8bc413-10b9-48f2-b116-b0d0111d46f9" />


 👉<img width="102" height="39" alt="image" src="https://github.com/user-attachments/assets/6016edb9-838f-480c-9eb5-7d28534026f4" />


# Reboot
<img width="567" height="123" alt="image" src="https://github.com/user-attachments/assets/a8da8158-d841-4da9-884c-010180e32336" />
<img width="543" height="213" alt="image" src="https://github.com/user-attachments/assets/88d1bf76-4670-4338-bf89-864da16abc80" />👈
<img width="359" height="181" alt="image" src="https://github.com/user-attachments/assets/a2438eb0-924b-4a08-90ab-95d690312f60" />👈

## Ajout dans intégration <img width="559" height="52" alt="image" src="https://github.com/user-attachments/assets/bd954d9b-3277-4fbf-9ee2-427641513af3" />


<img width="428" height="185" alt="image" src="https://github.com/user-attachments/assets/acda240a-215b-496e-924e-6f7e2dcb32f9" />


## Après ajout choix USB
<img width="450" height="527" alt="image" src="https://github.com/user-attachments/assets/c7e15fb9-936d-48a7-ac2b-02d56bde164d" />

# Choisir ce qui doit être le [BON !] port du Rfplayer
Devrait être dans le choix , avec son intitulé soit FTDI_FT232R_USB_UARTxxx ou l'ancien usb-Zieblue_RFPLAYER ...

## Après Validation

<img width="360" height="323" alt="image" src="https://github.com/user-attachments/assets/2964943e-1b40-462d-8c99-0659afe2e8ba" />

CHOIX POSSIBLE du Nom de l'appareil et de la pièce  (  Bug sur l'intitulé dans HA )<img width="150" height="48" alt="image" src="https://github.com/user-attachments/assets/3f548a3d-5ce2-441a-8b00-1f6e06d4c234" />


## ✅ 👉 Ignorer et terminer

<img width="278" height="133" alt="image" src="https://github.com/user-attachments/assets/15e1eb92-8ea1-4f54-bdc3-8e5688c84311" />


## selection ! 👆👆🏻
<img width="953" height="344" alt="image" src="https://github.com/user-attachments/assets/6a1b4cee-2a43-4ed6-ac21-7f4bc622db80" />


## Configurer si besoin !<img width="58" height="54" alt="image" src="https://github.com/user-attachments/assets/74fee173-1f02-43fc-9752-03cf0f6ae8d3" />

<img width="255" height="906" alt="image" src="https://github.com/user-attachments/assets/a63ea33c-ddd1-4c4a-ad5e-d466a5905bb2" />


## en bas Valider
Puis Terminer !

![image](https://github.com/Doubledom45/HA-RFPLAYER/assets/97252459/02ceaae4-b869-41b3-b3d7-bcd98cc1abaa)

# Donc Reboot !
## ET HOP

<img width="328" height="122" alt="image" src="https://github.com/user-attachments/assets/1d6937ac-3595-493e-9c10-b0ba691219c1" />


## Je vais sur l'appareil
<img width="928" height="326" alt="image" src="https://github.com/user-attachments/assets/3fdc3dc3-c9da-4106-b086-19572d522444" />


## Il est bavard !

<img width="973" height="237" alt="image" src="https://github.com/user-attachments/assets/6967d0a9-4346-4dd8-ba95-02c7de880c86" />

L'information des "Protocol" en cours 
<img width="373" height="262" alt="image" src="https://github.com/user-attachments/assets/eff6a52e-2612-4146-9667-9d0c64ad1829" />

Et la partie Diagnostic qui reprend l'information compléte du RFPLAYER
Un peu trop, mais c'est ce qui me permet de vérifier si Problème .
<img width="115" height="792" alt="image" src="https://github.com/user-attachments/assets/0481fa70-ad5d-43f2-9ee0-5d70a4e3451e" />

Il y a la possibilité de suivre les Log dans les journaux de HA, avec une cde développement 
```
action: logger.set_level
data:
  custom_components.rfplayer: debug
alias: Mode Debug
```
Voir l'Information Bouton log.md !
