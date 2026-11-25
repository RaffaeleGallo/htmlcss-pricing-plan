# Pricing Plan — Boolean

Pagina responsive di lezioni di ingegneria del suono e produzione musicale con Raffaele Gallo. Esercizio HTML/CSS con contenuti e tariffe dimostrativi.

Aprire `index.html` nel browser. Non occorrono installazioni, server, JavaScript o librerie esterne.

## Layout
- Mobile, meno di 1000 px: card e feature su una colonna.
- Tablet, da 1000 a 1499 px: due card, poi la terza a tutta larghezza con feature su due colonne.
- Desktop, da 1500 px: tre card affiancate con feature su una colonna.

Il riferimento mobile mantiene le feature su una colonna: questo dettaglio degli screenshot prevale sull'espressione generica del bonus “quando una card occupa tutto lo spazio”.

Il contenitore usa `display: flex`, `flex-wrap: wrap` e `gap: 40px`. La larghezza iniziale delle card sottrae i gap prima di dividere lo spazio: `(100% - gap) / 2` oppure `(100% - 2 * gap) / 3`. `flex-grow: 1` espande la terza card sul tablet.

## Contenuti dimostrativi
Basic: 49 €/mese, 2 lezioni. Professional: 99 €/mese, 4 lezioni. Ultimate: 179 €/mese, 8 lezioni. Ogni lezione dura 60 minuti.

Il selettore mensile/annuale utilizza radio HTML e selettori CSS `:checked`. L'annuale mostra il costo mensile equivalente scontato del 15%, non il totale annuo. I totali sono riportati a fondo pagina. I pulsanti rimandano alle informazioni dimostrative, senza acquisti o prenotazioni.

Nessuna pubblicazione online o repository remoto viene creato automaticamente.
