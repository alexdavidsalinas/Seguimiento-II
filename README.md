# Seguimiento-II
<h1 align="center">🏗️ Sistema de Grúa Robótica con ESP32</h1>

<p align="center">
Proyecto desarrollado en <b>Electrónica Digital II</b> que implementa una 
<b>grúa robótica de sobremesa con 2 grados de libertad (GDL)</b>, controlada mediante 
potenciómetros y gestionada por un ESP32.
</p>

<hr>

<h2>📌 Descripción General</h2>

<p>
Este sistema embebido permite controlar una grúa robótica de forma intuitiva mediante interfaces analógicas.
El usuario manipula la posición de los brazos usando potenciómetros, mientras que el sistema procesa las señales y controla servomotores en tiempo real.
</p>

<ul>
  <li>Modo automático de retorno</li>
  <li>Modo automático con secuencia predefinida</li>
  <li>Sistema de interrupciones con antirrebote</li>
</ul>

<hr>

<h2>⚙️ Arquitectura del Sistema</h2>

<h3>🔹 Entradas</h3>
<ul>
  <li>2 Potenciómetros lineales:
    <ul>
      <li>Rotación de la base</li>
      <li>Elevación del brazo</li>
    </ul>
  </li>
  <li>2 Pulsadores:
    <ul>
      <li>Retorno a posición inicial</li>
      <li>Ejecución de rutina automática</li>
    </ul>
  </li>
</ul>

<h3>🧠 Procesamiento</h3>
<ul>
  <li>Microcontrolador: <b>ESP32</b></li>
  <li>ADC:
    <ul>
      <li>Potenciómetro 1 → 12 bits</li>
      <li>Potenciómetro 2 → 10 bits</li>
    </ul>
  </li>
  <li>Conversión a PWM</li>
  <li>Gestión de interrupciones</li>
  <li>Manejo de estados</li>
</ul>

<h3>🔸 Salidas</h3>
<ul>
  <li>2 Servomotores</li>
  <li>LED verde → modo manual</li>
  <li>LED rojo → modo automático</li>
  <li>Buzzer</li>
</ul>

<hr>

<h2>🔄 Funcionamiento del Sistema</h2>

<h3>🟢 Modo Manual</h3>
<ul>
  <li>Lectura de potenciómetros</li>
  <li>Conversión ADC → PWM</li>
  <li>Control en tiempo real</li>
  <li>LED verde encendido</li>
</ul>

<p><i>Simula el control de una grúa real.</i></p>

<h3>🔴 Modo Automático: Retorno</h3>
<ul>
  <li>Se desactiva control manual</li>
  <li>Servos regresan a posición inicial</li>
  <li>LED rojo + buzzer activos</li>
  <li>Retorna a modo manual</li>
</ul>

<h3>🔁 Modo Automático: Secuencia</h3>
<ul>
  <li>Ejecuta rutina programada</li>
  <li>Señalización con LED y buzzer</li>
  <li>Retorno al estado previo</li>
</ul>

<hr>

<h2>🧩 Características Técnicas</h2>
<ul>
  <li>✔️ Control analógico con ADC</li>
  <li>✔️ PWM para servomotores</li>
  <li>✔️ Interrupciones externas</li>
  <li>✔️ Antirrebote por software</li>
  <li>✔️ Sistema basado en estados</li>
</ul>

<hr>

<h2>🛠️ Tecnologías</h2>
<ul>
  <li>MicroPython</li>
  <li>ESP32</li>
  <li>PWM</li>
  <li>ADC</li>
  <li>Programación por interrupciones</li>
</ul>

<hr>

<h2>🚀 Posibles Mejoras</h2>
<ul>
  <li>Pantalla LCD/OLED</li>
  <li>Control Bluetooth/WiFi</li>
  <li>IoT</li>
  <li>Automatización inteligente</li>
</ul>

<hr>

<h2>👨‍💻 Autores</h2>
<ul>
  <li><b>Alex Salinas Vega</b></li>
  <li><b>Isabella Suaza</b></li>
  <li><b>Juliana Areiza</b></li>
  <li><b>Melissa Sepúlveda</b></li>
</ul>
