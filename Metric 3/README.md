
# Mutation Score:

## Explaination:
For measuring metric 3 we do PITest mutation using maven. Mutation score is defined as percentage of killed mutants by total number of mutants.<br />
**Mutation Score** = (killed mutants/total number of mutants)*100

**Below I am attaching the code for implementing pitest mutation in maven.**

```html
<plugin>
    <groupId>org.jacoco</groupId>
    <artifactId>jacoco-maven-plugin</artifactId>
    <version>1.5.1</version>
</plugin>
```
## Results:

**Apache Commons Collections : 43%**<br />
**Apache Commons Configurations : 80%**<br />
**Apache Commons DbUtils : 47%**<br />
