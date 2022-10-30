# My Quickstart maven archetype

My custom archetype for my maven project generation, that is based on
`maven-archetype-quickstart`.

## Differences with maven quickstart archetype

- `App.java` and `AppTest.java`, were renamed to `Main.java` and `MainTest.java` respectively.
- Targets Java 17 by default
- Uses `maven-compiler-plugin` version `3.8.1`
- Uses `junit-jupiter-api` version `5.8.2`
- `exec:java` goal is configured to run the Main class
- configured to create executable `JAR` files
- has a maven `.gitignore` file
- includes my GitHub username on the `Built-By` manifest entry by default

## Installation

Clone this repo on your local machine:

```
git clone https://github.com/Lurky-phish-2085/my-quickstart-java-17.git
```

`cd` to the directory of the repo and then type:

```
mvn install
```

## Project Generation

**Disclaimer:** The following instructions provided only works as is on UNIX
machines. Please, make your own counterpart for your non-UNIX system.

To generate a new maven project based on my installed archetype, type:

```
archetypeGroupId="xyz.lurkyphish2085.maven.archetypes"
archetypeArtifactID='my-quickstart-java-17'
archetypeVersion='1.0'

mvn archetype:generate -DarchetypeGroupId="$archetypeGroupId" -DarchetypeArtifactId="$archetypeArtifactID" -DarchetypeVersion="$archetypeVersion"
```

The chunk of code above is best typed with an editor supported by your shell.
Or you can put it on a `.sh` script file and execute the script.
