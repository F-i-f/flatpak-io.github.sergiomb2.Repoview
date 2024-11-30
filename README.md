repoview flatpak manifest
==========================

With python 2.7 dropping from various distributions, it becomes hard
to run the venerable yet still useful
[repoview](https://github.com/sergiomb2/repoview/).

This flatpak manifest bundles Python 2.7.18 (the last Python 2
release), repoview and its dependencies.  The manifest allows full
host filesystem access. Run `flatpak run io.github.sergiomb2.Repoview`
instead of running `repoview`.

The templates are installed under
`/app/share/io.github.sergiomb2.Repoview/templates/` (as seen from
inside the Flatpak container).  For example one could switch between
the four included templates with:
- `flatpak run io.github.sergiomb2.Repoview -k /app/share/io.github.sergiomb2.Repoview/templates/default`
- `flatpak run io.github.sergiomb2.Repoview -k /app/share/io.github.sergiomb2.Repoview/templates/fedora`
- `flatpak run io.github.sergiomb2.Repoview -k /app/share/io.github.sergiomb2.Repoview/templates/kaos`
- `flatpak run io.github.sergiomb2.Repoview -k /app/share/io.github.sergiomb2.Repoview/templates/kaos-international`
