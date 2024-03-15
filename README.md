# MetaClass_FIA

MetaClass_FIA è un progetto univeristario che ha lo scopo di:
1. Analisi del problema e obiettivi da raggiungere
2. Analizzare un dataset preso da Kaggle per esplorare i dati al suo interno
3. Ingegnerizzazione dei dati affinchè siano conformi al problema in esame
4. Applicazione del metodo empirico su vari Regressori definendo un metodo opportuno per la validazione
5. Intregazione del modulo con l'applicativo MetaClass.

Nella repository in "MetaClassAI_Documentazione" è presente una documentazione in cui vengono mostrati in modo dettagliato tutti i passaggi descritti prima includendo anche righe di codice estratti da MetaClass.

Infine saranno presenti delle immagini che mostrano i plot utilizzati per l'analisi dei dati. 

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








