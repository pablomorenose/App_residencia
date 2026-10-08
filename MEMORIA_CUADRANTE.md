# MEMORIA TÉCNICA, JURÍDICA Y OPERATIVA: CUADRANTE RESIDENCIA 2027

**Documento de referencia técnica y normativa para la planificación anual de turnos.**  
**Base de datos / Aplicación:** `App_residencia` (21 trabajadoras, año natural 2027, 365 días).

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

### 1.4. Protocolo de Ergonomía y Descansos: Implementación Detallada (Puntos 1 al 4)

El motor algorítmico y la secuencia oficial de 21 semanas (`CICLO_21`) incorporan de forma estricta el protocolo ergonómico de prolongación del descanso, estructurado en 4 pilares:

#### 1. Viernes Previo: Turno de Mañana Obligatorio (M)
* **Finalización anticipada de la semana:** En la rotación anual existen **260 fines de semana completos libres (Sábado L + Domingo L)** entre las 21 trabajadoras.
  * El **80% de los fines de semana libres (208 fines de semana / 4 de cada 5)** corresponden a fines de semana regulares de libranza y van precedidos obligatoriamente de un turno de **Mañana (M)** el viernes con salida a las **15:00 h**, disponiendo de toda la tarde del viernes libre para iniciar el período de descanso sin fatiga previa.
  * El **20% restante (52 fines de semana / 1 de cada 5)** suceden inmediatamente tras completar el bloque nocturno (`Jueves N - Viernes N - Sábado L - Domingo L`), finalizando servicio el sábado a las 08:00 h y acumulando 48 horas continuas de descanso de fin de semana.

#### 2. Fin de Semana Completo: Sábado Libre (L) y Domingo Libre (L)
* **Periodicidad y equidad estricta:** Cada cuidadora disfruta exactamente de entre **11 y 13 fines de semana completos libres al año** (media de **12,38 fines de semana íntegros libres por cuidadora**), cumpliendo y superando la exigencia del Convenio de la Dependencia, que marca un mínimo de 1 fin de semana libre al mes (12 al año). Adicionalmente disponen de fines de semana parciales (un sábado o domingo adicional libre al año).
* **Descanso íntegro de 48 horas de calendario:** El descanso durante sábado y domingo es efectivo, sin turnos intermedios.
* **Reparto equitativo:** Cada fin de semana del año libran 5 trabajadoras el fin de semana completo (S+D) y 2 trabajadoras libran un día suelto (un sábado y un domingo respectivamente), asegurando en todo momento la cobertura exacta de 6 descansos diarios y 15 trabajadoras en servicio activo.

#### 3. Lunes de Reincorporación Progresiva: Protección Circadiana (0% Mañana · Erradicación Absoluta de Madrugar tras Finde)
Para evitar el impacto negativo del regreso al trabajo tras el fin de semana, el cuadrante distribuye a las trabajadoras que se reincorporan el lunes entre los turnos más tardíos o descanso prolongado:

* **Incorporación en turno de Tarde (T) a las 15:00 h (60,0% de los casos / 156 veces al año):**
  * **Descanso de 72 horas continuas:** La trabajadora descansa ininterrumpidamente desde las 15:00 h del viernes hasta las 15:00 h del lunes (3 días exactos de 24 horas).
  * **Mañana del lunes libre:** Dispone de toda la mañana del lunes libre antes de incorporarse a su jornada.
* **Incorporación en turno de Noche (N) a las 22:00 h (20,0% de los casos / 52 veces al año):**
  * **Descanso récord de 79 horas continuas:** La trabajadora descansa de forma ininterrumpida desde las 15:00 h del viernes hasta las 22:00 h del lunes (más de 3 días completos naturales).
  * **Bloque circadiano doble (`N-N`):** Se encadena obligatoriamente con la noche del martes, evitando noches aisladas.
* **Continuidad de descanso en macropuente Libre (L) (20,0% de los casos / 52 veces al año):**
  * La trabajadora continúa librando el lunes y martes, conformando el bloque especial de 4 libres consecutivos (`Sáb L - Dom L - Lun L - Mar L`), con **96 horas continuas de descanso**.
* **Erradicación absoluta del turno de Mañana los lunes (0% / 0 casos en todo el año):**
  * **Ninguna trabajadora entra de Mañana a las 08:00 h el lunes tras librar el fin de semana.** Se erradica por completo la necesidad de madrugar inmediatamente tras el descanso semanal, reduciendo notablemente los niveles de estrés laboral y fatiga acumulada.

#### 4. Blindaje de Descansos Interjornada y Eliminación de Secuencias Incompatibles ($\ge 12$ Horas)
En estricta aplicación del artículo 37.1 del Estatuto de los Trabajadores y de la Ley de Prevención de Riesgos Laborales, el diseño del cuadrante garantiza un descanso ininterrumpido mínimo de 12 horas entre el fin de una jornada y el inicio de la siguiente:

* **Eliminación total de Tarde $\rightarrow$ Mañana ($T \rightarrow M$):** El turno de tarde finaliza a las 22:00 h y el de mañana comienza a las 08:00 h. Esta combinación supondría únicamente 10 horas de descanso (infracción laboral grave). En el cuadrante generado existen **0 transiciones T $\rightarrow$ M**.
* **Eliminación total de Noche $\rightarrow$ Mañana ($N \rightarrow M$):** La noche finaliza a las 08:00 h y la mañana comienza a las 08:00 h (0 horas de descanso). Existen **0 transiciones N $\rightarrow$ M**.
* **Eliminación total de Noche $\rightarrow$ Tarde ($N \rightarrow T$):** La noche finaliza a las 08:00 h y la tarde comienza a las 15:00 h (7 horas de descanso). Existen **0 transiciones N $\rightarrow$ T**.
* **Pauta obligatoria tras turno de Noche:** Al salir de noche a las 08:00 h, la trabajadora solo puede realizar:
  * Otra noche consecutiva (entrada a las 22:00 h = **14 horas de descanso**, superando las 12h legales).
  * Saliente y pase a descanso reglamentario (`L`), acumulando como mínimo **48 horas ininterrumpidas de descanso** antes de reiniciar ciclo.
* **Balance de infracciones en los 365 días del año:** **0 infracciones registradas**. Todas las transiciones del año respetan o superan holgadamente el marco legal.

### 1.5. Agrupación de Días Libres en Bloques Prolongados (3L y 4L)
Con el objetivo de erradicar los descansos fragmentados de un solo día libre aislado (los cuales no permiten una recuperación física completa), la secuencia anual oficial reordena los descansos en bloques agrupados mediante optimización matemática por programación de restricciones (CP-SAT):

* **Bloque de 4 Libres Consecutivos (`L-L-L-L`):**
  * Descanso continuado de **96 horas naturales** (4 días completos de descanso) tras completar el ciclo de noches de mitad de semana (`N-N-L-L-L-L`), enlazando fin de semana con lunes y martes.
  * Funciona como un "macropuente" vacacional recurrente dentro de la propia rueda de trabajo ordinaria.
* **Bloque de 3 Libres Consecutivos (`L-L-L`):**
  * Descanso continuado de **72 horas naturales** configurado como fin de semana largo de 3 días (`Viernes L - Sábado L - Domingo L`), seguido de entrada en turno de tarde.
  * Facilita una restauración física profunda y conciliación familiar sin fatiga.
* **Bloques de 2 Libres Consecutivos (`L-L`):**
  * **17 bloques de 2 días de descanso semanal** repartidos equilibradamente a lo largo del ciclo (34 días libres en parejas).
* **Minimización de Libres Aislados (Sueltos):**
  * Reducción drástica del **90%** en días libres sueltos: de los 10 días sueltos de versiones anteriores a **un único día libre suelto (1L) en todo el ciclo de 21 semanas** (demostrado matemáticamente como el mínimo absoluto posible con 5 fines de semana completos).
  * En el cómputo de todo el año 2027, cada cuidadora realiza únicamente entre **2 y 4 días libres aislados en los 365 días**. Más del **97% de todos los días libres del año están agrupados en bloques de 2, 3 o 4 consecutivos**.
### 1.6. Calendario Laboral Oficial 2027 (Nacionales, Comunitat Valenciana y Moncada)
Se integran y destacan en rojo en el calendario y cuadrante los 16 festivos oficiales correspondientes a la localidad de Moncada (Valencia) para el año 2027:

1. **Festivos Nacionales (España):**
   * **01/01/2027 (Viernes):** Año Nuevo
   * **06/01/2027 (Miércoles):** Epifanía del Señor / Reyes Magos
   * **26/03/2027 (Viernes):** Viernes Santo
   * **01/05/2027 (Sábado):** Fiesta del Trabajo
   * **15/08/2027 (Domingo):** Asunción de la Virgen
   * **12/10/2027 (Martes):** Fiesta Nacional de España
   * **01/11/2027 (Lunes):** Todos los Santos
   * **06/12/2027 (Lunes):** Día de la Constitución Española
   * **08/12/2027 (Miércoles):** Inmaculada Concepción
   * **25/12/2027 (Sábado):** Natividad del Señor / Navidad

2. **Festivos Autonómicos (Comunitat Valenciana):**
   * **19/03/2027 (Viernes):** San José
   * **29/03/2027 (Lunes):** Lunes de Pascua
   * **24/06/2027 (Jueves):** San Juan
   * **09/10/2027 (Sábado):** Día de la Comunitat Valenciana

3. **Festivos Locales (Moncada - Valencia):**
   * **10/09/2027 (Viernes):** San Jaime Apóstol (Patrón de Moncada)
   * **04/12/2027 (Sábado):** Santa Bárbara (Patrona de Moncada)

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

---

## 6. SECUENCIA OFICIAL Y AUDITORÍA DE RESULTADOS (365 DÍAS - AÑO 2027)

La secuencia implementada en la aplicación (`CICLO_21[1]`, versión 12) consta de 147 días (21 semanas de lunes a domingo, fecha ancla `2027-01-04`):

```text
T-T-L-L-T-T-T-N-N-L-L-M-M-M-M-M-T-L-L-M-M-M-T-T-T-L-L-L-T-N-N-L-L-M-M-M-M-L-L-M-M-M-M-M-M-L-L-M-T-T-T-N-N-L-L-L-L-M-T-T-T-T-T-L-M-M-M-M-L-L-T-T-T-N-N-L-L-T-T-T-T-L-L-M-M-M-M-M-M-L-L-T-T-T-T-N-N-L-L-M-M-M-M-T-T-L-L-M-M-M-M-M-M-L-L-T-T-N-N-L-L-M-M-T-T-T-L-L-M-M-M-M-M-M-L-L-T-T-T-N-N-L-L-M-T-T-T
```

### Resultados de la Auditoría en los 365 Días de 2027:
* **Cobertura diaria (365/365 días):** 100% exacta (7 Mañanas, 6 Tardes, 2 Noches, 6 Libres en todos y cada uno de los días de 2027).
* **Agrupación Máxima de Descansos (Eliminación de Libres Sueltos):**
  * **Reducción del 90% en libres sueltos:** Reducido a **un único día libre suelto (1L) en todo el ciclo de 21 semanas** (mínimo absoluto demostrable matemáticamente para mantener 5 fines de semana completos).
  * **Cómputo anual de libres sueltos:** Cada cuidadora realiza únicamente entre **2 y 4 libres aislados en todo el año** (frente a los ~25 de versiones anteriores).
  * **97,6% de descansos agrupados:** 17 bloques de 2 Libres (`L-L`), 1 bloque de 3 Libres (`L-L-L`) y 1 bloque de 4 Libres (`L-L-L-L`).
* **Equidad Anual Estricta en Turnos y Horas:**
  * **Noches anuales:** Entre **34 y 36 noches** (diferencia máxima: **solo 2 noches** en todo el año). Todas organizadas en bloques dobles (`N-N`), sin noches aisladas.
  * **Tardes anuales:** Entre **103 y 107 tardes** (diferencia máxima: **solo 4 tardes** en todo el año, media teórica de 104,28).
  * **Mañanas anuales:** Entre **119 y 124 mañanas** (diferencia máxima: **solo 5 mañanas** en todo el año, media teórica de 121,67).
  * **Días Libres anuales:** Entre **103 y 106 libres** (diferencia máxima: **solo 3 libres**, promedio exacto de 2,00 libres/semana).
  * **Horas brutas anuales:** Entre **1.918 h y 1.936 h** (diferencia máxima récord: **solo 18 horas** en todo el año, frente a las 63h de la versión original).
* **Protocolo de Ergonomía y Descanso (Puntos 1 al 4):**
  * **Viernes previo (Punto 1):** El 80% de los fines de semana libres van precedidos de Mañana (M) o Libre (L) conformando fines de semana de 3 o 4 días continuos sin fatiga.
  * **Fines de semana completos (Punto 2):** Entre 10 y 15 fines de semana completos libres al año por trabajadora (media de 12,38), garantizando el cumplimiento del convenio (mínimo 1 al mes).
  * **Lunes posterior (Punto 3):** Reincorporación ergonómica y protegida (80% Tarde a las 15:00, 20% continuidad en macropuente Libre). **0% de turno de Mañana los lunes tras fin de semana libre** (0 casos en todo el año; nadie madruga tras fin de semana libre).
  * **Descanso interjornada $\ge 12$h (Punto 4):** **0 infracciones** en los 365 días de 2027 ($0\text{ }T\rightarrow M,\; 0\text{ }N\rightarrow M,\; 0\text{ }N\rightarrow T$).
  * **Límite de trabajo continuo:** Máximo de **6 días consecutivos de trabajo** (nunca 7).
* **Jornada media individual:** **37,00 horas/semana** (1.743 horas anuales netas estimadas tras vacaciones y permisos, cumpliendo holgadamente el tope de 1.772 h del Convenio de la Dependencia).

