# Utilitarianism.net

This is a WIP repository that will replace the current _utilitarianism.net_ website. The technology we are using is [*Hugo*](https://gohugo.io/) for its flexibility, speed, ease of use, and _i18n_ (internationalization) support.

### How to start

- _clone_ the repository
- open it with your _terminal_
- run `git submodule update --init` to download the themes submodule

After this, you can always resum from here:

- run `hugo server -D` to develop

### Building

To build the production version of the application just run:

```sh
hugo -D
```

### Adding documents

All the pages were imported from Google Documents via [Docs to Markdown](https://workspace.google.com/u/0/marketplace/app/docs_to_markdown/700168918607) (see [documentation](https://github.com/evbacher/gd2md-html/wiki)).

### Internationalization

In the future we may want to use some `rtl` support
```
{{ cond (eq $.Site.Language.LanguageDirection "rtl") "pl4-l" "pr4-l" }}
```

#### Notes
We have a shortcode that will generate the table of contents: `{{< TOC >}}`
