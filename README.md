# 🔐 HackDoor OWASP Top Ten - Android Security Training Platform

An intentionally vulnerable Android application designed as a hands-on learning platform for mobile security professionals and students to practice identifying and exploiting common security flaws.

## 📱 Overview

HackDoor is a comprehensive Android security training application that covers the OWASP Mobile Top 10 vulnerabilities. It provides a safe, controlled environment for learning mobile application penetration testing techniques through practical, hands-on exercises.

## 🎯 Learning Objectives

- Understand common Android security vulnerabilities
- Practice real-world exploitation techniques
- Learn secure coding practices and remediation strategies
- Develop skills in mobile application security assessment
- Master OWASP Mobile Top 10 security risks

## 🏗️ Architecture

- **Language**: Kotlin
- **UI Framework**: Jetpack Compose
- **Target SDK**: Android API 34
- **Minimum SDK**: Android API 24
- **Build System**: Gradle with Kotlin DSL

## 🚀 Features

### 📊 Progress Tracking
- Real-time scoreboard with completion status
- 100 points per completed vulnerability
- Visual progress indicators
- Reset functionality for practice

### 📚 Educational Content
- Detailed vulnerability explanations
- Step-by-step hints and guidance
- Comprehensive remediation strategies
- Real-world attack scenarios

## 🔍 Vulnerabilities Covered

### 1. **Logging Vulnerabilities** (M1: Improper Credential Usage)
- **Scenario**: Sensitive data logging in Android logs
- **Learning**: Understanding log exposure risks
- **Practice**: Identifying and exploiting logged credentials
- **Remediation**: Secure logging practices and log filtering

### 2. **Insecure Local Storage** (M2: Inadequate Supply Chain Security)
- **Scenario 2.1**: SharedPreferences with sensitive data
- **Scenario 2.2**: SQLite database with plain text storage
- **Scenario 2.3**: Hidden file storage with passport data
- **Learning**: Secure data storage practices
- **Practice**: Extracting sensitive data from local storage
- **Remediation**: Encryption, secure storage APIs, and data protection

### 3. **Hardcoded Secrets** (M3: Insecure Authentication)
- **Scenario**: Hardcoded MPIN and API keys
- **Learning**: Dangers of hardcoded credentials
- **Practice**: Extracting secrets from APK files
- **Remediation**: Secure credential management and obfuscation

### 4. **Exported Components** (M4: Insufficient Cryptography)
- **Scenario**: Exported activities with sensitive functionality
- **Learning**: Component exposure risks
- **Practice**: Exploiting exported components
- **Remediation**: Proper component protection and intent filtering

### 5. **SQL Injection** (M5: Insecure Communication)
- **Scenario 5.1**: Authentication bypass via SQL injection
- **Scenario 5.2**: UNION-based SQL injection for data extraction
- **Learning**: Database security and input validation
- **Practice**: Crafting SQL injection payloads
- **Remediation**: Parameterized queries and input sanitization

### 6. **File Inclusion** (M6: Inadequate Privacy Controls)
- **Scenario 6.1**: Local File Inclusion (LFI)
- **Scenario 6.2**: Remote File Inclusion (RFI)
- **Learning**: File access control and path validation
- **Practice**: Exploiting file inclusion vulnerabilities
- **Remediation**: Path validation and access controls

### 7. **Deep Links** (M7: Poor Code Quality)
- **Scenario 7.1**: Parameter injection and privilege escalation
- **Scenario 7.2**: Intent redirection and external URL loading
- **Learning**: Deep link security and validation
- **Practice**: Exploiting deep link vulnerabilities
- **Remediation**: Intent validation and URL filtering

### 8. **Cross-Site Scripting (XSS)** (M8: Code Tampering)
- **Scenario 8.1**: Reflected XSS in WebView
- **Scenario 8.2**: Stored XSS with JavaScript execution
- **Learning**: WebView security and JavaScript injection
- **Practice**: Crafting XSS payloads for Android WebView
- **Remediation**: Input sanitization and WebView security

### 9. **Root Detection Bypass** (M9: Reverse Engineering)
- **Scenario**: Root detection mechanisms and bypass techniques
- **Learning**: Root detection methods and anti-tampering
- **Practice**: Using Frida to bypass root detection
- **Remediation**: Multi-layer protection and obfuscation

## 🛠️ Installation & Setup

### Prerequisites
- Android Studio Arctic Fox or later
- Android SDK API 24+
- Java Development Kit (JDK) 11 or later

### Build Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/HackDoorOWASPTopTen.git
   cd HackDoorOWASPTopTen
   ```

2. **Open in Android Studio**
   ```bash
   android-studio .
   ```

3. **Build the project**
   ```bash
   ./gradlew assembleDebug
   ```

4. **Install on device/emulator**
   ```bash
   adb install app/build/outputs/apk/debug/app-debug.apk
   ```

## 🎮 Usage Guide

### Getting Started
1. Launch the application
2. Navigate through the main menu
3. Select a vulnerability to practice
4. Follow the scenario instructions
5. Use hints when needed
6. Complete the challenge to earn points
7. Check the scoreboard for progress

### Tips for Success
- Read the vulnerability descriptions carefully
- Use the hint system when stuck
- Practice on both emulator and real devices
- Try different attack vectors
- Review remediation strategies after completion

## 🔧 Development

### Project Structure
```
app/src/main/java/com/hackdoor/trainings/
├── MainActivity.kt                 # Main application entry
├── ScoreboardActivity.kt          # Progress tracking
├── LoggingVulnerabilityActivity.kt
├── InsecureStorageActivity.kt
├── HardcodedSecretsActivity.kt
├── ExportedComponentsActivity.kt
├── SQLInjectionActivity.kt
├── FileInclusionsActivity.kt
├── DeepLinksActivity.kt
├── XSSActivity.kt
├── RootDetectionActivity.kt
└── ui/theme/                      # UI theme components
```

### Key Components
- **ProgressTracker**: Centralized progress management
- **Vulnerability Activities**: Individual training modules
- **Theme System**: Cyberpunk-themed UI components
- **Database Helper**: SQLite operations for SQL injection scenarios

## 📖 Educational Resources

### OWASP Mobile Top 10
- [OWASP Mobile Top 10 2023](https://owasp.org/www-project-mobile-top-10/2023-risks/)
- Comprehensive mobile security guidelines
- Risk assessment methodologies
- Best practices and countermeasures

### Additional Learning Materials
- Android Security Best Practices
- Mobile Application Penetration Testing
- Secure Coding Guidelines
- Reverse Engineering Techniques

## ⚠️ Disclaimer

This application is designed for **educational purposes only**. It contains intentionally vulnerable code for learning mobile security concepts. Do not use this application or its techniques on real applications without proper authorization.

## 🤝 Contributing

We welcome contributions to improve the learning experience:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

### Contribution Guidelines
- Follow Kotlin coding conventions
- Add comprehensive documentation
- Include educational value in new vulnerabilities
- Maintain the cyberpunk theme consistency

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- OWASP Mobile Security Project
- Android Security Community
- Mobile Security Researchers
- Open Source Contributors

## 📞 Support

For questions, issues, or suggestions:
- Create an issue on GitHub
- Join our community discussions
- Contact the development team

---

**Happy Learning! 🎓🔐**

*Remember: The best way to learn security is through hands-on practice in a safe, controlled environment.*
