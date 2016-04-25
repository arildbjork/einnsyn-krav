# Oppgåveliste sprint 6
	
## ASiC-bibliotek

* Biblotek for pakking av json-ld og innsynsxml inn i ASiC-container
 	* Skal innehalde payload, orgnr avsendar, orgnr mottakar og tekststreng som definerar tyep

 * Bibliotek for reversering av overliggande

 * Applikasjon som brukar overliggande og som sender/mottar med Mock-api. API er under definisjonsarbeid

## Reception

 * Split/Dupliser dagens reception i "Avsendar"/"Mottak"-applikasjonar
 	* Avsendar:
		1. Dagens input-api
		2. Validering
		3. Konvertering
		4. Beriking (Kor "dumt" kan dette api-et gjerast? Mulighet for lett å legge til å ta bort berikingstenester)
		5. Send til/motta frå OEP

	* Mottakar:
		1. Motta frå/Send til innholdsleverandør
		2. Validering (Kanskje ?)
		3. Dump rådata
		4. Beriking
		5. Lagre til SD/ES

## Innsynskomponent
 	* Definering og lagring av innsynsbegjeringar
		* Innsynsbegjering bør inneholde:
			* Journalpostid
			* Orgnr ansvarleg organisasjon
			* Tidspunkt
			* Kontaktinfo til den som har bedt om innsyn
	
	* Skal motta Innsynsbegjering frå frontend
	* Lagre for rapportering og seinare bruk
	* Bygge opp innsynsxml
	* Sende til ansvarleg organisasjon

			
## Multi-server arkitektur
	1. Sette opp Docker overlay-network
	2. Consul
	3. Docker-Swarm

## Definere datamodell
	* Datamodel som er journalpost-sentrisk
	* Skal kunne vere dynamisk på kva som vert lagt til
		* Skal kunne lagre Noark data både med og utan arkiv-hierarki
		* Skal kunne hantere ulik type berrikingsdata
	* Bør nok representerast både gjennom SHAQL og meir "visuelt"


## Skille ut bibliotek som skal delast med OK
	* Bestille publik repo
	* Endre bygging/mvn for å handtere dette

## Støtte for versjonering/release for docker-bygging
	* I dag brukar me kun "latest" tag. Legge inn unstable/stable evt relase-taggar

## Sette opp fleire testmiljø
	* Inttest
	* Eksternt tilgjengeleg testmiljø (Avhengig av tagging av stabile bygg i docker)




To get started enter a title for your note above. When you're ready to save
your note just use Vim's :write or :update commands, a filename will be picked
automatically based on the title.

                                    * * *

The notes plug-in comes with self hosting documentation. To jump to these notes
position your cursor on the highlighted name and press `gf' in normal mode:

 * Note taking syntax
 * Note taking commands

## Test - slett denne endringen
