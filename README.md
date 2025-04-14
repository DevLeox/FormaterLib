# FormaterLib 📜

A lightweight **Java-based library formatter** that downloads Jar files using Gradle specifications. This utility simplifies dependency management for developers.

---

## Features ✨

- **Download Jar Files**: Retrieve Jar files based on Gradle dependency strings.
- **Pause Operations**: Delay execution with a built-in pause mechanism.
- **Resume Operations**: Activate operations after pausing.
- **Stop Operations**: Halt ongoing activities.

---

## Usage 💻

### Initialize FormaterLib:
```java
FormaterLib formatter = new FormaterLib("org.apache.commons:commons-lang3:3.12.0");
```

### Download Jar File:
```java
boolean isDownloaded = formatter.download("/path/to/save/jar");
System.out.println("Downloaded: " + isDownloaded);
```

### Pause Operations:
```java
boolean isPaused = formatter.pause();
System.out.println("Paused: " + isPaused);
```

### Resume Operations:
```java
boolean isResumed = formatter.resume();
System.out.println("Resumed: " + isResumed);
```

### Stop Operations:
```java
boolean isStopped = formatter.stop();
System.out.println("Stopped: " + isStopped);
```

---

## Code Overview 🛠️

### `FormaterLib.java`

The **`FormaterLib`** class includes:
- **Attributes**:
  - `groupId`, `artifactId`, `version`: Extracted from the Gradle specification.
  - `isRunning`: A boolean flag for operation control.
- **Core Methods**:
  - `download(String path)`: Downloads the Jar file to the specified path.
  - `pause()`: Pauses ongoing operations.
  - `resume()`: Resumes paused operations.
  - `stop()`: Stops all operations.

---

## How to Run 🚀

1. **Add the Library**:
   ```java
   // Include FormaterLib in your project.
   ```

2. **Compile and Run**:
   ```bash
   javac FormaterLib.java
   java FormaterLib
   ```

---

## Contributing 🤝

Contributions are welcome! Open an issue or submit a pull request to help improve FormaterLib.

---

## License 📜

This project is licensed under the MIT License. Feel free to use, modify, and distribute as per the license terms.
