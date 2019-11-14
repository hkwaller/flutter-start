# Flutter

Vi skal teste ut Flutter. For å være klare til møtet er det fint om dere laster ned og installerer Flutter før møtet begynner, sånn at vi kan komme igang med en gang.

## Hvordan?

- Last ned flutter [her](https://storage.googleapis.com/flutter_infra/releases/stable/macos/flutter_macos_v1.9.1+hotfix.6-stable.zip)
- Kjør `unzip ~/Downloads/flutter_macos_v1.9.1+hotfix.6-stable.zip` hvis den ligger i `Downloads`, oppdater ellers pathen til din zip fil. 
- Nå har du to valg. Hvis du kun vil teste Flutter denne gangen, følg 1), hvis du tenker _dette vil jeg teste flere ganger_, følg 2).

### 1) Legge til Flutter kun for gjeldene sessjon 
- Hvis du kun vil teste Flutter denne gangen kan du kjøre ```export PATH="$PATH:`pwd`/flutter/bin"```, det vil da kun fungere i gjeldende terminal sessjon. 

### 2) Legge til Flutter forever
- Åpne din `.bashrc` eller tilsvarende for `zsh` etc. 
- Legg til `export PATH="$PATH:[PATH_TO_FLUTTER_GIT_DIRECTORY]/flutter/bin"`. Merk at du må erstatte `[PATH_TO_FLUTTER_GIT_DIRECTORY]` med hvor mappen faktisk ligger. I mitt tilfelle var dette `/Users/hanneswaller/Downloads/flutter/bin`
- Gå ur `vim` eller `code` eller hva du brukte for å oppdatere filen
- Kjør `source $HOME/.bashrc` eller `source $HOME/.zshrc` eller hva det kan være.
- Sjekk om det fungerte ved å kjøre `echo $PATH`, flutter burde nå ligge i slutten av din PATH. 
- Hvis du ser flutter der, prøv `which flutter` - da burde du se noe á la `/Users/dittflottenavn/Downloads/flutter/bin/flutter`

## Videre installasjon
- Kjør `flutter precache` som laster ned litt nødvendigheter
- Sjekk status med `flutter doctor`
- Hvis denne dukker opp
![id_device](https://i.imgur.com/U6KlEV6.png)

Så kan du enten bare klikke avbryt, det skal funke fint uansett. Men den kan dukke opp flere ganger. Hvis det blir slitsomt så åpne _Sikkerhet & Personvern_ i dine instillinger og trykk på knappen hva den nå kan hete på norsk 🙃

![sikkerhet](https://i.imgur.com/1f0bLfr.png)

- Sjekk outputen fra `flutter doctor`, den forteller om hvilke SDKer du har for iOS og Android. Du trenger kun å installere for den plattformen du ønsker å utvikle på.
- Følg stegene [her](https://flutter.dev/docs/get-started/install/macos#platform-setup)
- Valider at du satt opp riktig med `flutter doctor`
- Burde se ut i hvert fall litt som dette:

![doctor](https://i.imgur.com/H3tO2ts.png)

- Nå skal du være klar for faggruppemøte!
