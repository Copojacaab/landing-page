# Landing Page Project - The Odin Project

This a landing page made for the course Foundations of The odin Project.

## Skill needed

- Web page structure with HTML 5
- Use of CSS for the style, the color and fonts
- Complex layout creation with flexbox
- Workflow implementation with GIT and GITHUB

## Flusso creativo del progetto

Guardando la pagina che devo replicare vedo che ha tre sezioni:

1. La testata con l'immagine
2. L'area principale con tutte le informazioni importanti del sito
3. Un pie di pagina

Rappresento queste tre sezioni tramite i tag di html5: header, main e footer

All'interno di header ho il logo(il div) e una lista di tre link cliccabili

all'interno del main ho diverse sezioni:

1. HERO: quella con la possibilitá di registrarsi e l'immagine. la divido in
    - titolo
    - testo
    - bottone
    - immagine
    ho anche pensato di dividere la sezione hero in ulteriori sezioni: una per il testo e una per l'immagine, in modo da rendere piú facile la separazione nel css
2. INFO: quella con le quattro immagini, che divido ulteriormente in:
    - h2 per il titolo
    - una lista di div per le carte, un div per raggruppare tutta la lista e successivamente un nested div per ogni carta (con la sua descrizione)
2. CIT: la sezione in cui abbiamo la citazione. Anche questa viene ulteriormente divisa:
    -la citazione vera e propria con il tag blockquote (fatto apposta)
    - il nome dell'autore con un tag p
3. CTA(Call To Action): l'ultima sezione interna al main, in cui abbiamo:
    - cta text:
        - h4
        - p
    - cta btn:
        -btn

l'ultima cosa che c'é da fare per quanto riguarda l'html é quello di fare il footer che possiamo fare con un semplice p

### CSS

La prima cosa da fare é un CSS reset, cioé riazzeriamo le informaizoni che inseriscono a volte i browser. successivamente applico il font a tutta la pagina.

ho messo il colore di sfondo e il colore del testo all'header e alla sezione hero(é lo stesso), adesso passo a disporre gli oggetti con flexbox.
aggiungendo display: flex al contenitore header lo trasformo in un contenitore flessibile.

ora spingo ai lati header logo e i link tramite justify-content (asse principale) e centro gli elementi verticalmente tramite align items


ora passiamo al prossimo punto, cioé rimuovere i pallini alla lista e mettere i link in orizzontale, credo che la soluzione sia prendere l'ul esterno e applicargli flexbox in modo da usarlo come contenitore flessibile

passo alla sezione hero, prima di tutto devo mettere orizzontalmente la sezione di testo e quella di immagine, lo faccio sempre tramite flexbox.
do uno stile ai singoli elementi all'interno di hero:
h1 main text
hero secondary text
bottone