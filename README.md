# 🎵 MP88 — Studio Vinyle & Audio

**MP88** est un lecteur audio professionnel avec **égaliseur 8 bandes**, **effets spatiaux 8D/4D**, **recherche de paroles en ligne**, **transcription audio locale** (Whisper AI) et **convertisseur vidéo→audio** (ffmpeg.wasm). Tout fonctionne dans votre navigateur.

---

## 📋 Prérequis

1. Un navigateur web moderne (Chrome, Firefox, Edge, Safari)
2. Connexion Internet requise pour :
   - Recherche de paroles (API lyrics.ovh)
   - Transcription audio (premier téléchargement du modèle Whisper)
   - Convertisseur vidéo (premier téléchargement de ffmpeg.wasm)
3. Aucune installation de logiciel nécessaire

---

## 🚀 Guide d'installation

### Étape 1 : Télécharger le fichier
1. Téléchargez le fichier `mp88.html` sur votre ordinateur
2. Placez-le dans un dossier de votre choix

### Étape 2 : Lancer l'application
- **Double-cliquez** sur le fichier pour l'ouvrir dans votre navigateur

---

## 🎯 Fonctionnalités principales

### 🎧 1. Lecteur Audio

**Formats supportés :**
| Format | Extension |
|--------|-----------|
| MP3 | `.mp3` |
| WAV | `.wav` |
| M4A | `.m4a` |
| FLAC | `.flac` |
| OGG | `.ogg` |

**Fonctionnalités :**
- Lecture/Pause avec animation vinyle
- Précédent/Suivant
- Mode aléatoire (Shuffle)
- Mode répétition
- Barre de progression cliquable
- Playlist avec noms et durées

---

### 🎚️ 2. Égaliseur 8 Préréglages

| Préréglage | Description |
|-----------|-------------|
| **Flat** | Aucun ajustement (neutre) |
| **Bass Boost** | Graves amplifiés (+8 dB à 200 Hz) |
| **Vocal Boost** | Voix mises en avant (+5 dB à 1 kHz) |
| **Treble** | Aigus amplifiés (+7 dB à 6 kHz) |
| **Rock** | Graves et aigus boostés |
| **Pop** | Équilibre général |
| **Classical** | Léger boost des extrêmes |
| **Lo-Fi** | Réduction des médiums (-6 dB à 6 kHz) |

**Filtres utilisés :**
- Low Shelf (200 Hz)
- Peaking 1 (1 kHz)
- Peaking 2 (3 kHz)
- High Shelf (6 kHz)

---

### 🌌 3. Effets Spatiaux

| Effet | Description |
|-------|-------------|
| **Off** | Son stéréo normal |
| **8D Audio** | Rotation complète en 9 secondes |
| **4D Audio** | Rotation rapide en 4.5 secondes |
| **Wide Stereo** | Élargissement stéréo subtil |

**Effets visuels :**
- Point lumineux orbitant autour du vinyle (8D/4D)
- Modulation du volume (0.85 à 1.0)

---

### 📝 4. Paroles (Lyrics)

**Deux méthodes :**

#### Méthode A : Recherche en ligne
1. Cliquez sur **« Find lyrics online »**
2. Utilise l'API gratuite lyrics.ovh
3. Nécessite une connexion Internet
4. Meilleur résultat si le fichier est nommé `Artiste - Titre.mp3`

#### Méthode B : Transcription locale
1. Cliquez sur **« Transcribe audio »**
2. Utilise le modèle Whisper Tiny (IA)
3. Premier téléchargement : ~15-40 secondes
4. Ensuite, tout fonctionne **localement**
5. Aucune donnée envoyée sur un serveur

**Correction des paroles :**
1. Sélectionnez le texte incorrect
2. Cliquez sur **« Fix selection »**
3. Tapez la correction
4. Cliquez sur **« Apply fix »**

---

### 🔄 5. Convertisseur Vidéo → Audio

**Formats d'entrée :**
| Format | Extension |
|--------|-----------|
| MP4 | `.mp4` |
| MOV | `.mov` |
| MKV | `.mkv` |
| WEBM | `.webm` |

**Formats de sortie :**
| Format | Codec | Extension |
|--------|-------|-----------|
| MP3 | libmp3lame | `.mp3` |
| WAV | PCM (sans perte) | `.wav` |
| M4A | AAC | `.m4a` |
| OGG | libvorbis | `.ogg` |

**Fonctionnement :**
- Utilise ffmpeg.wasm (compilé en WebAssembly)
- 100% client-side (aucun upload)
- Premier chargement : ~10-20 Mo de téléchargement
- Ensuite, tout fonctionne hors ligne

---

## 🎨 Thèmes

L'application propose **4 thèmes** :

| Thème | Ambiance |
|-------|----------|
| **Dark** (défaut) | Sombre avec accents dorés |
| **Light** | Clair et épuré |
| **Ocean** | Bleu océan |
| **Sunset** | Orange coucher de soleil |

**Changer de thème** : Cliquez sur l'icône lune/soleil dans l'en-tête.

---

## 📖 Guide d'utilisation détaillé

### 🔹 Étape 1 : Charger des fichiers audio

1. Cliquez sur la **zone de téléchargement**
2. Ou glissez-déposez vos fichiers
3. Sélectionnez un ou plusieurs fichiers audio
4. La playlist se remplit automatiquement
5. Le premier fichier commence à jouer

### 🔹 Étape 2 : Contrôler la lecture

- **Lecture/Pause** : Bouton central
- **Suivant/Précédent** : Flèches latérales
- **Shuffle** : Lecture aléatoire
- **Repeat** : Répétition de la piste
- **Progression** : Cliquez sur la barre pour naviguer

### 🔹 Étape 3 : Ajuster le son

1. Choisissez un **préréglage d'égaliseur**
2. Choisissez un **effet spatial** (8D, 4D, Wide)
3. Le vinyle tourne pendant la lecture
4. Le bras de lecture s'anime

### 🔹 Étape 4 : Obtenir les paroles

1. Sélectionnez une piste
2. Allez dans l'onglet **« Lyrics »**
3. Choisissez : recherche en ligne ou transcription
4. Corrigez les erreurs avec « Fix selection »
5. Copiez avec « Copy lyrics »

### 🔹 Étape 5 : Convertir une vidéo

1. Allez dans l'onglet **« Convert »**
2. Choisissez un fichier vidéo
3. Sélectionnez le format de sortie
4. Cliquez sur **« Convert to audio »**
5. Téléchargez le fichier audio

---

## 🛠️ Guide de dépannage

### Problème 1 : L'audio ne joue pas

**Cause** : Format non supporté ou fichier corrompu.

**Solution** :
- Vérifiez que le format est MP3, WAV, M4A, FLAC ou OGG
- Essayez avec un autre fichier
- Vérifiez que le volume n'est pas à zéro

---

### Problème 2 : L'égaliseur ne fonctionne pas

**Cause** : Le contexte audio n'est pas initialisé.

**Solution** :
- Cliquez sur **Play** d'abord (l'audio doit démarrer)
- L'égaliseur s'active après la première interaction
- Vérifiez que le navigateur supporte Web Audio API

---

### Problème 3 : Les effets 8D/4D ne sont pas perceptibles

**Cause** : Le son est en mono ou le casque est mal réglé.

**Solution** :
- Utilisez un **casque stéréo** pour un effet optimal
- Les effets sont plus subtils sur des haut-parleurs
- Vérifiez que l'effet est bien activé (chip en surbrillance)

---

### Problème 4 : La recherche de paroles échoue

**Cause** : La chanson n'est pas dans la base de données lyrics.ovh.

**Solution** :
- Renommez le fichier en `Artiste - Titre.mp3`
- Essayez la transcription audio à la place
- Vérifiez votre connexion Internet

---

### Problème 5 : La transcription est lente

**Cause** : Premier téléchargement du modèle Whisper (~40 Mo).

**Solution** :
- Attendez que le téléchargement se termine (une seule fois)
- Le modèle est mis en cache pour les utilisations futures
- Les pistes plus longues prennent plus de temps

---

### Problème 6 : La conversion vidéo échoue

**Cause** : Format vidéo non supporté ou mémoire insuffisante.

**Solution** :
- Utilisez des vidéos plus courtes (< 100 Mo)
- Essayez un format courant (MP4)
- Fermez les autres onglets gourmands
- Vérifiez que le navigateur supporte WebAssembly

---

### Problème 7 : La transcription ne fonctionne pas sur mobile

**Cause** : Mémoire insuffisante sur l'appareil.

**Solution** :
- Utilisez un ordinateur pour la transcription
- Fermez les autres applications
- Essayez avec une piste plus courte

---

## 📄 Copyright

**© 2026**  
📧 mohamed005cheikh@gmail.com  
**Développé par MC88**  
**Tous droits réservés**

---

## 🔒 Confidentialité

| Fonctionnalité | Traitement |
|----------------|------------|
| **Lecture audio** | 100% local |
| **Égaliseur** | 100% local (Web Audio API) |
| **Effets spatiaux** | 100% local |
| **Recherche de paroles** | Envoie le nom à lyrics.ovh |
| **Transcription audio** | 100% local (Whisper en navigateur) |
| **Conversion vidéo** | 100% local (ffmpeg.wasm) |

---

## 🔧 Bibliothèques utilisées

| Bibliothèque | Version | Usage |
|-------------|---------|-------|
| **Transformers.js** | 2.17.2 | Transcription Whisper |
| **ffmpeg.wasm** | 0.12.10 | Conversion vidéo |
| **Web Audio API** | Natif | Égaliseur et effets |

---

## ✅ Fonctionnalités techniques

- **Vinyle animé** avec rotation synchronisée
- **Bras de lecture** avec animation
- **Égaliseur 4 filtres** (Low Shelf, Peaking ×2, High Shelf)
- **Effets spatiaux** avec StereoPanner
- **Playlist** avec durées auto-détectées
- **4 thèmes** persistants
- **Transcription Whisper Tiny** en WebAssembly
- **Conversion ffmpeg** en WebAssembly
- **Correction de paroles** avec sélection
- **Design responsive** mobile-first

---

**Bonne écoute ! 🎵✨**
