# MEMORIA TÉCNICA, JURÍDICA Y OPERATIVA: CUADRANTE RESIDENCIA 2026

**Documento de referencia técnica y normativa para la planificación anual de turnos.**  
**Base de datos / Aplicación:** `App_residencia` (21 trabajadoras, año bisiesto/estándar 365 días).

---

## 1. REQUISITOS OPERATIVOS DEL CENTRO (ESPECIFICACIONES BASE)

A partir de los requerimientos y condiciones de funcionamiento fijados para la residencia, el sistema se estructura bajo los siguientes parámetros inalterables:

### 1.1. Dimensión y Denominación de la Plantilla
* **Plantilla total:** **21 trabajadoras** (personal de atención directa / cuidadoras).
* **Identificación neutral:** Códigos correlativos del **`01` al `21`** (sin nombres precargados en el motor algorítmico).
* **Edición y firma manuscrita:**
  * En la interfaz web: campo editable por trabajadora que se autoguarda localmente.
  * En el formato impreso / PDF: espacio reservado con línea para firma o rotulación manual del nombre (`01 _____________________`).

### 1.2. Cobertura Diaria Obligatoria (Presencia 24/7 los 365 días)
Todos los días del año (sin distinción de festivos, fines de semana o laborables) deben estar cubiertos con exactitud matemática:
* **Mañana (M):** **7 trabajadoras**
* **Tarde (T):** **6 trabajadoras**
* **Noche (N):** **2 trabajadoras**
* **Total en servicio diario:** **15 trabajadoras** en activo por día.
* **Descanso diario:** Exactamente **6 trabajadoras librando (L)** cada día ($21 - 15 = 6$).

### 1.3. Criterio de Equidad Estricta en Descansos
* **Días libres regulares:** Cada trabajadora disfruta exactamente de **2,00 días libres a la semana** (42 días libres semanales repartidos exactamente entre las 21 personas).
* Ninguna trabajadora puede finalizar el año con más o menos días libres reglamentarios que otra dentro del ciclo anual de trabajo (104 días de descanso semanal al año, más vacaciones y permisos).

### 1.4. Ergonomía del Descanso de Fin de Semana (Viernes M $\rightarrow$ Lunes N)
* En el fin de semana de libranza mensual (Sábado L + Domingo L), la rotación prioriza:
  * **Viernes previo:** Turno de **Mañana (M)** (salida a las 15:00 h).
  * **Fin de semana:** Sábado Libre (L) y Domingo Libre (L).
  * **Lunes de incorporación:** Entrada en turno de **Noche (N)** (entrada a las 22:00 h).
* **Resultado ergonómico:** Se genera un bloque ininterrumpido de **79 horas consecutivas de descanso** (desde el viernes a las 15:00 h hasta el lunes a las 22:00 h). Dado que los lunes solo existen 2 puestos de Noche, las trabajadoras que no entran de noche se incorporan de Tarde (72h de descanso continuo) o Mañana (65h de descanso continuo), superando siempre con creces el mínimo legal.

---

## 2. MARCO NORMATIVO Y LABORAL APLICABLE

El diseño y justificación del cuadrante se rige por la legislación laboral española y el marco sectorial de la dependencia:

1. **Estatuto de los Trabajadores (Real Decreto Legislativo 2/2015):**
   * **Art. 34 (Jornada):** Cómputo anual y distribución regular o irregular de la jornada.
   * **Art. 36 (Trabajo nocturno y trabajo a turnos):** Regulación del horario nocturno (22:00 h a 06:00 h), límites de jornada media y protección de la salud.
   * **Art. 37 (Descansos):** Mínimo de 12 horas entre jornadas y descanso semanal ininterrumpido de día y medio (o acumulable en períodos de hasta 14 días).

2. **Real Decreto 1561/1995 (Jornadas Especiales de Trabajo):**
   * **Arts. 32 y 33 (Trabajo nocturno y trabajos que exigen continuidad de servicio):** Autoriza la flexibilización y distribución de turnos de hasta 10 o 12 horas en centros sanitarios, asistenciales y residencias de mayores para garantizar la continuidad ininterrumpida de los cuidados 24 horas.

3. **Convenio Colectivo Marco Estatal de Servicios de Atención a las Personas Dependientes:**
   * **Jornada máxima ordinaria:** **1.772 horas anuales** de trabajo efectivo.
   * **Vacaciones anuales retribuidas:** **30 días naturales** al año.
   * **Días de libre disposición / Asuntos propios:** **4 días anuales**.
   * **Límites de turnos:** Prohibición de realizar más de 6 días consecutivos de trabajo; descanso mínimo de 12 horas entre fin y comienzo de turno; rotación con al menos 1 fin de semana completo libre al mes.

---

## 3. JUSTIFICACIÓN JURÍDICA DEL TURNO NOCTURNO DE 10 HORAS

A menudo surge la duda sobre si un turno de noche puede legalmente durar 10 horas. **La respuesta jurídica es rotundamente afirmativa.**

### 3.1. Interpretación Literal del Art. 36.1 del Estatuto de los Trabajadores
El artículo 36.1 establece:
> *«La jornada de trabajo de los trabajadores nocturnos no podrá exceder de ocho horas diarias **de promedio**, en un período de referencia de quince días.»*

* **La norma fija un PROMEDIO, no un tope diario rígido:** La legislación española y comunitaria (Directiva 2003/88/CE) permite turnos individuales de 10 horas siempre que el cómputo en la quincena o período de referencia no supere una media de 8 horas diarias de noche.
* **Cálculo en nuestro cuadrante:** 
  * En una quincena, una trabajadora de la residencia realiza como máximo 2 noches de 10 horas ($2 \times 10 = 20\text{ horas de noche en 15 días}$).
  * Promedio de noche en 15 días: $\frac{20\text{ h}}{15\text{ días}} = \mathbf{1,33\text{ horas/día}}$.
  * **Conclusión:** Queda a una distancia enorme del límite legal máximo de 8 h/día.

### 3.2. Descanso Ininterrumpido Entre Jornadas ($\ge 12$ Horas)
* **Entre dos turnos de noche consecutivos:**
  * Salida a las 08:00 h $\rightarrow$ Entrada a las 22:00 h del mismo día = **14 horas de descanso** (cumple $\ge 12$ h).
* **Al finalizar el ciclo de noche hacia día Libre:**
  * Salida a las 08:00 h del lunes $\rightarrow$ Día libre el martes $\rightarrow$ Entrada el miércoles de Mañana a las 08:00 h = **48 horas ininterrumpidas de descanso**.

### 3.3. Prohibición de Horas Extraordinarias
El art. 36.1 del ET prohíbe realizar horas extras a los trabajadores nocturnos. Dado que la jornada anual neta resultante del cuadrante (1.743 h) está por debajo de las 1.772 h del convenio, **no se generan horas extraordinarias estructurales**.

### 3.4. Deberes Empresariales Derivados
* **Plus de nocturnidad:** Retribución económica o descanso compensatorio específico por las horas trabajadas en la franja nocturna (según tablas del convenio).
* **Evaluación de salud específica:** Reconocimiento médico voluntario previo y periódico anual conforme a los protocolos de salud laboral para trabajadores nocturnos.

---

## 4. ESTUDIO COMPARATIVO: OPCIÓN 7 / 7 / 10 vs. OPCIÓN 7,5 / 7,5 / 9

Para cubrir la dotación exigida (7M + 6T + 2N), se analizan las dos configuraciones horarias:

| Parámetro | Configuración A: **7h M / 7h T / 10h N** *(Óptima)* | Configuración B: **7,5h M / 7,5h T / 9h N** *(Inviable sin refuerzo)* |
| :--- | :---: | :---: |
| **Horas diarias centro** | $7(7) + 6(7) + 2(10) = \mathbf{111\text{ h/día}}$ | $7(7,5) + 6(7,5) + 2(9) = \mathbf{115,5\text{ h/día}}$ |
| **Horas semanales centro** | $111 \times 7 = \mathbf{777\text{ h/semana}}$ | $115,5 \times 7 = \mathbf{808,5\text{ h/semana}}$ |
| **Media semanal por persona (21 trab.)** | $\frac{777}{21} = \mathbf{37,00\text{ h/semana}}$ | $\frac{808,5}{21} = \mathbf{38,50\text{ h/semana}}$ |
| **Horas brutas anuales centro (365 días)** | $365 \times 111 = \mathbf{40.515\text{ h/año}}$ | $365 \times 115,5 = \mathbf{42.157,5\text{ h/año}}$ |
| **Horas brutas por trabajadora** | $\frac{40.515}{21} = \mathbf{1.929,3\text{ h/año}}$ | $\frac{42.157,5}{21} = \mathbf{2.007,5\text{ h/año}}$ |
| **Deducción vacaciones (30 días nat.)** | $\approx -157\text{ h}$ (21,4 días lab. $\times$ 7,33h media) | $\approx -164\text{ h}$ (21,4 días lab. $\times$ 7,65h media) |
| **Deducción Asuntos Propios (4 días)** | $\approx -29\text{ h}$ (4 días $\times$ 7,33h) | $\approx -30,5\text{ h}$ (4 días $\times$ 7,65h) |
| **Jornada neta anual trabajada** | $\mathbf{1.743\text{ horas/año}}$ | $\mathbf{1.813\text{ horas/año}}$ |
| **Tope máximo Convenio Dependencia** | **1.772 horas/año** | **1.772 horas/año** |
| **Balance legal frente a convenio** | **$-29\text{ horas}$ (Margen legal seguro)** | **$+41\text{ horas}$ (EXCESO ILEGAL DE JORNADA)** |
| **Autosuficiencia de la plantilla (21)** | **100% autosuficiente (0 correturnos)** | **Imposible sin personal extra (exige 23,8 personas)** |

---

## 5. CONCLUSIÓN Y DICTAMEN TÉCNICO

1. **La opción de turnos 7h Mañana / 7h Tarde / 10h Noche es la única combinación matemáticamente autosuficiente y 100% legal** para una plantilla fija de 21 personas que deba cubrir 7M, 6T y 2N todos los días del año.
2. Produce una jornada media de **37 horas semanales** y una jornada neta de **1.743 horas anuales**, encajando de forma impecable dentro del límite de 1.772 horas del Convenio de la Dependencia.
3. Garantiza un reparto equitativo de **2,00 días libres a la semana** para todas las trabajadoras y cubre las 24 horas del reloj de forma natural (08:00–15:00, 15:00–22:00, 22:00–08:00) sin solapes artificiosos ni descubiertos.
4. Si la dirección decidiera implantar turnos de 7,5h / 7,5h / 9h, estaría legalmente obligada a:
   * Ampliar la plantilla a **24 trabajadoras**, o bien
   * Conceder entre **5 y 6 días libres adicionales de ajuste de convenio ("L+")** por trabajadora y contratar personal correturnos para cubrir los huecos resultantes.
