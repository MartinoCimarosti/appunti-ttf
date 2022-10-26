-Xml è un linguaggio di markup, con uno schema.
-Metalinguaggio, linguaggio che io uso non per descrivere oggetti ma linguaggi.
-Derivato dall'html

Creato per utilizzare il paradigma del tag (<>) anche in altri contesti.
Descrivere generici dati strutturati.
In xml esistono solo tag custum, vengono inventati dallo sviluppatore.

_xml non è un sostituto per html_, I metadati mi danno semplicemente un operazine operativa.

![[Pasted image 20221026112212.png]]

Riusciamo agevolmente a tirare fuori roba da questo XML (leggendo i tag tiro fuori i contenuti)

## Elementi

L'elemento xml è tutto quello che è incluso tra un tag di apertura e un tag di chiusura.
I TIPI di  element sono:

- Element: Se il contenuto dell'elemento  sono latri tag
- Simple content: Se il contenuto contiene soltanto testo.
- Empty: Elemnto vuoto(tag con slash finale)
- Mixed: Misto tra element e symbol (alternanza di testo e sottolementi).


## Attributi

Possono figurare negli attributi o nei tag vuoti (es src="bamba.png" in html)
![[Pasted image 20221026113737.png]]

Gli attributi sono più difficili da estendere e non possono avere dati sturtturati (continene  solo testo) quindi ad esempio non posso tenere un xml, nell'elemento ovvero posso ma non è nello standard e ha poco senso.



## Regole Semantiche XML

- I tag vanno chiusi
- I tag vanno chiusi in ordine (FILO)
![[Pasted image 20221026114720.png]]
- Ogni documeno XML ha una ed una sola Root
- Se concatento due xml non ottengo più un xml, devo inventarmi una nuova radice
- Case Sensitive
- Spazi/Invii preservati
- E' possibile fare escaping (evitare di spaccare il codice, usare dei termini che in un contesto hanno un particolare funzionamento nel codice)
![[Pasted image 20221026115405.png]]

 _Questi vincolo mi permettono di trattare in maniera omogena l'XML in vari programmi e linguaggi di programmazione_




XML differisce da JSON perchè posso definire uno schema, a differenza di json, per vedere se il documento che è quello che voglio.
Ad esempio nel 
![[Pasted image 20221026112212.png]]
Vado a definire lo schema di una **"nota"** come una roba che contiente un **to** un **from** un **title** ed un **message**.

![[Pasted image 20221026122154.png]]
Si fa un controlo tramite Software per verificare prima che il mio file XML sia valido(supporti le regole semantiche di XML, verifica di buona forma) e poi si fa una **validazione**, che prende in ingresso il mio file.xml e il mio **schema** e ottengo un altra validazione (ok il tuo xml è/non è una nota).


## Definire un Linguaggio XML

Posso definire ad esempio cosa per me è una nota.
Per definire un XML posso usare ad esemip un [[DTD]].
