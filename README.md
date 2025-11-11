# TestingAPI

An API automation testing framework for the restful-booker RESTful web service, built with Java and Maven.

## 📋 Overview

TestingAPI is a Maven-based Java application designed for automated API testing. This repository provides the foundational structure and build configuration necessary to develop, execute, and maintain automated API tests for the restful-booker service.

**Project Coordinates:**
- **Group ID:** `org.example`
- **Artifact ID:** `TestingAPI`
- **Version:** `1.0-SNAPSHOT`

> The `1.0-SNAPSHOT` version indicates this is an active development build.

## 🛠️ Technology Stack

| Technology | Version | Purpose |
|------------|---------|---------|
| Java | OpenJDK 25 | Runtime and compilation target |
| Maven | 4.0.0 | Build automation and dependency management |
| IntelliJ IDEA | Latest | Primary IDE for development |
| Git | Standard | Version control system |
| Character Encoding | UTF-8 | Source file and build encoding |

## 📁 Repository Structure
```
TestingAPI/
├── src/
│   └── main/
│       └── java/
│           └── org/
│               └── example/
│                   └── Main.java          # Application entry point
├── .idea/
│   ├── misc.xml                           # IntelliJ IDEA configuration
│   └── .gitignore                         # IDE-specific exclusions
├── out/                                   # IDE compilation output (ignored)
├── target/                                # Maven build output (ignored)
├── pom.xml                                # Maven project definition
├── .gitignore                             # Repository exclusion patterns
└── README.md                              # This file
```

### Directory Purpose

| Path | Purpose | Git Tracked |
|------|---------|-------------|
| `src/main/java/` | Source code root | ✓ Yes |
| `org/example/` | Package directory | ✓ Yes |
| `.idea/` | IntelliJ IDEA configuration | Partial |
| `out/` | IDE compilation output | ✗ No |
| `target/` | Maven build artifacts | ✗ No |

## 🚀 Getting Started

### Prerequisites

- **Java:** OpenJDK 25 or later
- **Maven:** 3.6+ (for dependency management)
- **IDE:** IntelliJ IDEA (recommended) or any Java IDE
- **Git:** For version control

### Installation

1. **Clone the repository:**
```bash
   git clone https://github.com/yourusername/TestingAPI.git
   cd TestingAPI
```

2. **Open in IntelliJ IDEA:**
   - Open IntelliJ IDEA
   - Select "Open" and navigate to the project directory
   - The IDE will automatically detect the Maven configuration

3. **Build the project:**
```bash
   mvn clean install
```

4. **Run the application:**
```bash
   mvn exec:java -Dexec.mainClass="org.example.Main"
```
   
   Or run directly from your IDE by executing the `Main` class.

## ⚙️ Configuration

### Maven Properties

The project uses Java 25 features and UTF-8 encoding:
```xml
<properties>
    <maven.compiler.source>25</maven.compiler.source>
    <maven.compiler.target>25</maven.compiler.target>
    <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
</properties>
```

### IDE Configuration

IntelliJ IDEA is configured to use:
- **Java SDK:** OpenJDK 25
- **Output Directory:** `out/`
- **Project Structure:** Maven standard

## 🧪 Running Tests
```bash
# Run all tests
mvn test

# Run specific test class
mvn test -Dtest=YourTestClass

# Run with coverage
mvn clean test jacoco:report
```

## 📦 Build Commands
```bash
# Clean build artifacts
mvn clean

# Compile the project
mvn compile

# Package as JAR
mvn package

# Install to local Maven repository
mvn install
```

## 🔧 Development Workflow

1. **Clone repository** → Git downloads project files
2. **Open in IDE** → IntelliJ IDEA reads `.idea/misc.xml` configuration
3. **Maven sync** → Dependencies and build configuration loaded from `pom.xml`
4. **Start development** → Write tests and code
5. **Build & test** → Maven compiles and runs tests
6. **Commit changes** → Git tracks modifications

## 📝 Version Control

The project uses a two-tier exclusion strategy:

- **Repository-level** (`.gitignore`): Excludes build artifacts, IDE workspaces, and OS files
- **IDE-level** (`.idea/.gitignore`): Excludes user-specific IDE data

### What's Tracked
- Source code (`src/`)
- Maven configuration (`pom.xml`)
- Shared IDE configuration (`.idea/misc.xml`)
- Documentation

### What's Ignored
- Build outputs (`target/`, `out/`)
- User-specific IDE settings
- OS-specific files (`.DS_Store`, `Thumbs.db`)
- Temporary files

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.


## 🙏 Acknowledgments

- restful-booker API for providing the testing endpoint
- Maven community for build automation tools
- IntelliJ IDEA for the excellent development environment

## 📞 Support

For issues, questions, or contributions, please open an issue in the GitHub repository.

---

**Note:** This project is currently in active development (`1.0-SNAPSHOT`). Features and APIs may change before the first stable release.
