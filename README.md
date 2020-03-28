> El siguiente contenido fue elaborado por [@_nhsz](https://twitter.com/_nhsz) como guía para las clases de [undefined school](https://twitter.com/undefinedSchool)
> Son bienvenidos los _issues_ y _PRs_ para mejorar el contenido, corregir errores, etc. 

> 👉 Si te resultó útil, **se agradece que lo compartas para que le llegue a más gente!**

# ![Git: Rebase vs Merge](https://i.imgur.com/OSj2s1F.png)

## Contenido

- [Merge](https://github.com/undefinedschool/notes-rebase-vs-merge#merge)
- [Rebase](https://github.com/undefinedschool/notes-rebase-vs-merge#rebase)

---

Para integrar cambios (commits) de una _branch_ a otra, podemos utilizar [merge](https://www.atlassian.com/git/tutorials/using-branches/git-merge) o [rebase](https://www.atlassian.com/git/tutorials/rewriting-history/git-rebase).

### Merge

Se suele utilizar para combinar branches públicas (por ejemplo, para mergear PRs en proyectos Open Source).

Al mergear, se genera un nuevo commit (por ejemplo, en `master`) que incluye todos los cambios (commits) que hicimos en la branch que queremos integrar (por ejemplo, `dev`), preservando el historial commits (del branch `dev`), con sus autores originales.

**Pros:**

- preserva el historial de cambios del branch.
- no destructivo.

**Cons:**

- el historial de cambios se va complejizando con el tiempo, dificultando un seguimiento y entendimiento del mismo.

[↑ Ir al inicio](https://github.com/undefinedschool/notes-rebase-vs-merge#contenido)

### Rebase

Se suele utilizar para combinar branches privadas.

Integra los cambios seteando al user que hace el rebase como nuevo autor, sobreescribiendo el historial original.

**Pros:**

- más prolijo.
- el `log` general de cambios es más fácil de entender y navegar.

**Cons:**

- no preserva el historial de cambios del branch.
- destructivo.

[↑ Ir al inicio](https://github.com/undefinedschool/notes-rebase-vs-merge#contenido)
