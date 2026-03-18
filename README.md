

🦊 EduStream: Videojuego Educativo 2D en Unity 6
EduStream es un proyecto interactivo desarrollado como herramienta de aprendizaje. Combina mecánicas de plataformas en 2D con un sistema de evaluación lógica para resolver preguntas técnicas.

🚀 Descripción del Proyecto
El jugador controla un personaje (Zorro) en un entorno de exploración. El objetivo es dirigirse hacia un punto de interés (un buzón/cartel) que funciona como portal hacia el nivel de evaluación. Una vez allí, el usuario debe responder preguntas de opción múltiple para ganar puntos y progresar.

🎮 Implementación de Eventos Principales
El núcleo del proyecto se basa en 3 eventos fundamentales que gestionan la lógica del juego:

1. Evento de Navegación (Transición de Escena)
Mecánica: Cambio de nivel al contacto físico.

Técnica: Se utiliza un Box Collider 2D en modo Is Trigger en el objeto "Buzón". Al detectar la colisión con el tag Player, se dispara el método SceneManager.LoadScene.

2. Evento de Interacción (Interfaz de Usuario)
Mecánica: Feedback visual inmediato tras la respuesta.

Técnica: Los botones de "Verdadero" y "Falso" utilizan el sistema OnClick. Al ser presionados, activan un mensaje en pantalla (UI Text) que indica el resultado de la elección.

3. Evento de Progresión (Sistema de Puntuación)
Mecánica: Actualización de datos del jugador.

Técnica: Una función lógica evalúa si la respuesta es correcta. Si se cumple la condición, se suma +10 a una variable de tipo int y se refresca el texto del contador de puntos en la interfaz.

🛠️ Detalles Técnicos
Motor: Unity 6 (6000.0.5f1).

Gráficos: Estética Pixel Art. Los sprites están configurados con Filter Mode: Point para máxima nitidez y el suelo utiliza el modo Tiled para evitar distorsiones.

Control: Script en C# compatible con el nuevo Input System y el sistema clásico (Active Input Handling: Both).

Físicas: Uso de Rigidbody 2D con rotación bloqueada en el eje Z para un movimiento estable.

📂 Cómo probar el proyecto
Descarga el repositorio.

Abre la carpeta en Unity Hub.

Asegúrate de que todas las escenas estén añadidas en File > Build Settings.

¡Dale a Play en la escena de Inicio!
