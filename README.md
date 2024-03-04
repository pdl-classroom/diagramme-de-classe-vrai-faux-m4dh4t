# Diagramme de classe

![Classes](uml/classes.png)

## Vrai ou faux

Etant donné le diagramme de domaine ci-dessus, les assertions suivantes sont-elles vraies ou fausses ?

- Etudiant est une classe d’association
  - Faux. Etudiant est représenté comme une classe normale dans ce diagramme. Ici, Etudiant est simplement relié à Cours sans indication qu'il agit comme une classe d'association.
- Un étudiant peut participer à autant de cours qu’il veut
  - Vrai. La multiplicité "*" côté Cours signifie qu'un Etudiant peut s'inscrire à un nombre illimité de Cours.
- Plusieurs professeurs peuvent enseigner la même discipline
  - Faux. La multiplicité "1" côté Professeur indique qu'une Discipline est enseignée par exactement un Professeur.
- Un professeur peut enseigner plusieurs disciplines
  - Vrai. La multiplicité "*" côté Discipline signifie qu'un Professeur peut enseigner plusieurs Disciplines.
- Un cours peut être enseigner à 2 étudiants
  - Faux. La multiplicité "5..30" côté Etudiant indique qu'un Cours doit avoir entre 5 et 30 Etudiants.
- Un cours peut être enseigner à 20 étudiants
  - Vrai. Puisque la multiplicité est "5..30", un Cours peut avoir 20 Etudiants, qui est compris dans cette fourchette.

## Question ouverte

Représentez la même association avec la notation UML « petit losange »

- Quelles informations perd-on par rapport au diagramme ci-dessus ?
  - Le diagramme initial implique qu'un cours est une collaboration spécifique entre un professeur et une discipline. Dans une association ternaire, bien que cela reste implicite, les détails sur comment ces entités interagissent précisément au sein du cours peuvent devenir moins clairs.
