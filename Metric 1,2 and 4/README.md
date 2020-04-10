
**Metric 1(Statement Coverage), 2(Branch Coverage) and 4(McCabe Complexity) can be calculated by using a code coverage tool like JaCoCo. Many configurations can be done inside the plugin. Below I am attaching the basic code to use JaCoCo plugin.**

### Process to measure the metrics:
**Step 1:** Check if EclEmma plugin is installed in Eclipse. If not, go to **Help-> Eclipse Marketplace-> Search for EclEmma-> Install-> Restart Eclipse.**<br />
**Step 2:** Import the maven project to Eclipse. **File-> Import -> Existing Maven projects.**<br />
**Step 3:** Add JaCoCo plugin information to pom file of the Maven porject.<br />
**Step 4:** Run the porject as Maven Clean Install and wait for the JaCoCo report to be generated. Code coverage report is generated in HTML, XML and CSV format.<br />

```html
	<plugin>
		<groupId>org.jacoco</groupId>
		<artifactId>jacoco-maven-plugin</artifactId>
		<version>0.8.2</version>
		<executions>
			<execution>
				<goals>
					<goal>prepare-agent</goal>
				</goals>
			</execution>
			<!-- attached to Maven test phase -->
			<execution>
				<id>report</id>
				<phase>test</phase>
				<goals>
					<goal>report</goal>
				</goals>
			</execution>
		</executions>
	</plugin>
```
