Rappresentazione dei numeri, vengono classificati come 
- binaria -> b=2 rappresentate da cifre  **0  e 1**
- ottale -> b=8 rappresentate da cifre **da 0 a 7**
- esadecimale -> b=16 rappresentate da cifre da **0 a F (15)**
La codifica delle cifre si utilizza la numerazione **binaria (2)** la rappresentazione in bit è uguale per qualsiasi base.
il numero di bit cambia in base alla **cardinalità dell'insieme**, cosa significa?
Ad esempio, se consideriamo numeri binari di lunghezza 3 bit, l'insieme contiene 2^3 = 8 possibili combinazioni binarie diverse, che vanno da 000 a 111. La cardinalità di questo insieme è 8, poiché ci sono 8 elementi unici in quell'insieme..
Esso mira a semplificare le manipolazioni per eseguire operazioni sulla macchina.
ad ogni numero  viene associata la stringa di bit che lo rappresenta nel sistema binario.
Overflow.
L'overflow è una situazione che si verifica quando si lavora con numeri in un sistema di rappresentazione numerica, come i numeri binari, e il risultato di un'operazione supera la capacità massima di rappresentazione del sistema.
In altre parole, quando il risultato di un calcolo è troppo grande per essere contenuto nei bit disponibili per la rappresentazione.
Ad esempio, in un sistema a 8 bit, il numero binario 11111111 rappresenta il numero massimo che può essere rappresentato, che in decimale è 255. Se si tenta di sommare 1 a questo numero, si verificherà un overflow, poiché il risultato (256) non può essere rappresentato in 8 bit e il sistema non è in grado di gestirlo correttamente. Questo può portare a risultati imprevisti o errati nelle operazioni matematiche e può causare problemi nei calcoli in sistemi digitali come computer o microcontrollori.
Esso può essere rilevato attraverso il **bit di overflow**
esempio;
0110+
1000 = 1110

1110+
0011 = 10001

(1)0001, quell'1 è **l'overflow**


*Rappresentazione in modulo e segno*
è la codifica in segno e modulo su  numero n bit - ovviamente quello più significativo.
mentre per il segno n-1 per il modulo.
Occorre operare separatamente sul segno e sul modulo, in due momenti diversi.
bisogna effettuare la somma tra due numeri di segno discorde, e determinare quello col modulo maggiore così da sottrarre ad esso il modulo dell'altro.
il risultato **deve assumere il segno dell'addendo maggiore in modulo**.
*complemento a due*
- i numeri positivi  0<=x=2^n-1, il numero stesso
- i numeri negativi -2^n-1<=x<=0, il numero x=2^n - x
Rappresentazione sulla base di 4 bit;
![[Pasted image 20231023163856.png]]

**Complementi diminuiti**
La rappresentazione in complementi diminuiti è una tecnica utilizzata per rappresentare i numeri negativi in forma binaria. Questo sistema rappresenta i numeri utilizzando due complementi, il complemento a uno e il complemento a due. Questi metodi consentono di rappresentare sia numeri positivi che negativi, ma con l'uso di una singola rappresentazione binaria.

- Complemento a uno: Per rappresentare un numero negativo, si invertono tutti i bit (0 diventa 1 e viceversa). Poi, si aggiunge 1 al risultato. Questo metodo è utile per eseguire operazioni aritmetiche come l'addizione e la sottrazione.
    
- Complemento a due: Questo è simile al complemento a uno, ma senza l'aggiunta di 1 al termine. Invece, si invertono i bit e si usa il risultato diretto come rappresentazione del numero negativo. Il complemento a due è più comune in architettura dei calcolatori e semplifica le operazioni di somma e sottrazione.
    

Usando questi complementi diminuiti, è possibile rappresentare sia numeri positivi che negativi in modo efficiente all'interno di un sistema binario, rendendo possibile l'aritmetica binaria completa.
![[Pasted image 20231106162713.png]]
Il risultato dell'aritmetica binaria completa deve essere corretta qualora fosse negativo, si aggiunge **1** al risultato.
se entrambi gli addendi sono negativi -> si genera un **OVERFLOW**
se un addendo è positivo e uno negativo, effettuando la somma il risultato è positivo -> si genera un **OVERFLOW**Caso contrario, se sommando uscisse un risultato negativo, non si genererà l'overflow e non ci sarà bisogno della correzione.
In sintesi, L'OVERFLOW, può essere visto come la metrica per effettuare una correzione sull'aritmetica binaria.

**Rappresentazione in eccesso -K**
La rappresentazione in eccesso-K (o anche detta rappresentazione con eccesso) è un metodo utilizzato per rappresentare i numeri in modo binario, in cui un valore positivo viene rappresentato aggiungendo un valore fisso K. Questo metodo consente di rappresentare sia numeri positivi che negativi in un unico sistema binario, semplificando alcune operazioni aritmetiche.

Nella rappresentazione in eccesso-K, K è un valore costante che viene sommato al numero da rappresentare. La rappresentazione di un numero positivo sarà quindi uguale al valore numerico più K, mentre la rappresentazione di un numero negativo sarà inferiore al valore numerico più K. Questo rende possibile la rappresentazione di numeri positivi e negativi nello stesso spazio di rappresentazione binaria.

Ad esempio, se utilizziamo una rappresentazione in eccesso-3 con numeri decimali:

- Il numero 5 sarebbe rappresentato come 8 (5 + 3).
- Il numero -2 sarebbe rappresentato come 1 (-2 + 3).

La rappresentazione in eccesso-K è preferibile utilizzarla laddove sono richieste operazioni sono somme algebriche e confronti logici.
Ad esempio; rappresentazione in virgola mobile.
rappresentazione in eccesso 8 su 4 bit.
![[Pasted image 20231106163229.png]]
**I numeri a virgola fissa** sono un tipo di rappresentazione numerica in cui un numero è rappresentato utilizzando una lunghezza fissa di cifre decimali (o binarie) dopo la virgola. Questa rappresentazione è utilizzata quando si desidera una precisione costante in tutte le operazioni aritmetiche.
Si rappresentano in maniera **SEPARATA** , dividendo la parte intera e la parte frazionata di un numero reale.
**Numeri razionali**
- *Insieme denso* - >   
Un insieme denso è un concetto matematico utilizzato nell'ambito della topologia e dell'analisi matematica. In termini semplici, un insieme denso è un sottoinsieme di uno spazio topologico in cui ogni punto dello spazio può essere "avvicinato" da punti nell'insieme denso. In altre parole, qualsiasi punto dello spazio topologico può essere approssimato da punti dell'insieme denso in modo molto vicino, quindi anche se si scegliesse un intervallo limitato non tutti i numeri all'interno di esso potranno essere rappresentati.
- *approssimazione* - >
l'approssimazione si riferisce a una tecnica che può essere utilizzata per semplificare calcoli complessi al fine di migliorare le prestazioni del sistema o ridurre la complessità hardware o software. Questa tecnica può coinvolgere l'uso di valori approssimati anziché valori esatti per eseguire calcoli.

Ecco alcune aree in cui l'approssimazione può essere applicata in architettura dei calcolatori:

1. **Arrotondamento**: In molti calcoli numerici, specialmente quelli che coinvolgono calcoli in virgola mobile, si possono utilizzare tecniche di arrotondamento per rappresentare numeri reali con una precisione limitata. Ad esempio, è possibile approssimare un numero reale troncandolo alle prime cifre decimali.
    
2. **Approssimazione di funzioni matematiche**: Alcune funzioni matematiche complesse possono essere approssimate da funzioni più semplici o mediante serie di Taylor per ridurre il carico computazionale in operazioni di calcolo.
    
3. **Compressione dei dati**: Nella compressione dei dati, l'approssimazione è spesso utilizzata per ridurre la quantità di dati necessari per rappresentare informazioni, riducendo leggermente la precisione dei dati.
4. **ERRORE ASSOLUTO** -> piccolo su numeri piccoli, grande su numeri grandi
5. **ERRORE RELATIVO** -> costante su tutto l'asse di rappresentabilità.
    

L'approssimazione in architettura dei calcolatori è spesso un compromesso tra la precisione e le risorse disponibili, poiché l'utilizzo di valori approssimati può ridurre il tempo e le risorse necessarie per effettuare calcoli, ma può anche introdurre errori accettabili per applicazioni specifiche. La scelta di quando e come utilizzare l'approssimazione dipende dall'applicazione e dai requisiti specifici del sistema.
Quindi, **l'approssimazione** associa ad un numero del suddetto intervallo la rappresentazione di un numero ''più vicino'' cioè quello che riesce ad approssimare meglio -> errore di approssimazione.
* *Underflow* - >
L'underflow è un termine utilizzato in informatica e nell'ambito delle rappresentazioni numeriche per descrivere una situazione in cui un valore numerico diventa troppo piccolo per essere rappresentato in modo accurato usando la convenzionale rappresentazione in virgola mobile o in virgola fissa.

Nel contesto della rappresentazione in virgola mobile, l'underflow si verifica quando un numero, dopo una serie di operazioni matematiche, diventa così piccolo che non può essere rappresentato con una precisione sufficiente all'interno del sistema di rappresentazione in virgola mobile. Questo comporta la perdita di cifre significative e la rappresentazione finale del numero potrebbe essere zero o molto vicina a zero. L'underflow può portare a risultati inattendibili in calcoli scientifici o ingegneristici, in quanto i risultati possono essere influenzati da errori di approssimazione.

Nel contesto della rappresentazione in virgola fissa, l'underflow si verifica quando un valore supera il limite inferiore della rappresentazione, che è di solito zero. Questo può causare problemi in operazioni di sottrazione o divisione, in quanto il risultato potrebbe essere fuori dal range di rappresentazione valido.
Quind come si verifica un underflow? Quando a causa di un **errore di approssimazione** viene rappresentato con 0 un numero prossimo a zero.
**Numeri reali in virgola mobile**
un numero reale può essere rappresentato come;
(m,e):x=mxb^e
dove;
m - > è detta *mantissa* -- 
e -> è detta esponente -- 
b -> è la base di numerazione adottata
Questa rappresentazione viene indicata come **codifica in virgola mobile** 

**Standard IEEE**
Lo standard IEEE 754 è uno dei più importanti standard nell'ambito della rappresentazione e dell'aritmetica dei numeri in virgola mobile nei calcolatori. È stato sviluppato dall'Institute of Electrical and Electronics Engineers (IEEE) ed è utilizzato ampiamente per definire come i calcolatori dovrebbero rappresentare, manipolare e eseguire operazioni su numeri in virgola mobile.

Ecco alcuni aspetti chiave dello standard IEEE 754:

1. **Formato dei numeri in virgola mobile**: Lo standard definisce i formati per la rappresentazione dei numeri in virgola mobile. Questi formati includono bit per il segno, l'esponente e la mantissa (parte frazionaria). Ci sono formati a singola precisione (32 bit) e doppia precisione (64 bit) tra i più comuni.
    
2. **Operazioni aritmetiche**: Lo standard stabilisce regole per le operazioni aritmetiche come l'addizione, la sottrazione, la moltiplicazione e la divisione tra numeri in virgola mobile. Le operazioni devono essere eseguite in conformità con le specifiche dello standard per garantire la coerenza tra calcolatori diversi.
3. 1. **Precisione e arrotondamento**: Lo standard stabilisce regole per l'arrotondamento dei risultati delle operazioni al fine di garantire una certa precisione. Questo è importante per gestire l'errore di rappresentazione nei calcoli in virgola mobile.
    
4. **Conformità**: Gli sviluppatori di hardware e software devono seguire le specifiche dell'IEEE 754 per garantire che le operazioni in virgola mobile siano conformi allo standard e che i risultati siano coerenti tra diverse piattaforme.
ESEMPIO PRATICO.
Supponiamo di voler sommare i seguenti due numeri in virgola mobile IEEE 754:

Numero 1:

- Segno: Positivo (+)
- Esponente: 10000000 (rappresentato in binario come 01111111)
- Mantissa: 11000000000000000000000 (rappresentata in binario come 1.75 in decimale)

Numero 2:

- Segno: Positivo (+)
- Esponente: 10000001 (rappresentato in binario come 10000000)
- Mantissa: 10000000000000000000000 (rappresentata in binario come 1.5 in decimale)

Passo 1: Verifica il segno dei due numeri. Entrambi sono positivi, quindi il segno del risultato sarà positivo (+).

Passo 2: Confronta gli esponenti. Sottrai l'esponente del numero 2 da quello del numero 1:

Esponente del risultato = 10000000 - 10000001 = -1 (rappresentato come 01111110 in binario).

Passo 3: Esegui l'operazione di somma tra le mantisse, aggiungendo un bit nascosto "1":

Mantissa del risultato = 11000000000000000000000 + 10000000000000000000000 = 10100000000000000000000 (rappresentato come 1.25 in decimale).

Passo 4: Normalizza il risultato. Poiché il bit nascosto è stato spostato verso sinistra, aggiorna l'esponente in base alla quantità di spostamenti:

Nuovo esponente = -1 - 1 = -2 (rappresentato come 01111101 in binario).

Pertanto, il risultato della somma di questi due numeri in formato IEEE 754 a singola precisione è:

- Segno: Positivo (+)
- Esponente: 01111101
- Mantissa: 10100000000000000000000 (1.25 in decimale)




