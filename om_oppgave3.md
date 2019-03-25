[Tilbake](readme.md)
# Om oppgave 3
Her redogjør jeg for de valgene jeg har tatt underveis i oppgave 3

* For at det skal være enkelt å legge til nye destinasjoner og hotell velger jeg her også (som i oppgave 2) å bruke et objekt med destinasjoner. Hver egenskap i objektet er en destinasjon.
* Innenfor hver destinasjon legges hotell til som egne objekter som hver har to egenskaper:
    * *sommer*: for sommer pris
    * *vinter*: for vinter pris 
* Initiellt lages et tomt skjema hvor man kan velge:
  1. destinasjon
  2. hotell
  3. sesong
  4. antall enkelt og dobbelt rom
* Til alle skjema-elementene som endrer pris registreres det en lytterfunksjon som oppdaterer oppsummeringen på høyre side. Dette gjøres i *setup()* funksjonen aller først. 
* I tilegg til denne lytterfunksjonen registreres lytterfunksjoner som oppdaterer andre skjemaelementer.
   * Hotellene er avhengige av hvilken destinasjon som er valgt derfor fyldes denne menyen hver gang brukeren velger en ny destinasjon. Dette gjøres i lytterfunksjonen *oppdaterDestinasjon()*.
   * Når en bruker velger en ny sesong må prisene oppdateres. Dette gjøres i lytterfunksjonen *oppdaterSesong()*. Denne oppdaterer merkelappene til inputelementene slik at man får en visuell tilbakemelding av at sesongen er endret. 
   * Når en bruker velger et hotell kalles *oppdaterHotel()*. Denne lytterfunksjonen endrer informasjonen om hva et enkelt og dobbeltrom koster. Denne informasjonen lagres i input-elementene slik at man ikke trenger noe mer info enn input-elementene når man skal oppdatere oppsummeringen når noe endres. Både pris for vinter og sommer sesong lagres for hver input-element.

[Tilbake](readme.md)
