# Resurse gratuite pentru învățătoare

Pagini statice, publicate pe GitHub Pages la <https://alexbosneanu.github.io/resurse/>,
pentru Pagina de Facebook „Planificări și Proiectări Rapide”.

Fiecare resursă e un singur fișier `index.html`, fără librării și fără cereri externe:
bifele și câmpurile stau în `localStorage`, iar tipărirea (Ctrl+P) dă PDF-ul. Lângă
fiecare pagină stă și PDF-ul generat, pentru distribuire directă în grupuri. Nu se
colectează emailuri (decizia din 7.11.2026: butonul de PDF din pagină face inutilă o poartă).

| Resursă | Pagina | PDF | Versiunea |
|---|---|---|---|
| Portofoliul de definitivat 2027 | `portofoliu-definitivat/` | `portofoliu-definitivat/portofoliu-definitivat-2027.pdf` | 1.1 · 8.11.2026 |
| Ziua inspecției de specialitate | `ziua-inspectiei/` | `ziua-inspectiei/ziua-inspectiei.pdf` | 1.1 · 8.11.2026 |
| Testul predictiv cu barem (evaluarea inițială) | `testul-predictiv/` | `testul-predictiv/testul-predictiv.pdf` | 1.1 · 8.11.2026 |

## Cum regenerezi PDF-ul (Windows, Edge instalat)

```
"C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --headless=new --disable-gpu ^
  --no-pdf-header-footer --print-to-pdf="C:\Projects\resurse\portofoliu-definitivat\portofoliu-definitivat-2027.pdf" ^
  "file:///C:/Projects/resurse/portofoliu-definitivat/index.html"
```

La orice schimbare de conținut: crește versiunea în antetul și în subsolul paginii, schimbă
cheia `localStorage` doar dacă s-au schimbat identificatorii bifelor, regenerează PDF-ul,
apoi `git commit` + `git push` (Pages publică în câteva minute).

Conținutul e al lui BOSNEANU ALEXANDRU-CONSTANTIN PFA și poate fi distribuit nemodificat,
cu sursa. Sursele oficiale sunt citate în subsolul fiecărei pagini.
