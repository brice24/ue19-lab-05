# ue19-lab-05
gestion de la securitz operationelle / lab_5

## Description
Ce programme Python interroge l'API publique JokesAPI pour afficher une blague.

## Installation
1. Cloner ce dépôt :
   ```bash
    git clone https://github.com/brice24/ue19-lab-05
    cd ue19-lab-05

2. Installer les dépendances : 
pip install -r requirements.txt

3. Pour exécuter le programme, utilisez :
python app.py

### 4. **Créer le fichier Dockerfile**

Créez un fichier Dockerfile pour containeriser l'application :
dockerfile
# Utiliser une image de base Python
FROM python:3.9-slim

# Définir le répertoire de travail dans le conteneur
WORKDIR /app

# Copier les fichiers nécessaires
COPY . /app

# Installer les dépendances
RUN pip install --no-cache-dir -r requirements.txt

# Définir la commande par défaut
CMD ["python", "app.py"]

# Procedure d'Installation de Docker sur windows 

il est important d'installer docker pour windows enfin de pemettre a notre image concu de 
application de tourner. 
une fois installer docker sur windows, faut lancer docker et ce rendre dans le termimal : 
saisir la command : build -t python-joke-fetcheur .
2. docker run --rm python-joke-fetcheur

si tous ce passe bien alors, une blague apparaitra sur le terminal comme dans la capture d'ecran. 

il est important de decoucher option wsl et aussi d'activer hyper-v sur notre machine. 



