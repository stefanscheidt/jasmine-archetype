jsts-jasmine-archetype
======================

Description
-----------

[Maven](http://maven.apache.org/) [Archetype](http://maven.apache.org/guides/introduction/introduction-to-archetypes.html) for projects using [Jasmine](http://pivotal.github.com/jasmine/).

Usage
-----

1. Clone the Repository
2. Build and install the archetype via `mvn clean install`
3. Generate a new Jasmine-project via `mvn archetype:generate` (see snippet below).
4. Adjust the maven project property `browser` in the generate `pom.xml`

Generate new project:

    mvn archetype:generate -DachetypeCatalog=local -DarchetypeGroupId=com.opitzconsulting.archetypes -DarchetypeArtifactId=jasmine-archetype -DarchetypeVersion=0.1.0-SNAPSHOT
    
In the generated project, you may

* start Jetty via `mvn jetty:run` and then open `http://localhost:8080/${project.artifactId}/SpecRunner.html`.
