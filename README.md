# ![Git: Rebase vs Merge](https://i.imgur.com/OSj2s1F.png)

<div align="center">  
  <p align="center">
  <sub>Hola! Soy Nico (<strong>nhsz</strong>), <strong>Dev Full Stack JavaScript y mentor</strong>.</sub>
  </p>
  
  <p align="center">
    <sub>
      Hace un tiempo (principios de 2019) empecé un proyecto llamado <a href="https://undefinedschool.io"><strong>undefined school</strong></a>, una <strong>escuela de Desarrollo Web Full Stack JavaScript</strong>, 100% Open Source, con mentorías personalizadas para grupos reducidos y el foco puesto en los <strong>fundamentos</strong> y <strong>conceptos avanzados</strong>.
    </sub>
  </p>

  <p align="center">
    <sub>
      Me interesa mucho la intersección entre la educación y la tecnología, por eso también participo en proyectos como <a href="https://freecodecampba.org">freeCodeCampBA</a> (co-founder y co-organizador) y <a href="https://twitter.com/LXBA_">Learning Experience BA</a> (co-founder y co-organizador).
    </sub>
  </p>

 <p align="center">
    <sub>
  👉 Si estás arrancando en el mundo del desarrollo web y necesitás una mano, podés encontrarme en <a href="https://twitter.com/_nhsz/">Twitter</a> (también para hablar sobre cualquier tema relacionado a JavaScript o <em>#nerdeadas</em> en general 😛).
  </sub>
  </p>
  
  <p align="center">
  <sub>
    Por último, te cuento que soy muy fan del café (obvio que negro y sin azúcar), asi que si las notas te resultaron útiles y querés colaborar para que no me quede dormido y siga escribiendo guías, apuntes y más <strong>contenido Open Source en español</strong>, podés invitarme uno, gracias! ❤️
  </sub>
  </p>
  
  <p align="center">
  ☕
  <code> 
  <a href="https://cafecito.app/nhsz">
    <strong>Invitame 1 café!</strong>
  </a>
  </code>
  </p>
  <hr>
</div>

👉 Ver [todas las notas](https://github.com/undefinedschool/notes)

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
