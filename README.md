# TP React Débutant

Ce projet est un TP React qui permet d'apprendre :

- les formulaires contrôlés
- les formulaires non contrôlés
- le partage d'état entre composants (lifting state up)
- l'utilisation du Context API

---

Interface générale

L'application contient plusieurs composants :

Formulaire contrôlé

Formulaire non contrôlé

Lifting State Up (température)

Profil utilisateur

---

1️⃣ Formulaire contrôlé

Ce formulaire utilise useState pour gérer les champs.

Les valeurs sont stockées dans le state React et mises à jour avec onChange.

Fonctionnement

L'utilisateur saisit un nom et un email

Les valeurs sont stockées dans le state

Un message d'alerte affiche les informations

<img width="563" height="397" alt="fotmControllee" src="https://github.com/user-attachments/assets/a36ad5db-929f-4668-9fc1-a67c1a7f0ebc" />



---
2️⃣ Formulaire non contrôlé

Ce formulaire utilise useRef pour accéder aux valeurs des champs.

React ne contrôle pas directement les inputs.

Fonctionnement

Les champs sont liés à des références (useRef)

Lors du submit, les valeurs sont récupérées via ref.current.value

<img width="559" height="177" alt="formNonControlee" src="https://github.com/user-attachments/assets/87371639-a367-41d4-a702-622871aecb91" />

---


3️⃣ Lifting State Up

Ce composant montre comment partager l'état entre un parent et un enfant.

Le composant parent TemperatureConvertor contient l'état :

const [celsius, setCelsius] = useState('');

Le composant enfant TemperatureInput reçoit :

la valeur

la fonction de modification

<img width="562" height="131" alt="temperature" src="https://github.com/user-attachments/assets/62c50b08-80f9-4af0-9349-06fe00424d2a" />

---

4️⃣ Profil utilisateur (Context API)

Le contexte React permet de partager les données utilisateur dans toute l'application.

Le contexte est défini dans :

UtilisateurContext.js

Le composant Profil permet :

d'afficher l'utilisateur connecté

de se déconnecter

<img width="556" height="143" alt="profil" src="https://github.com/user-attachments/assets/9f61cc91-fd1b-4a0c-9a2e-3487e9d026a6" />

---
##Résultat final :

<img width="558" height="621" alt="resultat" src="https://github.com/user-attachments/assets/f0810a72-19b2-44c2-9071-5d0362c8c964" />

---
Technologies utilisées

React

JavaScript

CSS
