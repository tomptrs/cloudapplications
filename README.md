# cloud applications 

## Project background

Beschrijf alle doelstellingen

## Technology stack

beschrijf alle technologie die je in je project gaat gebruiken. Vb. ASP.NET CORE MVC, Angular, HTML5, CSS3,..

## Architectuur

Maak een schematische voorstelling van je software architectuur. Indien je gebruik maakt van ASP.NET CORE MVC kan je 
gebruik maken van de architectuur beschreven in volgende post: https://www.toptal.com/angular/angular-5-asp-net-core?utm_source=hs_email&utm_medium=email&utm_content=64754821&_hsenc=p2ANqtz--ulC07UR5v9iSLi8tmPZLo3o3pzi0hXRShrOK5KK5tU5qRxHOhQ-UYRliQEqeJNoO5b_Q950Dnt4yjy5BYEJZbJIu2OA&_hsmi=64754821

## Deployment Environment requirements

Beschrijf hier hoe je je software oplossing kan deployen

## Beschrijving requirements

Maak hier een lijst van user stories aan. Deze user stories worden gekoppeld aan mockups.
Al je user stories vormen je backlog in jira.ap.be

Vooraleer je aan de implementatie van een user story begint, is er nood om exact te weten wat er moet gebeuren: beschrijf dit zorgvuldig! Vb.


UserStory1: Als een gebruiker kan ik inloggen met een username en paswoord
1). Login: #UserStory1 
Screenshot: 01_Login_A.png
This will be a simple login to capture username and password
Display Remember Me and Forgot Password links
On input focus need display the gold border (Screenshot: 01_Login_B.png)
Create validation error, also update border to red (Screenshot: 01_Login_C.png)

# Waarop wordt er gelet tijdens de evaluatie

### Specificaties: gewicht:100

- zijn alle hoofdrequirements geïmplementeerd : gewicht:70
  => 0: Verschillende requirements ontbreken of werken niet. De meeste hoofdfunctionaliteit ontbreekt
  => 3: Enkele requirements zijn niet geïmplementeerd. Significante delen ontbrekne
  => 6: De meeste functionaliteit is geïmplenteerd, doch zijn er belangrijke features die ontbreken
  => 9: Alle functionaliteit kan worden gebruikt
 
- Zijn alle nevenrequirements geïmplementeerd: gewicht:30
  => 0: Verschillende minder prioritaire requirements zijn niet geïmplementeerd
  => 2: Enkele minder prioritaire requirements ontbreken
  => 4: Alle requirements zijn geïmplenteerd
  
 ### Technische requirements : "Code best practices": gewicht: 30
 
 - Worden coding best practices gevolgd. Elk project heeft nood aan een coding guideline,. Zowel code kwaliteit, als code styles zijn gedefinieerd (zie appendix code styling): gewicht: 30
  => 0: code guidelines bestaan niet
  => 1: code guidelines worden niet gevolgd
  => 2: code guidelines worden gevolgd, op enkele uitzonderingen na
  => 3: code guidelines worden gevolgd
  
 - Code commentaar: commentaar is nodig wanneer de code niet makkelijk begrijpbaar is. Bijvoorbeeld je maakt een klasse aan waarbij je niet in één oogslag kan zien wat juist de bedoeling van deze klasse is.  Commentaar mag niet buitensporig gebruikt worden. Als developer identificeer je zelf waar er uitleg nodig is. gewicht: 20
 => 0: verschillende code statements zijn onduidelijk en missen commentaar
 => 1: je geeft commentaar, maar je code wordt er niet duidelijker door
 => 2: je geeft commentaar, maar ook bij code die al duidelijk is
 => 3: je commentaar is nuttig, en dragen bij om de applicatie duidelijker te begrijpen
 
 - Onnodige code is opgeruimd: gewicht 10
 => 0: nee: code is niet opgeruimd
 => 1: ja: code is opgeruimd
 
 ### Deployment: gewicht 10
 - je heb je applicatie kunnen deployen, en hebt beschreven hoe dit te doen: gewicht 60
 => 0: beschrijving is moeilijk te begrijpen
 => 1: je beschrijving mist belangrijke stappen
 => 2: je beschrijving is goed, maar mist nog extra documentatie voor een beginner
 => 3: volledige beschrijving
 
 - je applicatie staat in de cloud: 40
 => 0: nee
 => 1: ja
 
 ## Testing: gewicht 20
 => 0: nee
 => 1: beperkt gebruik van unit testing
 => 2: je test de meeste functionaliteit in je business layer
 => 3: je test alle functionaliteit 
 
 
 # Deliverables
 
 - een document in PDF/Word/Markdown die een beschrijving geeft van je werk methodologie. (minimum 2 pagina's). Maak gebruik van schema's, grafieken, tabellen om je idee uit te leggen.
- deployment beschrijving
- Implementatie beschrijving (je kan gebruik maken van doxygen : http://www.doxygen.nl/)
- een step-by-step instructie gids hoe we je applicatie kunnen gebruiken
- Je code mag in elke programeertaal gebruikt worden. Doch de stakeholders hebben een voorkeur om ASP.NET CORE MVC in de backend te gebruiken.
- Al je bron code via github
- Alle project management taken via jira.ap.be
- eindpresentatie

# Appendix
 
 ## Code styling
 1. gebruik consistent indentation
 2. Maak gebruik van het DRY principe: don't repeat yourself. Hetzelfde stuk code mag niet herhaald worden
 3. Zorg ervoor dat je methodes niet te veel lijnen code bevatten. Refactor! Denk aan het Single Responsibility principe
 3. File / Folder structuur. Denk goed na over je sofware architectuur. Je code mag niet vervat zitten in 1 of 2 bestanden. Maak nieuwe projecten aan, en refereer in andere projecten naar deze.
 4. Naming convention: geef goede benaming aan je variabelen, en maak geen gebruik van vb. var x1, y2...
 
 ## Wat loopt er dikwijls mis
 1. Zorg ervoor dat je duidelijk weet hoe de user storie in elkaar zit. Zorg ervoor dat alle paden van de user story geïmplenteerd worden.
 2. Elke ontwikkelaar werkt aan een volledige user story. Dit wil zeggen dat je zowel frontend als backend code dient te schrijven.
 3.Verwijder onnodige code. Eens je user story werkt moet de code in commentaar verwijderd worden
 
 ## Voorbeeld projecten

Het is de bedoeling dat je zelf een project voorstel uitwerkt. Onderstaande voorbeeld projecten kunnen je hierbij helpen.

### City escape game
Via puzzels en gps routes moet je uit de stad ontsnappen. Via smartphones moet het spel speelbaar zijn. Maak gebruik van AR technologie om je city game uniek te maken. Het is belangrijk om een goede data bron (API) te vinden om de geschiedenis of toerisische attracties van de stad in je spel te kunnen betrekken.

### Question-App
Ooit al eens een vraag willen stellen, maar toch niet gedurfd omdat je dacht dat het een domme vraag was? Domme vragen bestaan niet! Met deze applicatie willen we een systeem ontwikkelen dat toelaat om online vragen te stellen in de klas. Hiervoor starten docenten een les op en en waarop studenten zich kunnen registeren. Vanafnu hebben studenten de mogelijkheid om vragen te stellen via de applicatie. Bij een nieuwe vraag worden alle studenten genotifieerd en kunnen ze deze vraag liken. Op deze manier ziet de docent welke vragen populair zijn. De docent heeft hiervoor een dashboard ter beschikking die een lijst van vragen toont gerankschikt op populariteit.
Verder wordt een history van vragen per les bijgehouden voor de docent, beschikbaar via een Restful API. Ook voorzie je in je API dat vragen over hetzelfde onderwerp worden samengebundeld over verschillende universiteiten en hogescholen heen. Deze moeten ook gerankschikt kunnen worden op populariteit (vb. % likes per aantal studenten in les..). Deze vragen zijn via de API beschikbaar. Een history van vragen bijhouden zonder antwoord zorgt voor enige frustatie. De antwoorden kunnen beoordeeld worden, maar ook de gebruikers die antwoorden posten worden beoordeeld. Het beoordelingssysteem van de app is bedoeld om wederzijds respect en
verantwoordelijkheid op het platform te bevorderen. Na het afronden van een les kan de docent telkens aan de studenten vragen om een score te geven: in hoeverre denk je deze leerstof te begrijpen (1, ik snap er niks van, 5: alles duidelijk), of bv. Snel enkele multiple choice vragen (die bv. Al op voorhand klaar staan) af te vuren waarop studenten klassikaal moeten antwoorden via de app zodat de docent snel feedback krijgt wat er duidelijk is en wat nog niet.

### Uber voor ijskarren
Uber voor ijskarren is een technologieplatform dat ijscoventers in contact brengt met mensen zin in een ijsje door middel van een webapplicatie. Het werkt als volgt. Je kan een ijsje aanvragen door middel van de app. Je aanvraag wordt verzonden naar een chauffeur in de buurt. Wanneer een chauffeur je aanvraag accepteert, wordt in de app vermeld hoe lang het ongeveer zal duren voordat de chauffeur aankomt op je ophaallocatie. De app geeft ook een melding wanneer de chauffeur bijna bij de ophaallocatie is. Nadat je een rit hebt aangevraagd, krijg je in de app de naam van de chauffeur, en bedrijfsnaam te zien, zodat je zeker weet dat je de juiste ijscocar hebt.
Wanneer je aankomt op je bestemming, eindigt je ijscorit. Direct na afloop van de rit vraagt de app je de ijscoman te beoordelen. Chauffeurs worden eveneens gevraagd hun passagiers te beoordelen. Het beoordelingssysteem van de app is bedoeld om wederzijds respect en verantwoordelijkheid op het platform te bevorderen.

 
 ## Links
 
Creating a Secure REST API in Node.js:
https://www.toptal.com/nodejs/secure-rest-api-in-nodejs?utm_source=hs_email&utm_medium=email&utm_content=65084081&_hsenc=p2ANqtz--jcfJBW9uzYCGLTD0XmwKtxnPiP7EBdMCxQ6DnzmOQ6Nr7FPwprC_LkpiLS5WB4EEQXfpjIEvfuPDwFH_m8ssu2-Lqgg&_hsmi=65084081

Scalable CSS
https://www.toptal.com/css/smacss-scalable-modular-architecture-css?utm_campaign=Toptal%20Engineering%20Blog&utm_source=hs_email&utm_medium=email&utm_content=65020470&_hsenc=p2ANqtz-8V-puyDKDK-zqXhXLCfwmY1xAAEwv-LtGCD3hxI5HTE0ESF8MyvDJVpfXRUrxM-xoUlkkSOKaZuUJKlEEFOPmptkNcTg&_hsmi=65020472

How to Do JWT Authentication with an Angular 6 SPA
https://www.toptal.com/angular/angular-6-jwt-authentication?utm_source=hs_email&utm_medium=email&utm_content=64754821&_hsenc=p2ANqtz--ulC07UR5v9iSLi8tmPZLo3o3pzi0hXRShrOK5KK5tU5qRxHOhQ-UYRliQEqeJNoO5b_Q950Dnt4yjy5BYEJZbJIu2OA&_hsmi=64754821

Angular5 tutorial
https://www.toptal.com/angular/angular-5-tutorial?utm_source=hs_email&utm_medium=email&utm_content=64754821&_hsenc=p2ANqtz--ulC07UR5v9iSLi8tmPZLo3o3pzi0hXRShrOK5KK5tU5qRxHOhQ-UYRliQEqeJNoO5b_Q950Dnt4yjy5BYEJZbJIu2OA&_hsmi=64754821

Angular5 & ASP.NET CORE
https://www.toptal.com/angular/angular-5-asp-net-core?utm_source=hs_email&utm_medium=email&utm_content=64754821&_hsenc=p2ANqtz--ulC07UR5v9iSLi8tmPZLo3o3pzi0hXRShrOK5KK5tU5qRxHOhQ-UYRliQEqeJNoO5b_Q950Dnt4yjy5BYEJZbJIu2OA&_hsmi=64754821

Integration and End-to-end Tests Made Easy with Node.js and MongoDB
https://www.toptal.com/nodejs/integration-and-e2e-tests-nodejs-mongodb?utm_campaign=blog_post_integration_and_e2e_tests_nodejs_mongodb&utm_campaign=Toptal%20Engineering%20Blog&utm_medium=email&utm_medium=email&utm_source=blog_subscribers&utm_source=hs_email&utm_content=61529325&_hsenc=p2ANqtz---KeTRS-GX0pu10jTL1JO4E1-Q-RVmSScdsheAd4B7HwORDSqIjeJzH3ym7GaSr5BQl06k6YIRcTh17EXPhj9Cku1hdg&_hsmi=61529325

Asynchronous JavaScript: From Callback Hell to Async and Await
https://www.toptal.com/javascript/asynchronous-javascript-async-await-tutorial?utm_campaign=blog_post_asynchronous_javascript_async_await_tutorial&utm_medium=email&utm_source=blog_subscribers&utm_campaign=Toptal%20Engineering%20Blog&utm_source=hs_email&utm_medium=email&utm_content=59947367&_hsenc=p2ANqtz-_8Uxtf8sL5uhy3h4N8VpqemRLsupSzbRTgz5u5zcfPfhtqwHd_kFdEh1gMFIhtc_OdDnesdCActBPij5qQGC-HzeL_zg&_hsmi=59947367

Tokens in ASP.NET CORE
https://developer.okta.com/blog/2018/03/23/token-authentication-aspnetcore-complete-guide

JWT in ASP.NET CORE & Angular
https://code-maze.com/authentication-aspnetcore-jwt-1/

Unit testing ASP.NET CORE
https://code-maze.com/unit-testing-aspnetcore-web-api/

Getting started on ASP.Net MVC here
https://docs.microsoft.com/en-us/aspnet/core/getting-started/?view=aspnetcore-2.1&tabs=macos 
 
