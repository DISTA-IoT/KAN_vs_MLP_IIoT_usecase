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

# Riassunto
Negli ultimi anni, l'intelligenza artificiale e il machine learning hanno guadagnato una rilevanza crescente in vari settori, dalla medicina all'economia, dall'ingegneria alla scienza dei dati. Tra i modelli alla base delle moderne applicazioni di deep learning ci sono le Multi-Layer Perceptrons (MLPs), note anche come reti neurali feedforward completamente connesse. Le MLP sono un pilastro del machine learning per l’approssimazione di funzioni non lineari grazie al loro potere espressivo garantito dal teorema di approssimazione universale.

Tuttavia, nonostante il loro ampio utilizzo, le MLP presentano alcuni svantaggi. Ad esempio nei transformers le MLP consumano quasi tutti i parametri non incorporati e sono generalmente meno interpretabili senza strumenti di post-analisi. Una promettente alternativa agli MLP sono le reti neurali Kolmogorov-Arnold Networks (KANs), che hanno anche loro strutture completamente connesse ma a differenza degli MLP si basano sul teorema di rappresentazione di Kolmogorov-Arnold.

La sostanziale differenza tra i due modelli sono le funzioni di attivazione sui nodi, detti neuroni. Mentre le MLP utilizzano funzioni di attivazione fisse sui nodi nelle reti KAN ogni peso è sostituito da una funzione univariata apprendibile parametrizzata come un spline. I nodi KAN sommano poi i segnali in entrata senza applicare alcuna non linearità. 

Le reti KAN sfruttano i punti di forza sia delle spline che degli MLP evitando i loro punti deboli. Le spline sono particolarmente efficaci per funzioni a bassa dimensionalità, adattandosi localmente con precisione, ma soffrono della cosiddetta "maledizione della dimensionalità" con l'aumento delle dimensioni dell'input. Le MLP, invece, sono più adatte a problemi ad alta dimensionalità, ma non ottimizzano efficacemente funzioni univariate, poiché le loro funzioni di attivazione sono globali e fisse.

Le reti KAN combinano il meglio dei due approcci, consentendo di rappresentare accuratamente funzioni complesse grazie alla capacità delle spline di modellare funzioni univariate e alla potenza delle MLP di apprendere interazioni di caratteristiche complesse. Rispetto alle MLP, le KAN richiedono grafi di calcolo più piccoli e offrono una maggiore interpretabilità, rendendo più chiara la rappresentazione delle funzioni apprese.

L'obiettivo di questa tesi è analizzare le reti Kolmogorov-Arnold e confrontarle con le tradizionali MLP. Durante l'analisi sono emerse evidenze che suggeriscono come le KAN possano rappresentare una promettente area di sviluppo nel machine learning, soprattutto per la loro capacità di approssimare funzioni multivariate complesse in modo più interpretabile rispetto alle MLP, che spesso operano come "scatole nere".

Il codice fornito in questa tesi consente di sperimentare direttamente con le reti KAN, permettendo di esplorare le loro dinamiche e potenzialità attraverso prove pratiche e test su differenti configurazioni. 

Tuttavia, nonostante i vantaggi teorici, rimangono sfide significative nell'implementazione pratica delle KAN, come il lungo tempo di addestramento rispetto alle MLP. Questo potrebbe limitarne l'adozione in contesti dove la rapidità è essenziale.

In particolare, una delle principali limitazioni riscontrate è il tempo di addestramento significativamente più lungo rispetto a quello richiesto da un MLP, il che può rappresentare un ostacolo in contesti in cui sono necessari tempi di risposta rapidi e risultati immediati. Questo lungo processo di apprendimento può ridurre l'attrattiva delle KAN per applicazioni pratiche, dove l'efficienza e la velocità sono fondamentali.

Le reti Kolmogorov-Arnold rappresentano un promettente campo di ricerca per il futuro del machine learning, ma sarà necessario lavorare sull'ottimizzazione degli algoritmi e sull'esplorazione di nuove architetture per sfruttarne appieno il potenziale. 

Le KAN offrono una nuova prospettiva per l'approssimazione di funzioni complesse, combinando interpretabilità ed efficienza, ma il loro successo dipenderà dalla capacità di superare le attuali limitazioni computazionali.

# Link Utili
**Libreria pykan**: [pykan Library](https://github.com/KindXiaoming/pykan)

