Anteckningar från arbetsmöte
============================

2020-03-13 Zoom\
Vid protokollet: Tomas Snäckerström\

Per inledde mötet med att hälsa alla välkomna och föreslog att vi rent praktiskt skulle fortsätta mötet utifrån det gemensamma mötet i Göteborg.
 
Praktiska frågor om teknik
--------------------------

Per meddelade att alla som fick X-konto nere i Göteborg ska kunna komma åt nätverket genom att ansluta med rätt VPN-client(Cisco AnyConnect).
Det finns en instruktion om hur man ansluter publicerad i projektet (jag är dock inte med på exakt var).

Östergötland meddelade att de hade vissa problem med versionerna av SSL protokoll som de såg när de försökte ansluta, men det föreföll efter lite utredning sannolikt vara kopplat till lokal brandvägg. Övriga som testat hade inte mötts av samma fel.

_Actionpunkt_:\
Det beslutades gemensamt att alla får till uppgift att säkerställa inloggning på VPN:et.

Man behöver installera CiscoAnyconnect och sedan ansluta till https://asa.vpn.gu.se/

När man anslutit till VPN:et ska man verifiera att man kan nå maskinen genom att ansluta med ssh till maskinen:
````
   ssh -l <användarnamn> 10.248.210.5
````

Per har ännu inte lagt till alla i rätt behörighetsgrupp i AD:t så det kan hända att inloggningen inte lyckas men bara att man får ett svar visar att man är på rätt nätverk och därmed ha lyckats ansluta till VPN:et. Nätverksinstöällningarna bör även visa en anslutning med en IP på samma subnät.

Introduktion och kunskapsöverföring
-----------------------------------

Per berättar att han i nästa vecka kommer att göra uppgraderingar i klustret och erbjuder alla att delta i pedagogiskt syfte. Det kan vara ett bra tillfälle att få en bättre allmän förståelse för vad det är vi har att arbeta med.

Detta mottogs mycket positivt och flera deltagare avser att försöka vara med. Per kommer att göra detta med delad skärm på Zoom 2020-03-16 kl 12-14 Mötesinbjudan skickad.


Fråga om maskiner och output
----------------------------
Vi höll en allmän diskussion kring skillnader i format och output från olika sekvensieringsmaskiner. Uppfattningen är att det är ganska spritt och inte helt klarlagt vad som använd var.

_Actionpunkt_:\
Vi behöver genomföra en kartläggning över vilka maskiner vi har på olika ställen och vilka versioner. 

Jens lägger upp info baserat på vad vi vet och detta behöver verifieras av alla för sina respektive organisationer.


Diskussion kring upplägget och arbetsordning
--------------------------------------------

Tomas uttryckte en känsla av att sakna överblick ifråga om projektets övergripande mål och hur olika delar hänger ihop i arbetet mot målet. Detta ledde till en gemensam diskussion kring hur projektet är uppdelat och vilka områden som hör till vad. 

Per presenterade att han såg några olika och ganska tydliga delar i det delprojekt som kallas "AP2". I en gemensam diskussion identifierade vi fyra övergripande områden som ska arbetas med i arbetspaketet.

Efter diskussion enades mötet om att formulera fyra huvudområde som projektet arbetar inom och föreslog ansvariga deltagare enligt nedan.\
 
**Praktisk uppgift att skapa konnektivitet**\
Detta arbetspaket berör frågor om praktisk anslutning av system för deltagande enheter. Arbetet innefattar att utveckla system och komponenter för att underlätat enheternas anslutning till lagringsmiljön samt för att överföra data från sekvensieringsinstrumenten.

Deltar i denna del gör:

- *Vilma* 
- Mårten
- Isak
- Jens
\

**Informatik**\
Arbetsområde informatik berör frågor relaterade till inforamationsstandarder och struktur för informationen. Arbetet ska definiera format och protokoll för överföringen av information både avseende insamling och resultatrapportering. Erik leder arbetet med stöd av Tomas. Domänkunskap och stöd för frågor om specifikt bioinformatik ges i första ledet av Vilma.

Deltar i denna del gör:

- *Erik*
- Tomas
- Vilma
\

**Akritektur för NGP**\
Arbetsområdet avser att besluta om och dokumentera den övergripande arkitekturen för systemet. 

Deltar i denna del gör:

- *Per*
- Tomas
- Henrik
\

**Pipeline Mikro**\
Detta arbetsområde avser att genomfrös en praktisk pilot där hela kedjan testas för ett antal analyser inom området mikrobiologi.

Deltar i denna del gör:

- *Isak*
- Jens
- Mårten
- Jenny/Tobias
