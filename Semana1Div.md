### 1. Miguel: Interfaz Gráfica (UI) y Gestión del Repositorio
**Sus tareas:**
* Diseñar e implementar la interfaz principal en Godot.
* Aplicar el estilo Frutiger Aero (RNF-01): botones con efecto de cristal, fondos con degradados vibrantes y texturas de gotas de agua.
* Mantener el orden en GitHub, revisar los Pull Requests de los compañeros y hacer los merges a la rama `main` para asegurar que el proyecto no se rompa.

**Rama de Git:** `feature/ui-base`

### 2. Diony: Activos Gráficos (Assets) y Accesibilidad
Alguien debe encargarse de que el juego se vea bien y cumpla con los requisitos visuales antes de que los programadores metan el código.

**Sus tareas:**
* Diseñar o conseguir los sprites de los tres botes de basura respetando la paleta estricta (verde, gris, azul) (RNF-03).
* Crear los íconos geométricos claros para cada contenedor, garantizando la accesibilidad para personas con daltonismo (RNF-02).
* Conseguir los primeros sprites de basura básica (ej. botella PET, cáscara de plátano, papel).

**Su entregable:** Una carpeta `/assets` ordenada y subida al repositorio con todos los recursos listos para usarse en el motor.

### 3. Felipe: Programación de Físicas y Mecánica Core (Drag & Drop)
El corazón de la semana 1 es lograr que la basura se mueva y el usuario pueda interactuar con ella.

**Sus tareas:**
* Programar el script que hace que los objetos caigan por la pantalla a una velocidad constante inicial.
* Crear la mecánica de Drag & Drop (Arrastrar y Soltar). El jugador debe poder hacer clic en un residuo, mantenerlo presionado y moverlo por la pantalla.
* Configurar las colisiones (`CollisionShape2D` o `Area2D` en Godot) de la basura.

**Su rama de Git:** `feature/mecanica-drag-drop`

### 4. Rubén: Arquitectura de la Escena y Lógica de Colisiones
Mientras Felipe programa cómo se mueven los objetos, Rubén debe programar qué pasa cuando esos objetos llegan a su destino.

**Sus tareas:**
* Armar la escena principal integrando los assets de Diony.
* Programar las zonas de detección de los botes de basura.
* Escribir el script lógico inicial: si la "Botella PET" entra en el área del "Bote Azul", se destruye el objeto y se imprime un "Acierto" en la consola. Si entra en el "Bote Verde", imprime un "Error".

**Su rama de Git:** `feature/logica-contenedores`

---

### Dinámica de trabajo de la Semana 1
Diony sube las imágenes al repo. Miguel arma la pantalla de fondo y la interfaz sobre esas imágenes. En paralelo, Felipe y Rubén crean escenas de prueba aisladas para programar el *Drag & Drop* y las zonas de los botes. 

El lunes o martes 27 o 28 de abril unimos todo: metemos los scripts de Felipe y Rubén en la interfaz, compilamos el `.exe` y así tenemos lista nuestra primera entrega.
