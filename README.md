#  LAB 9 : Démo Navigation Drawer et Fragments

---

### Réalisé par

**Abla MARGHOUB**

### Encadré par

**Pr. Mohamed LACHGAR**

### Module

**Développement et Design Web**

### Établissement

**École Normale Supérieure - Université Cadi Ayyad**

---


## 1.  Objectif du TP

* Créer une application Android utilisant le modèle **Navigation Drawer Activity**
* Manipuler un **DrawerLayout** et un **NavigationView**
* Créer et afficher des **Fragments** dynamiquement selon le menu sélectionné
* Ajouter un **ListFragment** pour afficher une liste simple
* Structurer correctement un projet Android avec ViewBinding

---

## 2. Architecture du TP

### 2.1 Stack technologique

| Technologie / Outil            | Rôle dans le projet                  |
| ------------------------------ | ------------------------------------ |
| **Android Studio**             | Environnement de développement       |
| **Java**                       | Langage principal de l’application   |
| **Android SDK 24+**            | Version minimale supportée           |
| **Material Design Components** | Composants UI du Drawer / Navigation |
| **Fragments API**              | Création et gestion des écrans       |
| **XML Layouts**                | Création de l’interface graphique    |

---

### 2.2 📁 Structure du projet

```
NavigationDrawerDemo/
│
├── java/
│   └── ma/ens/navgationdraw/
│       ├── MainActivity.java
│       ├── BlankFragment.java
│       ├── BlankFragment2.java
│       └── FragmentList.java
│
├── res/
│   ├── layout/
│   │   ├── activity_main.xml
│   │   ├── app_bar_main.xml
│   │   ├── content_main.xml
│   │   ├── fragment_blank.xml
│   │   ├── fragment_blank2.xml
│   │   └── nav_header_main.xml
│   │
│   ├── menu/
│   │   ├── activity_main_drawer.xml
│   │   └── main.xml
│   │
│   ├── drawable/
│   │   ├── ic_home.xml
│   │   ├── ic_dashboard.xml
│   │   └── ic_list.xml
│   │
│   ├── values/
│       ├── colors.xml
│       ├── strings.xml
│       └── themes.xml
│
└── AndroidManifest.xml
```

---

## 3. 🟢 Résultat attendu

L’application finale doit afficher un **menu latéral Navigation Drawer**, permettant d’afficher trois fragments différents :

### ✔️ Écran d’accueil (avec Drawer fermé)

📸 *Capture d’écran attendue*
*(exemple)*

```
[Toolbar avec bouton hamburger]
[Contenu vide avant sélection d’un fragment]
```

---

### ✔️ Menu Navigation Drawer ouvert

📸 *Capture d’écran attendue*
*(exemple)*

```
Fragment 1
Fragment 2
Fragment List
```

---

### ✔️ Fragment 1 (fond rose)

📸 *Capture d’écran attendue*
*(exemple)*

```
-------------------------------
|   Fragment 1 (fond rose)    |
-------------------------------
```

---

### ✔️ Fragment 2 (fond bleu)

📸 *Capture d’écran attendue*

```
-------------------------------
|   Fragment 2 (fond bleu)    |
-------------------------------
```

---

### ✔️ Fragment List (ListFragment)

📸 *Capture d’écran attendue*

```
Item 1
Item 2
Item 3
...
Item 10
```

---

Si tu veux, je peux aussi te créer :

✅ un **README en Markdown avec images intégrées**
➡️ (tu m’enverras les captures d’écran et je les place correctement)

ou

✅ un **fichier README.md prêt à télécharger**

Dis-moi ce que tu préfères !
