# streamlitbot
Construction chatbot basé sur ChatGPT et Streamlit en utlisant simplement du code python.

## Groupe :
    * Moustapha DIAGNE
    * Marie Josiane ODZALI
    * Miracle VODOUMBO


# Projet Streamlit avec OpenAI

Cette documentation explique comment récupérer ce projet, configurer votre environnement pour l'exécuter avec **Streamlit**, et ajouter une clé secrète pour utiliser l'API OpenAI.

---

## **Prérequis**

Avant de commencer, assurez-vous d'avoir :

1. **Python 3.8 ou supérieur** installé.
2. **Git** installé sur votre machine.
3. Une clé API valide pour OpenAI.

---

## **1. Cloner le dépôt GitHub**

1. Clonez ce dépôt GitHub en exécutant la commande suivante dans votre terminal :
   ```bash
   git clone <URL_DU_DEPOT_GITHUB> 
   ```
   Remplacez `<URL_DU_DEPOT_GITHUB>` par l'URL HTTPS ou SSH de ce dépôt.

2. Accédez au répertoire cloné :
   ```bash
   cd <NOM_DU_DEPOT>
   ```

---

## **2. Configurer l'environnement Python**

1. Créez un environnement virtuel Python :
   ```bash
   python -m venv env
   ```

2. Activez l'environnement virtuel :
   - **Windows** :
     ```bash
     .\env\Scripts\activate
     ```
   - **macOS/Linux** :
     ```bash
     source env/bin/activate
     ```

3. Installez les dépendances requises :
   ```bash
   pip install -r requirements.txt
   ```

---

Pour interagir avec l'API OpenAI, vous devez fournir une clé secrète. Créez un fichier nommé `secrets.toml` à la racine de votre projet et ajoutez-y votre clé au format suivant : `[default] OPENAI_API_KEY = "votre_clé_secrète"`. Pour protéger cette clé, assurez-vous que le fichier `secrets.toml` est ignoré par Git en ajoutant ou en vérifiant la ligne `secrets.toml` dans votre fichier `.gitignore`. Cela évitera tout risque de partage accidentel de la clé sur des plateformes comme GitHub.`

---

## **4. Lancer l'application Streamlit**

1. Exécutez le serveur Streamlit avec la commande suivante :
   ```bash
   streamlit run <NOM_DU_FICHIER>.py
   ```
   Remplacez `<NOM_DU_FICHIER>.py` par le nom exact du fichier Python à exécuter.

2. Une URL s'affichera dans le terminal, par exemple :
   ```
   Local URL: http://localhost:8501
   ```
   Cliquez ou ouvrez cette URL dans votre navigateur pour accéder à l'application.

---