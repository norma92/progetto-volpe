# progetto-volpe

dopo aver creato un progetto springboot
avvio la classe che contiene il main
<br><br>
<img width="298" alt="01 - avvio applicazione" src="https://user-images.githubusercontent.com/91018701/225995401-f4852e6f-c601-462a-9437-f8b33cfb6fd8.png">
<br><br><br>
clicco direttamente sulla classe per essere sicura che venga avviata PROPRIO quella classe.. e dimentico di usare di nuovo il run, per non andare a usare una porta già in uso
<br><br>
<img width="1166" alt="02 - avvio java application" src="https://user-images.githubusercontent.com/91018701/225995867-21cbf994-5f43-4247-ad2f-824f0f230f0e.png">
<br><br><br>
per ogni package che dovrò creare devo accertarmi di aver selezionato il package principale
<br><br>
<img width="740" alt="03 - creazione package" src="https://user-images.githubusercontent.com/91018701/225998972-881df4e6-faab-4563-97e7-9f5eb8cd9120.png">
<br><br><br>
creo un package .models in cui inserirò le classe pojo
<br>che ottengo trasformando i file da formato JSON a Java
<br><br>
<img width="880" alt="creazione models" src="https://user-images.githubusercontent.com/91018701/226010794-c2864962-95cc-4288-8821-bef2e49c7d78.png">
<br><br><br>
copiando il link nell'url ottengo il file in formato JSON
<br><br>
<img width="660" alt="04 - file JSON" src="https://user-images.githubusercontent.com/91018701/226001200-0fe1af1b-e744-4338-9617-487b3867a61e.png">
<br><br><br>
una volta selezionati i dati non elaborati
<br><br>
<img width="636" alt="05 - dati non elaborati" src="https://user-images.githubusercontent.com/91018701/226001224-5028062b-a6e1-4ffd-8217-0a236bed1fd7.png">
<br><br><br>
li passo a Json2CSharp (https://json2csharp.com/code-converters/json-to-pojo) per convertirli in formato Java
<br>quello che ottengo è una classe pojo:
<br><br>
<img width="1026" alt="06 - deserializzazione" src="https://user-images.githubusercontent.com/91018701/226001258-ec0fdfdb-e268-4120-9cad-8ddb02782094.png">
<br><br><br>
copio i suoi attributi nella classe creata in .models
<br><br>
<img width="793" alt="creazione classe pojo" src="https://user-images.githubusercontent.com/91018701/226011117-b4f32e7d-4b1d-406e-b4ec-d6a8e83c036b.png">
<br><br>
<img width="574" alt="creazione pojo" src="https://user-images.githubusercontent.com/91018701/226011229-d1ea5c98-b4e9-43b5-ad19-65ad1be3ab02.png">
<br><br><br>
cambiando i modificatori di visibilità a PRIVATE
<br>
e sfrutto lombok per creare i setters, i getters, il toString (@Data), il costruttore parametrizzato (@AllArgsConstructor) e il costruttore di default (@NoArgsConstructor)
<br><br>
<img width="409" alt="fine pojo" src="https://user-images.githubusercontent.com/91018701/226015445-157afe95-7edc-464e-a12e-6092a22974b6.png">
<br><br><br>
creo un altro package all'interno di quello principale che chiamo .service
<br><br>
<img width="897" alt="package service" src="https://user-images.githubusercontent.com/91018701/226018330-c10effc0-6b88-4d42-a800-edc8a1a3a806.png">
<br><br><br>
all'interno del quale creo una classe
<br><br>
<img width="877" alt="classe service volpe" src="https://user-images.githubusercontent.com/91018701/226019642-ab8c0873-e4d0-4132-9dfd-ae6b56f9527d.png">
<br><br><br>
che conterrà la logica dei metodi che verranno chiamati nell'url grazie alle rotte
<br>per far capire alla classe la sua funzione devo usare l'annotazione @Service
<br><br>
<img width="555" alt="service annotation" src="https://user-images.githubusercontent.com/91018701/226020185-fb0bd166-d357-433e-87d9-58f8f927ed7f.png">

