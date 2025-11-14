# Sistema de Control de Temperatura y Humedad con Arduino

## Descripción
Sistema de control automático que regula la temperatura ambiental mediante un calefactor y un ventilador, manteniendo el entorno dentro de un rango óptimo.

## Funcionalidades

### 📊 Monitoreo en Tiempo Real
- Lectura constante de temperatura y humedad desde los sensores
- Visualización en el **Monitor Serie** de:
  - **Temperatura actual** (T)
  - **Humedad actual** (H) 
  - **Estado del sistema**

### 🎛️ Lógica de Control
El sistema gestiona automáticamente los dispositivos según los siguientes umbrales:

| Condición | Acción | Estado Visual |
|-----------|--------|---------------|
| **T > 28°C** | Activar motor DC (ventilador) | 🌀 Ventilando |
| **T < 20°C** | Encender LED Rojo (calefactor) | 🔥 Calefaccionando |
| **20°C ≤ T ≤ 28°C** | Apagar ambos sistemas + LED Verde | ✅ Óptimo |

### 💻 Estructura del Código
- **Código bien estructurado y comentado**
- **Variables configurables** para fácil modificación de umbrales
- Organización modular para mantenimiento sencillo

## Esquema de Conexiones
<img width="1536" height="598" alt="Spectacular Fyyran" src="https://github.com/user-attachments/assets/36d8b492-f980-42df-84c6-e5785790383a" />


## Configuración
1. Conectar sensores DHT11/DHT22
2. Conectar LED Rojo y Verde según especificaciones
3. Conectar motor DC con driver apropiado
4. Cargar código al Arduino
5. Abrir Monitor Serie para visualizar datos

---

*El sistema mantiene automáticamente el confort térmico dentro del rango predefinido.*
