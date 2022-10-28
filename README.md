# My Quickstart maven archetype

My custom archetype for my maven project generation, that is based on
`maven-archetype-quickstart`.

## Differences with maven quickstart archetype

- `App.java` and `AppTest.java`, were renamed to `Main.java` and `MainTest.java` respectively.
- Targets Java 17 by default
- Uses `maven-compiler-plugin` version `3.8.1`

## Installation

Clone this repo on your local machine:

```
git clone
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
archetypeGroupId="xyz.lurkyphish2085.archetypes"
archetypeArtifactID='my-quickstart-java-17'
archetypeVersion='1.0'

mvn archetype:generate -DarchetypeGroupId="$archetypeGroupId" -DarchetypeArtifactId="$archetypeArtifactID" -DarchetypeVersion="$archetypeVersion"
```

The chunk of code above is best typed with an editor supported by your shell.
Or you can put it on a `.sh` script file and execute the script.
