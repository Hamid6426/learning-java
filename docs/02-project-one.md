# New Project

## Create project folder and sub-folders

```sh
mkdir -p project_one/src
mkdir -p project_one/bin
cd project_one
```

## Development Workflow

### Source Code

Create your source file in the src directory. Ensure the filename matches the public class name exactly.
The defined Class in the source code must match the name of the file. `ProjectOne.java` should have `public class ProjectOne`.

```java
// src/ProjectOne.java

public class ProjectOne {
    public static void main(String[] args) {
		System.out.println("Hamid First Java Code!");
	}
}
```

### Compilation

Use the -d (destination) flag to keep your source directory clean. This sends the .class files to the bin folder.

```sh
javac -d bin src/*.java # Compile files in the src directory
```

### Execution

```sh
java -cp bin ProjectOne 
```

Glossary:

mkdir = Creates directory as a child of current folder
-p = Creates parent directories if they don't exist (no error if they already exist)
-cp (Classpath) = Specifies where Java looks for compiled classes and libraries
-d (destination) = Specifies output directory for compiled classes and creates package structure

