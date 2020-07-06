# Content Poisson

**[Blog di Partenza]** Nuovi articoli (o guide soprattutto) sono ben accette, prima o poi questo progetto diventerà un [sottomodulo git](https://git-scm.com/book/it/v2/Git-Tools-Submodules) di `server-poisson` in `/blog`. 

Lo stile è praticamente il tema "Ghostwriter" con qualche modifica ma **non sarà** quello finale (eventuali pull request per uniformare con lo stile dell'altro sito sono ben accette (in realtà al momento non c'è ancora un'altro sito)), ad un certo punto servirà uniformare il blog con lo stile delle altre pagine.

## Development

(poiché alla fine il blog finirà su `/blog`)

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
    ```
    ```toml
    # /post/servizio-git-di-poisson.md
    series = "git"
    ```
    ```toml
    # /post/altro-articolo-git-e-poisson.md
    series = "git"
    ```

    in modo che Hugo possa raggrupparli tutti insieme in una taxonomy apposita.

- `page`

    Per pagine statiche di informazione come About e Contatti.

## Idee per Articoli e Progetti

- [TODO] Serie su come usare `git` e come usare il servizio Git come remote e la frontend (che probabilmente sarà Gitea).
- [TODO] Presetazione del forum
- [TODO] Presetazione del nuovo sito
- [TODO] Redirect della mail dell'aula 4
- [TODO] Usare ssh e scambiare file tra macchine.
