# Kom igång med ESP8266 och Arduino IDE

Den här guiden hjälper dig steg för steg att komma igång med din ESP8266 och Arduino IDE, även om du aldrig har programmerat eller använt Arduino förut.

## Innehållsförteckning
1. [Vad  är ESP8266](#vad-är-esp8266)
2. [Vad är Arduino IDE](#vad-är-arduino-ide)
3. [Vad du behöver](#vad-du-behöver)
4. [Installera Arduino IDE](#installera-arduino-ide)
5. [Installera ESP8266-stöd i Arduino IDE](#installera-esp8266-stöd-i-arduino-ide)
6. [Anslut ESP8266 till din dator](#anslut-esp8266-till-din-dator)
7. [Ladda upp din första kod till ESP8266](#ladda-upp-din-första-kod-till-esp8266)

## Vad är ESP8266?
ESP8266 är en kraftfull mikrokontroller med inbyggt Wi-Fi. En mikrokontroller är en liten dator som innehåller en processor (CPU), minne och in- och utgångar. Den är designad för att styra andra enheter och utföra specifika uppgifter, som att läsa sensorer eller styra motorer och lampor mm.

## Vad är Arduino IDE?
Arduino IDE (Integrated Development Environment) är ett användarvänligt programmeringsverktyg som används för att skriva, kompilera och ladda upp kod till Arduino-kompatibla mikrokontroller, inklusive ESP8266. Det är särskilt utformat för nybörjare, med ett enkelt gränssnitt och många exempel och bibliotek som gör det enkelt att komma igång med hårdvaruprogrammering. Arduino IDE stöder flera programmeringsspråk, men använder främst en variant av C++.

## Vad du behöver

För att komma igång behöver du följande:
- En dator (Windows, macOS eller Linux)
- En USB-kabel
- Ett ESP8266-utvecklingskort
- Arduino IDE (gratis programvara för att programmera din ESP8266)

## Installera Arduino IDE

1. Gå till [Arduino-webbplatsen](https://www.arduino.cc/en/software) och ladda ner Arduino IDE för ditt operativsystem (Windows, macOS eller Linux).
2. Installera programmet genom att följa instruktionerna på skärmen. För de flesta är det bara att klicka "Nästa" och "Installera" tills installationen är klar.
3. När installationen är klar, öppna Arduino IDE.

## Installera ESP8266-stöd i Arduino IDE

Nu när du har Arduino IDE installerat behöver du lägga till stöd för ESP8266 så att du kan programmera ditt kort.

1. Öppna Arduino IDE om du inte redan gjort det.
2. Gå till `Fil` > `Preferences` 
3. I rutan som heter "Ytterligare URL:er till Board Manager", klistra in följande URL: https://arduino.esp8266.com/stable/package_esp8266com_index.json
Klicka på `OK`.
4. Gå till `Verktyg` > `Kort: "xxx"` > `Kortadministratör`.
5. I sökfältet, skriv `esp8266`. När ESP8266-paketet dyker upp, klicka på `Installera`.
6. Vänta tills installationen är klar, detta kan ta några minuter.

## Anslut ESP8266 till din dator

1. Anslut din ESP8266 till datorn med USB-kabeln.
2. I Arduino IDE, gå till `Verktyg` > `Kort: "xxx"` och välj ditt ESP8266-kort (t.ex. "NodeMCU 1.0" eller "WeMos D1 R2 & mini").
3. Gå till `Verktyg` > `Port` och välj den port som ditt ESP8266-kort är anslutet till (vanligtvis COM3, COM4, etc. på Windows eller `/dev/cu.usbserial-xxxx` på macOS).

## Ladda upp din första kod till ESP8266

Nu ska vi ladda upp ett enkelt exempel som blinkar en LED på ditt ESP8266-kort.

1. I Arduino IDE, gå till `Fil` > `Exempel` > `01.Basics` > `Blink`.
2. Koden som öppnas är ett enkelt program som får den inbyggda LED-lampan på ESP8266 att blinka.
3. Klicka på `Pilen` (ladda upp) i övre vänstra hörnet för att kompilera och ladda upp koden till ditt ESP8266-kort.
4. Vänta medan koden kompileras och laddas upp. Du ser en status längst ner i Arduino IDE-fönstret.
5. Om allt fungerar som det ska kommer LED-lampan på ditt ESP8266-kort att börja blinka.


