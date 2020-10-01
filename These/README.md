# Template de These
Structure minimale pour rédiger un manuscrit de thèse de doctorat aux normes typographiques françaises.

## Compilation
### (pdf)latex
Le fichier `Manuscrit.tex` est le fichier maitre, c'est donc lui qu'il faut compiler avec (pdf)latex. 

### bibtex
Une bibliographie globale est prévue pour le document, à compiler avec `bibtex`

### Makefile
Un makefile est à votre disposition pour faciliter la compilation.
`make` compile le document `make clean` nettoie le répertoire de travail (y compris le manuscrit compilé).
La variable `NAME` est a personnaliser dans le makefile.

## Rédaction chapitre par chapitre
Dans le fichier ``Main.tex``, on peut utiliser la ligne suivante pour définir la liste des chapitres à compiler (ici 1, 2 et annexes) :
````latex
\includeonly{Chapitre1,Chapitre2,Annexes}
````
