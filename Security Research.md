# Security Research
![Cyber security header_1920x1280px (1)](https://user-images.githubusercontent.com/99720686/173595792-05216ab6-c25e-4718-b00d-96d6d1b001c3.jpg)

<h2 align="center">Inleiding</h2>

In dit document zal ik onderzoek naar hoe ik de veiligheid van mijn gebruikers beter kan beveiligen om specifiek te zijn gaat het om de persoonlijke data van een gebruiker. Dit is ook op dit moment een serieus probleem in de wereld. Hieronder een stukje uit een artikel.

In navolging van de Senaat en het Congres, heeft ook de Amerikaanse president Donald Trump onlangs zijn handtekening gezet onder nieuwe regelgeving die het Amerikaanse internetproviders toestaat de surfgeschiedenis van burgers te verzamelen en te verkopen aan externe partijen. Zo’n schok zou dat eigenlijk niet moeten zijn, gebruikersdata worden immers al massaal gebruikt door internetconglomeraten als Google en Facebook voor dergelijke commerciële doeleinden. De Republikeinen zeggen het speelveld nu gelijk te willen trekken voor de internetproviders; ze worden slechts toegevoegd aan het reeds bestaande illustere lijstje van partijen die dergelijke persoonlijke informatie van burgers mogen exploiteren voor financieel gewin.

<hr>

<h2 align="center">Inhoudsopgave</h2>

<a href="#onderzoeksvraag">Onderzoeksvraag</a><br>

<a href="#1-authenticatie">1. Welke authenticatie service kan ik het beste gebruiken voor mijn gebruikers?</a><br>

<a href="#2-testen">2. Hoe kan ik testen dat de persoonsgegevens van mijn gebruikers veilig zijn?</a><br>

<a href="#3-risico">3. Aan welke beveiligingsrisico's komen gebruikers vaak in aanmerking voor?</a><br>

<a href="#4-veiligheid">4. Hoe zorg ik ervoor dat de persoonsgegevens van mijn gebruikers veilig blijft?</a><br>

<a href="#bron">Bronnenlijst</a>

<hr>

<h2 align="center" id="onderzoeksvraag">Onderzoeksvraag</h2>

In dit ondezoek ga ik opzoek naar manieren om de veiligheid van mijn gebruikers data beter te beveiligen Daaom luidt de onderzoeksvraag als volgt:

**Hoe zorg ik ervoor dat de persoonsgegevens van mijn gebruikers beter is beveiligd?**

<h3>Deelvragen</h3>

Om de hoofdvraag te kunnen beantwoorden, deel ik deze op in deelvragen:

<ul>
    <li>Welke authenticatie service kan ik het beste gebruiken voor mijn gebruikers?</li>
    <li>Hoe kan ik testen dat de persoonsgegevens van mijn gebruikers veilig zijn?</li>
    <li>Aan welke beveiligingsrisico's komen gebruikers vaak in aanmerking voor?</li>
</ul>

<hr>

<h2 align="center" id="1-authenticatie">1. Welke authenticatie service kan ik het beste gebruiken voor mijn gebruikers?</h2>

**QR CODE**
QR-code-authenticatie wordt meestal gebruikt voor gebruikersauthenticatie een flow die vaak wordt gebruikt bij het inloggen van de applicatie. Dit process geeft de optie wanneer je inlogt een QR code te weergeven en deze met bijvoorbeeld een smartphone te scannen om in te loggen.

**SMS OTP**
Deze eenvoudige maar effectieve authenticatiemethode omvat het verzenden van een sms-bericht naar de mobiele telefoon van de gebruiker, met daarin een eenmalig wachtwoord dat wordt gebruikt om de authenticatie van online betalingen te voltooien.

**PUSH NOTIFICATION AUTHENTICATION METHOD**
Een op push gebaseerd authenticatiesysteem stuurt een melding naar een app op het apparaat van een gebruiker en informeert hen over een authenticatiepoging. De gebruiker kan de details van de authenticatiepoging inspecteren en op basis van zijn kennis over bijvoorbeeld een transactie die plaatsvindt, kan hij de verificatie van het verzoek bevestigen of weigeren.

Voor deze deelvraag heb ik gebruik gemaakt van de library stategie en de best good and best practices methode.
<hr>

<h2 align="center" id="2-testen">2. Hoe kan ik testen dat de persoonsgegevens van mijn gebruikers veilig zijn?</h2>

Om zeker te zijn dat de persoonsgegevens van mijn gebruikers zal ik testen moeten gaan draaien om te kijken hoe veilig mijn gebruikers nou echt zijn. Om dit te testen zal ik gebruiken maken van tools die beschikbaar zijn op dit moment. Verschillende testen die ik zou kunnne gebruiken zijn. static testing, Database security testen en application security testen.

Voor deze deeling heb ik gebruik gemaakt van de library LAB en de methode Security test.
<hr>

<h2 align="center" id="3-risico">3. Aan welke beveiligingsrisico's komen gebruikers vaak in aanmerking voor?</h2>

Uit onderzoeken is gebleken dat gebruikers zelf ook vaak de oorzaak zijn van de risico's van hun eigen data. Dergelijke praktijken maken het volgens Zscaler makkelijk voor aanvallers om netwerken binnen te komen. In de praktijk maken veel aanvallen ook gebruik van menselijke fouten in de beveiliging van netwerken. Zo wisten de aanvallers achter de SolarWinds-hack ook beveiligingen te omzeilen door simpelweg veelgebruikte wachtwoorden te proberen op slecht beveiligde inlogpagina’s. Om dit nou tegen te gaan kun je als oplossing is om maandelijks een email te sturen naar je gebruikers om ze te herinneren wat de risico's zijn en aan te geven wat ze kunnen doen om dit tegen te gaan.

Om deze deelvraag te beantwoorden heb ik gebruik gemaakt van de Field strategie en de probleem analyse methode.
<hr>

<h2 align="center" id="conclusie">Conclusie</h2>

Als conclusie zijn er vele manieren om de persoonsgegevens van je gebruikers beter te beveiligen. Een stukje hiervan is om je applicaite te testen voor risico's. Dit kan met tools gedaan worden. Een stukje hiervan is ook authenticatie voor je gebruikers zodat het inloggen ook veiliger gaat. En het laatst is om je gebruikers zelf te educeren zodat zij ook op de hoogte zijn van de risico's zoals niet zomaar op een link te klikken die je binnen krijgt. Dit helpt ook al een heleboel.

<h2 align="center" id="bron">Bronnenlijst</h2>

Hoe veilig zijn wij en onze data eigenlijk online?: https://netwerkmediawijsheid.nl/hoe-veilig-en-data-eigenlijk-online/

TOP 5 most reliable and user-friendly authentication methods: https://cybersecurity.asee.co/blog/top-authentication-methods-in-online-payments/

10 Types of Application Security Testing Tools: When and How to Use Them: https://insights.sei.cmu.edu/blog/10-types-of-application-security-testing-tools-when-and-how-to-use-them/
