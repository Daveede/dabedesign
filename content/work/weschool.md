---
title: "Weschool UX"
date: 2021-10-02T18:08:43+01:00
draft: false
featured_image: "weschool.png"

---
WeSchool è una piattaforma utilizzata principalmente da due tipi di utenti, studenti e insegnati, il goal della piattaforma è però unico, da un lato facilitare e potenziare l'insegnamento di docenti e l'apprendimento degli studenti attraverso l'utilizzo di strumenti digitali forniti dalla piattaforma. In questa analisi andremo ad analizzare il lato dedicato ai docenti e a tutti gli strumenti a loro disposizione.

---

## Sitemap
La sitemap (visitabile a questo [link](https://www.gloomaps.com/aHpikfmnfs)) ci fa subito notare un gran numero di funzioni in primo piano. diverse di queste però non vanno hanno una funzione primaria e non aiutano l'utente a raggiungere il proprio goal.

![ ](https://dabe.design/images/vecchiasitemap.png)

Sarebbe bene quindi spostare queste funzioni in un livello inferiore per mantenere l'interfaccia il più possibile pulita e libera da distrazioni.

![ ](https://dabe.design/images/nuovasitemap.png)


---


## Log-in

Subito dopo esserci registrati e aver effettuato il login, veniamo reindirizzati alla pagina dei gruppi. I gruppi hanno la funzione di creare delle "community" di docenti e/o studenti dalla quale il docente ha la possibilità di creare esercizi, verifiche, avviare delle stanze attraverso i principali servizi di videoconferenza e assegnare delle scadenze, infine la presenza di una bacheca, dove gli studenti possono fare domande e avviare conversazioni con il docente.



![ ](https://dabe.design/images/gruppivanilla.png)

Manca però la possibilità di creare delle sezioni e categorie per meglio organizzare i gruppi, questa pagina tenderà inevitabilmente a popolarsi di numerosi gruppi, che mischiandosi tra gruppi di studenti e docenti potrebbe diventare confusionaria.  

![ ](https://dabe.design/images/gruppi.png)

Uno step successivo potrebbe l'integrazione con l'orario delle lezioni del docente, così da avere i gruppi dedicati alle classi in primo piano al momento del bisogno.

---

## Navigation System

![ ](https://dabe.design/images/hamburger.png)


Alla destra troviamo un hamburger menu, che nasconde la barra di ricerca, il link "I miei gruppi", "profilo", "impostazioni" e "help", l'hamburger menu è un menu inventato dal Norm Cox, per lo Xerox Star (il primo computer ad interfaccia grafica), è rientrato in auge con l'avvento dei primi smartphone ora però, sta di nuovo "morendo", aggiunge infatti diversi step alla navigazione, rallentandola e nascondendo informazioni e funzioni importanti. L'hamburger menu presenta dei problemi di reachability, il pulsante per raggiungerlo si trova infatti nella parte meno raggiungibile dello schermo, problema che peggiora ogni anno con l'aumentare delle dimensioni dello schermo come mostra l'immagine sottostante.

![ ](https://dabe.design/images/rechability.png)


L'eliminazione dell' hamburger menu permette all'utente di avere più funzioni sempre a portata di mano, migliorandone l'efficienza, sia da desktop che da mobile, dove una *tab-bar* presente nella parte inferiore dello schermo lo sostituisce.

![ ](https://dabe.design/images/hamburgeraggiornato.png)
In questo modo la barra di ricerca è sempre in vista, la pagina "i miei gruppi" diventa una homepage accessibile tramite il logo WeSchool e le informazioni di secondaria importanza come la modifica del profilo o le impostazioni sono nascoste dietro un click in alto a destra.

---

## Gruppi

All'interno dei gruppi troviamo in primo piano la bacheca che occupa maggior parte dell'interfaccia a destra possiamo invece avviare una videoconferenza, creare una scadenza e una lista dei membri del gruppo.



#### Scadenze

Le scadenze possono essere utilizzate dai docenti per assegnare compiti a casa, ufficializzare date di compiti in classe e verifiche, assegnargli una data e allegare un documento di vario formato, non è però possibile visualizzare uno storico di tutte quelle che sono le scadenze passate che arrivate al loro termine, spariscono.

---

## Perdita di progressi

Durante la creazione di test è molto facile per un docente perdere tutte le domande e i progressi creati, per motivi relativamente banali, come l'apertura della chat o delle notifiche che reindirizzano in sezioni diverse di WeSchool.
Il problema è facilmente risolvibile spostando la chat e le notifiche (anche quelle già lette) in un popup dedicato o un *modal* per sollecitare il salvataggio dei dati.

![ ](https://dabe.design/images/modaltest.png)
*Modal salvataggio dati*

![ ](https://dabe.design/images/popupchat.png)
*Chat popup*

---

## Pulsante indietro

Troviamo in diverse parti dell'interfaccia desktop, un *back button*, che su mobile ritroviamo su numerosissime interfacce, è più inusuale invece ritrovarlo su browser desktop dove gli utenti sono abituati a cliccare sul più tradizionale *back button* del browser.
Il pulsante inoltre non agisce solo per riportare l'utente ad una schermata di livello superiore ma funziona come un tradizionale indietro, ma può portare l'utente fuori dalla piattaforma se si accede direttamente ad una schermata interna al sito come mostrato nella gif.

![ ](https://dabe.design/images/indietro.gif)

Il pulsante indietro può essere sostituito su desktop, da un breadcrumb, che mostra il percorso che l'utente ha fatto per raggiungere quella pagina.
![ ](https://dabe.design/images/breadcrumb.png)


---

## Azioni distruttive

Con il passare del tempo gli utenti sviluppano il cosiddetto "habitual tapping".</br>
L' *habitual tapping* rende facile completare i compiti più velocemente e senza pensare. Ma rende anche più facile toccare accidentalmente i pulsanti con azioni distruttive. È bene quindi allontanare tutte le azioni distruttive dalle azioni che non lo sono e segnalarle di rosso, colore normalmente associato col pericolo per evitare i click accidentali.

![ ](https://dabe.design/images/destructive.png)
*Interfaccia attuale*


![ ](https://dabe.design/images/fixed.png)
*Azioni distruttive modificate*

---

## Inconsistenze

Nella piattaforma sono presenti diverse inconsistenze, in particolar modo, nei menù contestuali e il modo in cui essi vengono segnalati, checkbox e switch. Questo crea dei flow inconsistenti e confusione negli utenti oltre che a sviluppatori e designer, costretti a mantenere diversi componenti che eseguono la stessa azione.

![ ](https://dabe.design/images/context.png)

![ ](https://dabe.design/images/Check.png)

---


## Conclusioni

WeSchool è una piattaforma pensata per docenti e studenti, ha bisogno di essere di facile comprensione e utilizzo, adopera però un' *Navigation System* (hamburger menu)non al passo con gli standard di usability (specialmente mobile). </br>

I user flows potrebbero essere ulteriormente estremizzati, riducendone gli step e aumentandone l'efficienza.
</br> Presenta inoltre diversi punti in cui viene a mancare la coesione del design system e dei componenti, con un diverso numero di componenti che effettuano lo stesso step, riducendo l'*expected behaviour*, costringendo l'utente a navigare con attenzione l'interfaccia.
