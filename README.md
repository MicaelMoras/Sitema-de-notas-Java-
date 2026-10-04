Student Grades System

A console application in Java that registers students, calculates their averages, ranks them, and shows overall class statistics.

Built as part of my Computer Science studies at UVA to practice object-oriented programming and the Java Collections Framework.

Features

- Register any number of students with two grades each
- Automatic average calculation: (grade 1 + grade 2) / 2
- Automatic status: **Aprovado** (average ≥ 6) or **Reprovado** (average < 6)
- Students listed in descending order of average
- Class statistics: overall average, highest average, and lowest average

 Concepts practiced

- **Object-oriented programming**: classes, encapsulation (private fields with getters), constructors, and toString() overriding
- **Separation of responsibilities**: Aluno represents one student, SistemaNotas manages the collection, and Main handles user input
- **Collections**: ArrayList to store the students
- **Sorting**: Collections.sort with Comparator.comparingDouble(...).reversed() and a method reference (Aluno::getMedia)
- **User input**: reading data from the console with Scanner

Project structure

| Class | Responsibility |
|---|---|
| Aluno| Stores name and grades, calculates the average, and defines the status |
| SistemaNotas | Holds the list of students, sorts them, lists them, and computes statistics |
| Main | Reads the data from the user and runs the program |

## How to run

Requires JDK 8 or higher.

bash
javac Main.java
java Main

Example:
 
Quantos alunos deseja cadastrar? 3

Aluno 1
Nome do Aluno: Ana
Nota 1: 8
Nota 2: 9

Aluno 2
Nome do Aluno: Bruno
Nota 1: 5
Nota 2: 4

Aluno 3
Nome do Aluno: Carla
Nota 1: 7
Nota 2: 6

Lista dos Alunos (Ordenada pela  Média)
Ana | Média: 8.5 | Situação: Aprovado
Carla | Média: 6.5 | Situação: Aprovado
Bruno | Média: 4.5 | Situação: Reprovado
Estatísticas gerais da Turma
Média da turma: 6.5
Maior média: 8.5
Menor média: 4.5

Author
[GitHub](https://github.com/MicaelMoras) · [LinkedIn](https://www.linkedin.com/in/micael-moras-ab70b036b/)
