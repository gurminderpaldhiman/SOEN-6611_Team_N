# Maintainability Index:

## Explaination

Software maintenance involves modification of the product to fix the bugs. 
This plays an important role in a way that software does not age. 
Maintainability is defined as the difficulty of changing a software system’s source code, thus it is tied very closely to the concept of software maintenance. 
Maintainability Index was first proposed by Oman and Hagemeister and derived a formula of their own. 
This formula was modified and used in programs like Microsoft visual studio. After a lot of changes the final formula resulted:

MI = 171-5.2*ln(V) -0.23*(G) -16.2*ln (LOC)

Where the independent variables are <br />
V- Halstead Volume<br />
G- Cyclomatic complexity<br />
LOC- Source lines of code (SLOC). <br />

According to the formula if the maintainability index is greater than 45 indicates a class or a project indicates good maintainability. If it is less than 45 then it requires high maintenance. 
The individual parameters Halsted volume, cyclomatic complexity and SLOC involves changes in overall value. 
Halsted volume involves the number of operators and operands, if there is an increase in these values results in increase of Halstead volume which in turn decreases maintainability index that requires high maintenance. 
Similarly, higher the cyclomatic complexity involves higher the control predicates that results in less maintainability index.

## Calculating Maintainability Index:

### Tools Used : JHawk

We have taken five different projects and calculated the maintainability index for each class and then found the average of all the classes to get the maintainability index of individual projects and their versions. For each version we imported the project into JHawk tool and obtained the maintainability of the project.

## Results:

### Apache Commons Collections :

| Version | Maintainability Index |
|---------|-----------------------|
|   4.4   |         61.06
|   4.1   |         60.56
|   3.2   |         75.24
|   3.0   |         78.96
|   2.0   |         79.62

### Apache Commons Configurations :

| Version | Maintainability Index |
|---------|-----------------------|
|   2.6   |         75.16
|   2.4   |         73.92
|   2.2   |         72.6
|   2.0   |         68.92
|   1.8   |         70.41

### Apache Commons DbUtils :

| Version | Maintainability Index |
|---------|-----------------------|
|   1.7   |         79.03
|   1.6   |         78.79
|   1.4   |         78.43
|   1.2   |         70.57
|   1.1   |         72.63
