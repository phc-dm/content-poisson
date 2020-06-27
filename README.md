# Content Poisson

**[Blog di Partenza]** Nuovi articoli (o guide soprattutto) sono ben accette, prima o poi questo progetto diventerà un [sottomodulo git](https://git-scm.com/book/it/v2/Git-Tools-Submodules) di `server-poisson` in `/blog`. 

Lo stile è praticamente il tema "Ghostwriter" con qualche modifica ma **non sarà** quello finale (eventuali pull request per uniformare con lo stile dell'altro sito sono ben accette (in realtà al momento non c'è ancora un'altro sito)), ad un certo punto servirà uniformare il blog con lo stile delle altre pagine.

Tutti i contenuti inseriti in Poisson e.g. articoli, guide, ecc.

## Development

(poiché alla fine il blog finirà su `https://phc.dm.*****.**/blog`)

```
hugo server -b localhost/blog
```

## Convenzioni

Ci sono tre "tipi" di contenuti: articoli (`post`), pagine (`page`)

- `post`

    Contenuti quali progetti, guide e altro sono dei post, ciò che cambia è la "categoria" da indicare nella frontmatter. 

    - `categories = "Guide"` per le guide
    - `categories = "Progetti"` per i progetti

    Per i progetti o gli articoli che si dilungano su più di un file, aggiungere il nome di una stessa "serie" ad esempio

    ```toml
    # /post/come-usare-git.md
    series = "git"
    ...
    # /post/servizio-git-di-poisson.md
    series = "git"
    ...
    # /post/altro-articolo-git-e-poisson.md
    series = "git"
    ```

    in modo che Hugo possa raggrupparli tutti insieme in una taxonomy apposita.

- `page`

    Per pagine statiche di informazione come About e Contatti.

## Idee per Articoli e Progetti

- [ ] Serie su come usare `git` e come usare https://git.phc.dm.*****.**/ come remote e la frontend (probabilmente Gitea).
- [ ] Presetazione del forum
- [ ] Presetazione del nuovo sito
- [ ] ...