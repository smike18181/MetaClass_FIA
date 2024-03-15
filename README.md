# MetaClass_FIA

MetaClass_FIA è un progetto univeristario che ha lo scopo di:
1. Analisi del problema e obiettivi da raggiungere
2. Analizzare un dataset preso da Kaggle per esplorare i dati al suo interno
3. Ingegnerizzazione dei dati affinchè siano conformi al problema in esame
4. Applicazione del metodo empirico su vari Regressori definendo un metodo opportuno per la validazione
5. Intregazione del modulo con l'applicativo MetaClass.

## Com'è strutturata la repository?
La nostra repository presenta una cartella chiamata 'MetaClassAI_Documentazione' in cui è presente la documentazione relativa al regressore.
Il documento è stato realizzato in LaTeX e come editor è stato utilizzato 'Overleaf' (motivo per il quale ha una struttura divisa in varie sezioni).
Il documento finale è stato esportato in formato pdf e si chiama 'MetaClass_FIA.pdf'

Nella cartella file è presente il dataset utilizzato per allenare e testare il modello. All'apertura su github è possibile vedere i dati in forma tabellare con le intestazioni delle varie colonne (feature) del dataset. 

Fuori dalla cartella è presente il file 'MetaClass_Meeting_IA.ipynb' che è il cuore pulsante del nostro progetto. E' stato sritto su Jupiter Notebook e mostra l'intera fase di analisi e progettazione del modello e dei dati che lo compongono.
Nell'ultimo blocco di codice è possibile vedere come viene esportato il modello allenato in un file PMMl ('RegressoreDurataMeeting.pmml') che verrà utilizzato per effettuare le stime in MetaClass.

Infine sono presenti tutte le immagini generate dal notebook citato prima. Queste immagini sono plot sui dati e sui risultati degli algoritmi utilizzati per il metodo empirico.

## Obiettivo

Il nostro obiettivo è quello di creare un regressore che consente di stimare la durata ideale di un meeting all'interno di una stanza.
I meeting e le stanze a cui si fa riferimento sono delle entità logiche definite e sviluppate in MetaClass che sono la base per la realizzazione di eventi e incontri virtuali tra i vari partecipanti presenti nella stanza. Più in particolare:
1. Stanza: una stanza è come un gruppo su whatsapp, ovvero un luogo dove si possono effettuare incontri, conversazioni, giochi etc. le stanze sono sia ad accesso privato che pubblico e per accedervi è necessario l'inserimento di un codice a 6 cifre per poi essere autorizzato dall'organizzatore (o organizzatore master) della stanza stessa.
2. Meeting: un meeting è un incontro organizzato per un giorno e un orario specifico. Ogni meeting è correlato alla stanza, quindi ogni partecipante che ha accesso a quest'ultimo può partecipare alla riunione virtuale.

MetaClass a sua volta è una companion app di MetaClassVR, ovvero l'estensione di tutto ciò che si è detti (più ulteriori funzionalità) nel mondo della realtà aumentata. Per poter utilizzare tale applicativo è necessario l'ausilio di un VisoreVR che può portare problemi fisiologici (per esempio nausea, mal di testa etc.) a utenti sia esperti che inesperti.
MetaClass_FIA vuole venire incontro a queste problematiche, cercando di stimare un durata di utilizzo ideale del visore durante lo scheduling (organizzazione) di un meeting.

## Guida all'installazione

### 1. Clonare il repository

Per prima cosa, clona il repository sul tuo computer utilizzando il comando `git clone` e subito dopo l'url del repository:
```sh
git clone https://github.com/smike18181/MetaClass_FIA
```
All'interno di questa repository ci sono file che non richiedono il download di librerie in aprticolare, tranne il file 'MetaClass_Meeting_IA.ipynb'

### 2. Installazioni librerie

Prima di tutto è necessario aver scaricato il linguaggio 'Python'. Per scaricarlo si può accedere al seguente link: https://www.python.org/downloads/

Per poter accedere al notebook è necessario installare jupiter Notebook al seguente link: https://jupyter.org per poi avere la possibilità di poter modificare e utilizzare l'intero progetto. 
Prima di fare ciò però è necessario installare le seguenti librerie:

pandas: È una libreria Python che fornisce strutture dati e strumenti di analisi dati per manipolare e analizzare dati in modo rapido e facile. È particolarmente utile per la pulizia, l'esplorazione e la manipolazione di dati tabulari.
```sh
pip install pandas
```
matplotlib: È una libreria per la visualizzazione dei dati che consente di creare grafici e visualizzazioni di alta qualità in Python. È molto flessibile e offre un'ampia gamma di opzioni per personalizzare i grafici.
```sh
pip install matplotlib
```
scipy: È una libreria Python per la matematica scientifica e l'ingegneria che fornisce funzioni per l'ottimizzazione, l'algebra lineare, l'interpolazione, la trasformata di Fourier, la statistica e molto altro ancora.
```sh
pip install scipy
```
seaborn: È una libreria Python basata su matplotlib per la visualizzazione dei dati statistici. Offre una sintassi ad alto livello per creare grafici attraenti e informativi, ed è particolarmente utile per esplorare e visualizzare relazioni complesse nei dati.
```sh
pip install seaborn
```
statsmodels: È una libreria Python che fornisce strumenti per la stima di modelli statistici, la condotta di test statistici e l'analisi dei dati. È particolarmente utile per la modellazione statistica e l'analisi dei dati.
```sh
pip install statsmodels
```
yellowbrick: È una libreria Python per la visualizzazione dei modelli di machine learning che offre strumenti per visualizzare metriche di prestazione, diagnostiche dei modelli e altro ancora. È progettata per essere facile da usare e integrarsi con altri strumenti di machine learning in Python.
```sh
pip install yellowbrick
```
termcolor: È una libreria Python per colorare il testo nelle console Python. È utile per migliorare la leggibilità del testo nelle console e nei terminali.
```sh
pip install termcolor
```
scikit-learn: È una libreria Python per l'apprendimento automatico (machine learning) che offre una vasta gamma di algoritmi di apprendimento supervisionato e non supervisionato. È progettata per essere semplice da usare e integrarsi con altre librerie Python per l'analisi dei dati.
```sh
pip install scikit-learn
```
sklearn2pmml: È una libreria per la conversione di modelli scikit-learn in PMML (Predictive Model Markup Language), un formato standard per la rappresentazione dei modelli di apprendimento automatico. È utile quando si desidera distribuire modelli scikit-learn su piattaforme che supportano PMML.
```sh
pip install sklearn2pmml
```





