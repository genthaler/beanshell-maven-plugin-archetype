#  ${pluginName}

## Example

The following configuration shows how to use the ${pluginName} in a pom:

	<project>
	  [...]
	  <build>
	    [...]
	    <plugins>
	      <plugin>
	        <groupId>${groupId}</groupId>
	        <artifactId>${artifactId}</artifactId>
	        <version>${version}</version>
			<executions>
				<execution>
					<id>${goalName}</id>
					<phase>validate</phase
					<goals>
						<goal>${goalName}</goal>
					</goals>
				</execution>
			</executions>
	        <configuration>
	          <${parameterName}>${parameterDefaultValue}</${parameterName}>
	        </configuration>
					
	      </plugin>
	      [...]
	    </plugins>
	    [...]
	  </build>
	  [...]
	</project>

Here is an example of how to use the ${pluginName} from the command line:

	mvn ${groupId}:${artifactId}:${version}:${goalName} -D${parameterExpression}=${parameterDefaultValue}
