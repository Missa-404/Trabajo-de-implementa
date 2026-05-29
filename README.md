# Hangman Code

Juego del ahorcado con temática de programación desarrollado en Flutter. El objetivo es adivinar palabras y conceptos relacionados a la programacion e informatica mientras se acumulan puntos y se mantienen rachas de victorias consecutivas, volviendo el aprendizaje y estudio un juego entretenido.

---

## Características principales

- **Modo de juego normal**: Adivina palabras de programación, acumula puntos y mantén tu racha. Cada palabra correcta otorga 500 puntos y se restan 20 por cada letra fallida. La partida termina cuando falles en adividar la palabra.
- **Sistema de puntuación y racha**: Gana puntos por cada palabra acertada y mantén una racha de victorias. Solo los usuarios registrados pueden guardar sus partidas y ver un top de sus mejores puntuaciones en el apartado "Mis Records".
- **Modo estudio**: Modo de juego infinito donde puedes practicar con todas las palabras del juego sin límite de errores. No otorga puntos ni guarda registros. Requiere iniciar sesión.
- **Sistema de pistas**: Botón de pista disponible durante la partida que muestra la definición o descripción de la palabra actual.
- **Agregar palabras personalizadas**: Los usuarios registrados pueden agregar nuevas palabras con su descripción, las cuales aparecerán aleatoriamente durante las partidas. Solo los usuarios registrados tienen acceso a esta función.
- **Inicio de sesión y registro**: Sistema de autenticación para guardar progreso y acceder a funciones exclusivas.

---

## Tecnologías utilizadas

| Tecnología | Uso |
|---|---|
| **Flutter** | Framework principal para el desarrollo multiplataforma |
| **Dart** | Lenguaje de programación |
| **Provider** | Gestión de estado del juego |
| **SharedPreferences** | Almacenamiento local de sesión de usuario y datos en web |
| **SQFlite** | Base de datos SQLite para dispositivos móviles |
| **Path Provider** | Acceso al sistema de archivos del dispositivo |

---

## Estructura del proyecto
```
hangman_programming/
├── lib/
│   ├── main.dart                    # Punto de entrada de la aplicación
│   ├── models/
│   │   └── models.dart              # Modelos: User, Word, Score
│   ├── providers/
│   │   └── game_provider.dart       # Lógica del juego y estado
│   ├── services/
│   │   ├── auth_service.dart        # Autenticación de usuarios
│   │   └── database_service.dart    # Persistencia de datos (SQLite / SharedPreferences)
│   ├── screens/
│   │   ├── home_screen.dart         # Menú principal
│   │   ├── game_screen.dart         # Pantalla de juego normal
│   │   ├── study_mode_screen.dart   # Pantalla de modo estudio
│   │   ├── login_screen.dart        # Inicio de sesión
│   │   ├── register_screen.dart     # Registro de usuarios
│   │   ├── add_word_screen.dart     # Agregar nuevas palabras
│   │   └── leaderboard_screen.dart  # Tabla de records
│   └── widgets/
│       ├── gradient_background.dart  # Fondo degradado morado-rojo
│       └── hangman_figure.dart      # Dibujo del ahorcado
├── pubspec.yaml                     # Dependencias del proyecto
└── README.md                        # Este archivo

```

---

## Instalación y ejecución

### Requisitos previos
- Flutter SDK instalado ([guía oficial](https://docs.flutter.dev/get-started/install))
- Editor de código (Visual Studio Code recomendado)
- Dispositivo o emulador Android/iOS, o navegador para ejecución web

### Pasos

1. Clonar o descargar el proyecto:
   ```bash
   git clone https://github.com/Missa-404/Trabajo-de-implementa.git
   cd Trabajo-de-implementa
Instalar dependencias:
```bash
flutter pub get
# Ejecutar la aplicación:

# En un emulador o dispositivo físico
flutter run

# En navegador (modo web)
flutter run -d chrome # (o el navegador principal de tu computadora)
```
---
Desarrolladores: Astrid Alvarado Moreno y Brenda Lizeth Mendoza Hernández
