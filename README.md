# LLama_front - AI Coffee Kiosk

An intelligent coffee ordering kiosk system with voice recognition capabilities. This Spring Boot application provides a user-friendly interface for customers to order coffee through natural language interaction.

## 🎯 Features

- **Voice-Activated Ordering**: Order coffee using natural speech
- **Interactive UI**: User-friendly kiosk interface with step-by-step ordering process
- **Menu Management**: Browse and select from various coffee options
- **Order Processing**: Real-time order confirmation and receipt generation
- **Responsive Design**: Optimized for kiosk touchscreen displays

## 🛠️ Technology Stack

- **Backend**: Spring Boot 2.7.18
- **Frontend**: JSP, HTML5, CSS3, JavaScript
- **Build Tool**: Maven
- **Java Version**: 8
- **Server**: Apache Tomcat (embedded)
- **Additional Libraries**:
  - Spring Security
  - Lombok
  - jQuery 3.6.0

## 📋 Prerequisites

Before running this application, ensure you have the following installed:

- Java JDK 8 or higher
- Maven 3.6+ (or use the included Maven wrapper)
- A web browser for accessing the kiosk interface

## 🚀 Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/AI-coffee-Kiosk/LLama_front.git
   cd LLama_front
   ```

2. **Build the project**
   ```bash
   ./mvnw clean install
   ```
   Or on Windows:
   ```bash
   mvnw.cmd clean install
   ```

3. **Run the application**
   ```bash
   ./mvnw spring-boot:run
   ```
   Or on Windows:
   ```bash
   mvnw.cmd spring-boot:run
   ```

4. **Access the application**
   
   Open your web browser and navigate to:
   ```
   http://localhost:8091
   ```

## 📁 Project Structure

```
LLama_front/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/sample/www/
│   │   │       ├── controller/      # REST controllers
│   │   │       ├── dto/             # Data Transfer Objects
│   │   │       └── BigdataApplication.java
│   │   ├── resources/
│   │   │   ├── static/              # Static resources (CSS, JS, images)
│   │   │   │   ├── css/
│   │   │   │   ├── html/
│   │   │   │   ├── img/
│   │   │   │   └── js/
│   │   │   └── application.yml      # Application configuration
│   │   └── webapp/
│   │       └── WEB-INF/
│   │           └── views/           # JSP views
│   └── test/                        # Test files
├── pom.xml                          # Maven configuration
└── README.md
```

## ⚙️ Configuration

The application can be configured via `src/main/resources/application.yml`:

- **Server Port**: Default is `8091`
- **Context Path**: `/`
- **View Configuration**: JSP files in `/WEB-INF/views/`
- **File Upload**: Max file size 50MB
- **SSL**: Configuration available (currently commented out)

## 🎨 UI Components

The kiosk interface includes:

- **Welcome Screen**: "SPEAK EASY COFFEE" introduction
- **Order Steps**: Guided ordering process (STEP 1, 2, 3...)
- **Menu Selection**: Interactive menu display
- **Order Confirmation**: Review before finalizing
- **Receipt**: Order summary and confirmation

## 🔧 Development

### Hot Reload

The application includes Spring DevTools for automatic restart during development:

```yaml
spring:
  devtools:
    livereload:
      enabled: true
```

### Building for Production

To create a deployable WAR file:

```bash
./mvnw clean package
```

The WAR file will be generated in the `target/` directory.

## 📝 License

This project is part of the Suseongu Bigdata project.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📧 Contact

For questions or support, please open an issue in the GitHub repository.

---

**SPEAK EASY COFFEE** - Making coffee ordering intelligent and effortless! ☕️