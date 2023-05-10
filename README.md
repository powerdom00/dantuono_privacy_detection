# dantuono_privacy_detection

Questa repository contiene gli strumenti ottenuti come descritto nella ricerca: 
Tecniche per individuare vulnerabilità software che mettono a rischio la privacy.

La ricerca va a modificare dx2021 (https://github.com/dcoimbra/dx2021) nella direzione dell'individuazione di vulnerabilità legate alla privacy.\\
La cartella astminer/dataset contiene il dataset di test ottenuto, suddiviso in 3 parti.\\
Lo script astminer/src/main/kotlin/astminer/Code2VecCMethods.kt è stato modificato per assegnare l’etichetta di tipo privacy.\\
Lo script code2vec/prediction_outputter.py è stato modificato per riconoscere la nuova etichetta.\\
Lo script code2vec/config.py è stato modificato per gestire la nuova etichetta e per applicare gli ipeprarametri descritti nella ricerca.\\
Lo script code2vec/preprocess.sh è stato modificato per prendere in input gli ast path generati tramite astminer e i file preprocessati da code2vec sono salvati nella directory data/fixes/.\\
I modelli finali ottenuti sono in dx2021/code2vec/models/, in particolare la cartella devign contiene il modello di confronto e la cartella fixmodels contiene i fixmodel descritti nella ricerca.\\\\

*per utilizzare i modelli è necessaria l’installazione del software Google TensorFlow.
