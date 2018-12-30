# microservice-project
progetto microservizi

Il progetto consiste di 4 microservizi:

1 un'interfaccia gui che orchestra i servizi 2 e 3 
2 un servizio che esegue crud su mongo db ed in particolare effettua una query individuando un valore in un range di date
3 un servizio che scrive su un topic kafka e che contiene un consumer che legge i messaggi appena scritti e li invia tramite mail ad un destinatario
4 un servizio di invio mail

Nella gui oltre all'autenticazione (username=Andrea e password=password) è presente un form che innesca tutti gli altri servizi.
I servizi sono collegati e orchestrati tramite client feign e predisposti al load balancing mediante client Ribbon una volta che verrà istallato un servizio di discovering
