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

```sh
import pandas as pd
```





