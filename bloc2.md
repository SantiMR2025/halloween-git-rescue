
# Bloc 2: Les Branques del Més Enllà i Resolució del Conflicte

## Acció 3.6 — Creació de branques

Les dues branques parteixen de la versió inicial estable.
Això permet comparar dues solucions diferents sobre la
mateixa línia de codi.

```bash
git switch -c feature-nightmare
git branch
```

**Captura:** [Afegir captura de la terminal]

## Acció 3.7 — Línia temporal de la pesadilla

S'ha modificat l'estat del sistema per representar una
infecció fantasma i s'ha registrat el canvi.

```bash
git add main.js
git commit -m "feat: inject spectral nightmare protocol"
```

**Captura:** [Afegir captura del commit]

## Acció 3.8 — Línia temporal de protecció

S'ha creat una segona branca des de main i s'ha substituït
la mateixa línia per activar el protocol de protecció.

```bash
git switch main
git switch -c feature-sanctuary
git add main.js
git commit -m "feat: activate sanctuary protection protocol"
```

**Captura:** [Afegir captura del commit]

## Acció 3.9 — Integració de branques

S'ha integrat primer la branca de la pesadilla i després
s'ha intentat integrar la branca de protecció.

```bash
git switch main
git merge feature-nightmare
git merge feature-sanctuary
```

La segona integració provoca un conflicte perquè les dues
branques han modificat la mateixa línia.

**Captura:** [Afegir captura del conflicte]

## Acció 3.10 — Resolució del conflicte

S'han eliminat manualment les marques de conflicte i s'ha
conservat el protocol de protecció del servidor.

```bash
git add main.js
git commit -m "merge: resolve spectral conflict with sanctuary protocol"
git log --graph
```

**Captura:** [Afegir captura del commit de fusió]
