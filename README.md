[IDEA-356054](https://youtrack.jetbrains.com/issue/IDEA-356054)

## How to reproduce

1. Clone this repository
2. Wait until project is indexed (important)
3. Attempt to open `src/main/java/example/Test.java`

## How to reproduce from scratch

1. Create an empty Gradle project (or with any other build tool)
2. Create a new file with the following contents:
   ```java
   class Test {
     Object.Example example;
   }
   ```
3. Close the tab for the created file - if you don't close the file, when you reopen the project it 
   will hang on "Analysing..."
4. Close the window
5. Reopen the project
6. Attempt to reopen the file