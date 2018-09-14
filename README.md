# cloudapplications <<TEMPLATE DOCUMENT>>

## Project background

## Technology stack

beschrijf alle technologie die je in je project gaat gebruiken. Vb. ASP.NET CORE MVC, Angular, HTML5, CSS3,..

## Architecture

Maak een schematische voorstelling van je software architectuur. Indien je gebruik maakt van ASP.NET CORE MVC kan je 
gebruik maken van de architectuur beschreven in volgende post: https://www.toptal.com/angular/angular-5-asp-net-core?utm_source=hs_email&utm_medium=email&utm_content=64754821&_hsenc=p2ANqtz--ulC07UR5v9iSLi8tmPZLo3o3pzi0hXRShrOK5KK5tU5qRxHOhQ-UYRliQEqeJNoO5b_Q950Dnt4yjy5BYEJZbJIu2OA&_hsmi=64754821

## Deployment Environment requirements

Beschrijf hier hoe je je software oplossing kan deployen

## Beschrijving requirements

Maak hier een lijst van user stories aan. Deze user stories worden gekoppeld aan mockups.
Al je user stories vormen je backlog in jira.ap.be

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
