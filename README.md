# 🛰️ Albatastic Micro
### La PCB ultra-compacta definitiva para E22/E22P y nRF52840

**Albatastic Micro** es el factor de forma más pequeño y optimizado de todo el ecosistema Albatastic. Diseñada específicamente para nodos de batería pura donde el espacio y el peso son críticos (como nodos de mochila, rastreadores portátiles o balizas ocultas), esta placa logra empaquetar una potente radio de largo alcance y un microcontrolador de bajísimo consumo en la mínima superficie de PCB posible.

A diferencia de sus hermanas mayores, la Micro prescinde de todo lo innecesario placa para enfocarse en la máxima miniaturización.

---

## 🛠️ Características Principales

*   **Miniaturización Extrema:** Huella ultra-reducida diseñada para encajar en cajas minúsculas impresas en 3D.
*   **Cerebro nRF52:** Preparada para el Pro Micro en NRF52.
*   **Conectividad de Radio Nativa:** Diseñada originalmente en torno al potente transceptor **E22/E22P** de Ebyte.
*   **Monitoreo de Energía:** Incluye un divisor de tensión con resistencias SMD para medir el estado real de la batería.
*   **Supervisión del Sistema (TLV840):** Incorpora la huella para un supervisor de voltaje de ultra-bajo consumo **TLV840**, garantizando reinicios limpios del sistema si el voltaje cae por debajo del umbral seguro.
*   **Expansión I2C:** Cuenta con pads expuestos para el bus **I2C**, permitiendo soldar rápidamente sensores ambientales (como el BME280) o pantallas OLED sin aumentar el tamaño de la placa.

---

## 📐 Vista del Diseño

A continuación se muestran los renders frontales y traseros del diseño compacto de la PCB:

<p align="center">
  <img width="450" alt="Albatastic Micro Frente" src="https://github.com/user-attachments/assets/e0857c7a-690c-4f96-a0e6-cd1726f825af" />
  <img width="450" alt="Albatastic Micro Trasera" src="https://github.com/user-attachments/assets/e0dccca3-8518-4b0b-a1d0-bf40452a2785" />
</p>

---

<details>
<summary><b>📜 Historial de Cambios / Changelog (Clic para desplegar)</b></summary>

<br>

> [!NOTE]
> **Filosofía de versiones:** La serie **V1.X** mantiene el Pro Micro en formato Through-Hole (THT) para mayor facilidad de montaje manual. La serie **V2.X** da el salto al formato SMD para exprimir aún más la reducción de espacio y expandir la compatibilidad.

#### 🚧 [V2.0] - En fase de diseño y desarrollo
*   **Cambio estructural mayor:** El Pro Micro pasa de formato THT a **SMD**, reduciendo drásticamente el grosor y el perfil total de la placa.
*   **Cambio estructural mayor:** Se pasa la PCB de 2 a 4 capas al tener tantas radios
*   **Expansión Multi-Radio:** Rompe la exclusividad del E22 y añade compatibilidad nativa para 4 radios distintas en la misma PCB: **E22/E22P**, **RA62**, **E28** y **E80**.
*   **Añadido:** Añadidos pads para GPS, I2C y serial
*   **Eliminado:** Eliminado el TLV840

#### ⚠️ [V1.1] - En fase de testeo / Fabricada
*   **Mejora de RF y Ruido:** Se añade un **plano de tierra continuo (GND plane)** para mejorar la resiliencia al ruido.

#### ✅ [V1.0] - Estable y Testeada con éxito
*   **Lanzamiento Inicial:** Diseño base ultra-compacto plenamente funcional para E22/E22P y Pro Micro THT.
*   **Características integradas:** Divisor de tensión para lectura analógica de batería, supervisor TLV840 y pads de expansión I2C operativos.

</details>

---

### 🚧 Work in Progress 🚧
Actualmente el esfuerzo de desarrollo está centrado en la **V2.0**. Esta próxima iteración convertirá la placa en una solución multi-radio compatible con hardware SMD, permitiendo crear nodos de bolsillo polivalentes con tecnologías Sub-GHz o 2.4GHz bajo el mismo factor de forma minúsculo.

---

### 📝 Licencia
Proyecto Open Source **No Comercial**.
