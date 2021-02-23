[![made-with-latex](https://img.shields.io/badge/Made%20with-LaTeX-1f425f.svg)](https://www.latex-project.org/)
# Der "Slide-Aggregator"

Ein kleines LaTeX-Paket was ich geschrieben habe um Vorlesungsfolien aufbereitet in einer PDF zu sammeln. Das Paket unterstützt Kommentare und Keyword-Zuordnungen auf Seitenbasis und legt automatisch Inhaltsverzeichnisse und Metadaten an.

Der gesamte Code findet sich in der [slide-aggregator.sty](slide-aggregator.sty).

*Hinweis: Die hier gezeigten Beispielpdfs werden auch hier erstellt und sind deswegen nur exemplarisch :)*

## Strukturen

Das Paket unterstützt flache Strukturen ([one-example.tex](examples/one-level/one-example.tex)):
[![one-example](examples/one-example.png)](examples/two-levels/two-example.tex)

Das Paket unterstützt auch hierarchische Strukturen (einer Stufe, [two-example.tex](examples/two-levels/two-example.tex)).
Dabei erlaubt es Querverweise, Kommentare und kann sich auch an PDFs unterschiedlicher Größen anpassen (`auto`-Option).
Um die Anpassung an verschiedene Größen zu zeigen, ist in diesem Beispiel die ursprüngliche PDF-Größe grau hinterlegt:
[![two-example](examples/two-example.png)](examples/two-levels/two-example.tex)