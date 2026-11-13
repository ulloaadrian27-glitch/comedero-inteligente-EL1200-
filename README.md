# Comedero Inteligente para Gatos
Proyecto del curso EL-1200 Introducción a la Electrónica, TEC, II semestre 2026.
**Integrante**: Adrián Ulloa Rivera

## Descripción
Comedero automático que dispensa alimento solo cuando detecta al gato
y evita servir de más si el gato se queda frente al plato.

## Funcionamiento
- El sensor PIR detecta la presencia del gato.
- El servomotor abre la compuerta 1,5 s y la vuelve a cerrar.
- El LED indica que se está sirviendo.
- Una variable booleana (dispensado) evita que se sirva otra vez
 mientras el gato sigue ahí.

## Conexiones
| Componente | Pin del ESP32 |
|-----------------|---------------|
| Sensor PIR | GPIO 2 |
| Servomotor | GPIO 13 |
| LED (con 220 Ω) | GPIO 5 |
| Alimentación | 3V3 y GND |

![Diagrama] (https://github.com/user-attachments/assets/5d369a07-e03f-4c59-8388-d39fda58ba5a)

## Simulación
Proyecto en Wokwi: https://wokwi.com/projects/480607078968297473 

## Código
Ver la carpeta firmware/. Biblioteca usada: ESP32Servo.

## Evidencia
![Simulación](https://github.com/user-attachments/assets/84c4ef20-b6e0-4836-980f-6c8eee2fb79b)

## Mejoras futuras
Modificar el modelo para que este se active por horarios y un ajuste para indicar cuántos gramos de comida debe servir por activación.
