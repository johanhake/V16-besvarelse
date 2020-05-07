[Tilbake](readme.md)
# Om oppgave 2
Her redogjør jeg for de valgene jeg har tatt underveis i oppgave 2

* Det skal være enkelt å legge til spørsmål, derfor har jeg samlet alle spørsmålene i et eget objekt med de ulike språkene som egenskapsnavn.
* For hvert språk samler jeg så spørsmålene i en liste slik at antall spørsmål blir lengden på listen.
* For hvert spørsmål inkluderer jeg fire ulike informasjoner:
  1. *sporsmal*: selve spørsmålet som skal vises i oppgaven
  2. *lyd*: om spørsmålet skal innholde en lyd? Hvis ikke skal denne være blank.
  3. *alternativ*: En liste med de ulike alternativene. Disse vill så ble vist som checkbokser for brukeren
  4. *korrekte*: en liste med indeksene som er korrekte alternativ. Her kan det være flere alternativ som er korrekt.
* Så lages automatisk en navbar hvor brukeren kan velge hvilket språk som skal brukes. Lytterfunksjonen til hver av knappene *lagSporsmal(sprak)* lager et skjema knyttet til spørsmålene for hvert språk.
* For hvert språk går jeg igjennom listen av spørsmål og genererer korrekt HTML for hvert spørsmål gjennom en for-løkke. For svar-alternativene har jeg en til for-løkke som går igjennom listen med alternativer for hvert spørsmål og lager checkbokser som brukeren kan klikke på for sin besvarelse.
* Listen med korrekte svar bruker jeg til å lagre poengene en brukere får hvis de har svart på et av alternativene (klikket på en av checkboksene). Poenget lagres som et data-attributt i hver checkboks. 
* Når så svarene skal sjekkes går jeg bare igjennom alle spørsmålene som er checked og summerer opp poengene til alle checkboksene som er krysset av. 
* Til sist gir jeg en fin tilbakemelding avhenging av hvor mange poeng brukeren har fått.


[Tilbake](readme.md)
