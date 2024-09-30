# Reti Kolmogorov Arnold e Multilayer Perceptron: Un Confronto Sperimentale

# Introduzione
La ricerca di intelligenze artificiali più interpretabili e precise ha portato allo sviluppo delle Kolmogorov-Arnold Networks (KAN), che offrono un'alternativa agli MLP (Multi-Layer Perceptron). Le reti KAN si distinguono per una maggiore accuratezza e interpretabilità rispetto agli MLP, grazie all'uso di funzioni di attivazione apprendibili al posto dei pesi presenti nei modelli MLP.

# Reti MLP
Un MLP (Multilayer Perceptron) è una rete neurale feedforward che rappresenta una delle architetture di base nel deep learning. È progettato per apprendere funzioni non lineari complesse attraverso una serie di strati di neuroni completamente connessi.
Una rete MLP è composta fondamentalmente da tre tipologie di layer: un input layer, un output layer e un numero arbitrario di hidden layer che si trovano tra l'input e l'output layer. 
I neuroni che si trovano in strati adiacenti sono completamente collegati tra loro. Ogni connessione ha un peso associato, che determina la forza della connessione. Un peso elevato significa una forte connessione, mentre un peso basso o negativo indica una connessione debole o inibitoria. 

# Reti KAN
Le reti di Kolmogorov-Arnold (KAN) sono alternative promettenti ai percettori multistrato (MLP). Le reti KANs si basano sul teorema di rappresentazione di Kolmogorov-Arnold a differenza degli MLP che si basano su teorema si approssimazione universale.
A differenze di quanto avviene negli MLP in un KAN, ogni parametro di peso è sostituito da una funzione univariata  parametrizzata come spline. Di conseguenza, le KAN non hanno pesi lineari. I nodi sommano poi i segnali in entrata senza applicare alcuna non-linearità.
Questo cambiamento rende le KAN più interpretabili degli MLP.

# Contenuti della Repository
**`/Power Consuption`**: Directory che contiene il dataset PowerConsuption e l'addestramento delle reti KAN  e MLP su questo dataset.

**`/Train Delay`**: Directory che contiene il dataset Train Delay e l'addestramento delle reti KAN  e MLP su questo dataset.

**`requirements.txt`**: File contenente le dipendenze Python necessarie per eseguire il progetto, che possono essere installate con `pip`.

# Link Utili
**Libreria pykan**: [pykan Library](https://github.com/KindXiaoming/pykan)

# Riassunto
