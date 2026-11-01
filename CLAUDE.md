# MSE1_26 – Mathematics for Software Engineering

Kursusside (engelsk) for MSE1. Bogen er `C:\GitHub\MSE_book_v2` (engelsk) og `C:\GitHub\MSE_book_v2_da` (dansk).

## Kobling til bogen

- Session NN ↔ bogens kapitel NN for sessionerne 01–11 (01 Functions … 11 Gradients and Partial Derivatives). Kapitel 0 (Basic Arithmetic) og kapitel 12–15 har ingen session.
- Sessionssiderne linker til bogens PDF via `raw.githubusercontent.com/RBrooksDK/MSE_book_v2/main/main.pdf` (og `MSE_book_v2_da`). En ændring i bogens `main.pdf` slår derfor igennem her.

## Struktur

- Sessioner `01_Functions` til `12_Conclusion_and_QA_Session`. Hver session er én `README.md` med Key Concepts, Session Preparation (bogkapitel på engelsk og dansk), Resources, Exercises (`#### Exercise N: Titel`) og Challenge Exercises.
- Figurer til opgaver og løsninger ligger i sessionens `src/`.
- Ingen Tutorial-filer eller notebooks pr. session.

## Konfiguration, der afviger fra den globale opsætning

- Ingen `mkdocs-jupyter`.
- CI (`ci.yml`) bruger GitHub Pages-actions (`upload-pages-artifact`/`deploy-pages`) i stedet for `gh-deploy`.

## Status og kilder (2026)

- Richard Brooks overtog undervisningen fra session 7. Sessionerne 01–08 er opdaterede.
- Sessionerne 09–12 indeholder gammelt materiale, indtil de er opdateret. Brug det som inspiration, ikke som kilde til notation eller indhold.
- Session notes ligger på Google Drive i mappen MSE1_26. Egne noter findes fra session 7. Materialet i MSE_9–MSE_11 er gammelt materiale fra det danske hold og trainee.
- MSE_book_v2_da er den danske udgave af bogen. Den må læses for at holde links og kapitelhenvisninger konsistente, men rettes kun, når det er aftalt.

## Struktur har forrang

Denne fil har forrang for generiske skills (fx course-session). Lav ikke tutorials eller notebooks pr. session.
