# RESPUESTAS — Reflexión y Resumen (Plantilla genérica)

> **Actividad / ID:** IS-2.a..e-IVP 
> **Unidad / Tema:** 2: Análisis de incidentes.  
> **Alumno/a:**  Inca Vico Prieto
> **Fecha:**  20/02/2026

---

## 1) Reflexión crítica (preguntas)
Responde con **lenguaje técnico** y **argumentos** (no solo opiniones). Si procede, usa ejemplos, riesgos y decisiones justificadas.

### 1.1) ¿Qué te han parecido los temas tratados en la unidad?
- Esta unidad me ha parecido más atractiva que la unidad 1. Desde la charla de Jezer Ferreira en Córdoba, me he sentido muy atraida por OSINT, así que estudiarla y practicarla en esta unidad ha sido el punto definitivo para reafirmar que quiero seguir formándome en esta dirección. He sentido que esta unidad era más práctica que la anterior. Aquí ya no nos centrábamos únicamente en la documentación, si no que debíamos realizar nosotros mismos la investigación/análisis y crear nuestros informes, una tarea que me gusta especialmente. 

### 1.2) ¿Qué ha sido más útil para tu futuro puesto de trabajo? ¿Por qué?
- Para mi, lo más útil ha sido tanto la taxonomía (que es clave para trabajar de forma ordenada con el resto del equipo) como las herramientas del SOC. El ejercicio de detección de incidentes me ha servido mucho: poder configurar algo y ver al instante cómo se recogen los ataques es fundamental. En un puesto de trabajo real, saber clasificar rápido un incidente según su peligrosidad es lo que te permite no perder el tiempo y actuar donde de verdad hace falta.

### 1.3) ¿Qué partes ya conocías y cuáles han sido nuevas para ti?
- Ya conocía las fuentes abiertas (OSINT), pero no desde este punto de vista de ciberseguridad. Lo estudié hace años en el Máster, pero era todo muy teórico y enfocado a HUMINT. Esta unidad me ha servido para profundizar y poner en práctica conocimientos que tenía un poco "en el aire". Lo que sí que ha sido totalmente nuevo para mi es la arquitectura del SOC, los diferentes niveles de analistas y cómo se usa el SOAR para automatizarlo todo.

### 1.4) ¿Qué concepto/idea te ha llamado más la atención y por qué?
- Como he dicho antes, realizar las prácticas de OSINT ha sido lo que más me ha enganchado. Me parece la combinación perfecta con mis estudios de Criminología y Criminalística: investigar el rastro digital y buscar el porqué de un ataque. También me ha hecho pensar mucho el tema de la "fatiga de alertas": cómo una herramienta avanzada puede acabar siendo inútil si el analista está saturado de avisos que no sirven para nada.

### 1.5) ¿Qué parte recortarías o simplificarías si hubiera menos tiempo? Justifica.
- En mi caso, recortaría el apartado de cómo documentar y escribir informes técnicos. Entiendo que hay que seguir un estándar, pero como ya he hecho otros estudios donde redactar informes periciales es lo normal, me parece una obviedad. Sé que quizás a otros compañeros les haga falta, pero en un Curso de Especialización creo que se podría dar por sentado y dedicar ese tiempo a cosas más técnicas, como entrar más a fondo en las reglas del SIEM.

### 1.6) ¿Qué tema has echado en falta o ampliarías? Justifica.
- Me hubiera gustado ampliar más la implementación práctica de un SIEM. Siento que es la pieza maestra de esta unidad y me ha sabido a poco. Me gustaría haber visto casos de uso más complejos desde cero: cómo pasar de una amenaza que nos imaginamos a una regla técnica que de verdad detecte el ataque sin darnos mil falsos positivos.

### 1.7) ¿Qué aplicarías “mañana” en un entorno real con recursos limitados?
- Las herramientas OSINT que hemos visto. Es increíble cómo, incluso sin presupuesto, se puede conseguir muchísima información importante usando solo herramientas gratuitas y Google Dorks. También implementaría de inmediato una taxonomía clara; tener un idioma común no cuesta dinero y es fundamental para mantener un orden.

### 1.8) ¿Qué duda, riesgo o punto crítico te queda abierto tras la unidad?
- Mi duda es cómo de efectivos seríamos de verdad ante un atacante que sepa ocultarse del SIEM (amenazas persistentes avanzadas). A veces parece que confiamos demasiado en la tecnología, y me pregunto si no deberíamos potenciar más la búsqueda manual (threat hunting). Supongo que hasta que no me vea en un caso real de verdad, no seré plenamente consciente de los límites que tenemos.


## 2) Resumen esquematizado (obligatorio)
En esta unidad hemos visto todo el proceso de cómo detectar y responder a un ataque, empezando por aprender a llamar a las cosas por su nombre con la taxonomía (para saber qué es peligroso y qué no) y siguiendo por cómo se monta un SOC de verdad. Hemos entrado a fondo en las herramientas que se usan, como el SIEM para vigilar los logs y el SOAR para que no haya que hacerlo todo a mano, sin olvidar lo importante que es el factor humano y tener unos buenos playbooks. Además, hemos visto cómo el OSINT nos ayuda a tener inteligencia usando solo fuentes abiertas para estar un paso por delante de las amenazas.

A continuación, presento un desglose más detallado de los contenidos organizados por secciones:

---

### 2.1) Mapa/índice de la unidad (visión global)
#### 2.1.1 Taxonomía de incidentes de ciberseguridad
1. **Introducción**
   1.1. Motivación
   1.2. Incidente de seguridad
2. **¿Que significa Taxonomía?**
   2.1. ¿Qué es una Taxonomía en este contexto?
   2.2. ¿Qué es la Taxonomía de Incidentes de Ciberseguridad?
   2.3. ¿Por qué es importante?
3. **Taxonomía de incidentes**
   3.1. Factores a considerar en la clasificación de incidentes
   3.2. Taxonomía de Referencia para la Clasificación de Incidentes de Seguridad
      3.2.1. Contenido abusivo
      3.2.2. Contenido dañino o malicioso
      3.2.3. Obtención de información
      3.2.4. Intento de intrusión
      3.2.5. Intrusión
      3.2.6. Disponibilidad
      3.2.7. Compromiso de la información
      3.2.8. Fraude
      3.2.9. Vulnerable
      3.2.10. Otros
   3.2. Peligrosidad e impacto
      3.2.1. Grado de gravedad/peligrosidad
      3.2.2. Impacto/Alcance del incidente
   3.3. Prioridades
   3.4. Respuesta al incidente
4. **Actividades**
   4.1. Ejemplo
   4.2. Actividad

#### 2.2.1 Ecosistema de un SOC: Servicios y herramientas
1. **Introducción**
   1.1. ¿Qué es un SOC?
   1.2. Objetivos principales de un SOC
   1.3. Diferencias entre SOC, CERT, CIRT y CSIRT
      1.3.1. Definición de términos
      1.3.2. Relación y diferencias clave
   1.4. Importancia de los SOC en la ciberseguridad empresarial
      1.4.1. Amenazas crecientes
      1.4.2. Beneficios de contar con un SOC
      1.4.3. Relevancia estratégica
2. **Componentes de un SOC**
   2.1. Personas (Roles y desarrollo)
   2.2. Procesos (Estandarización)
   2.3. Tecnologías (SIEM, SOAR, Ticketing, Forense)
   2.4. Servicios (Intelligence, Monitoring, Hunting)
3. **Diseño y estructura de un SOC**
   3.1. Organización interna vs. SOC tercerizado (MSSP)
   3.2. Relación entre capacidades, servicios y procesos
   3.3. Fases de implementación

#### 2.2.2 ¿Qué es un SIEM?
1. **Introducción a SIEM** (Productos y Roles)
2. **Recopilación de registros** (Agentes, Syslog, Agentless)
3. **Agregación y análisis** (EPS, Normalización, Enriquecimiento)
4. **Almacenamiento de registros**
5. **Creación de alertas** (Listas blancas/negras, Cola larga)
6. **Gestión de incidentes** (Definiciones, IMS, Playbooks)

#### 2.2.2 Casos de Uso en un SOC
1. ¿Qué es un caso de uso?
2. ¿Cómo se crean los casos de uso?
3. 10 casos de uso que todo servicio SOC moderno debería tener
4. Cómo gestionar los casos de uso en un SOC
5. Conclusiones

#### 2.2.3 Mejores prácticas para implementar una estrategia SIEM
1. SIEM y componentes
2. Estrategia para implementar un SIEM (Fases de planificación a mejora)
3. Mejores prácticas para la implementación

#### 2.2.4 Evolución de SIEM y SOAR
1. La evolución del SIEM
2. Herramientas SOAR
3. El SIEM del futuro
4. La necesidad de disponer de herramientas SOAR

#### 2.3.1 Fuentes abiertas (OSINT)
1. **Introducción a OSINT** (Ciclo y Aplicaciones)
2. **Uso en Ciberseguridad** (Pentesting, Forense, Prevención)
3. **Proceso de OSINT** (Planificación, Adquisición, Análisis)
4. **Técnicas** (Dorking, Metadatos, WHOIS, Redes Sociales)
5. **Herramientas** (Shodan, Maltego, SpiderFoot)
6. **Retos Éticos y Legales** (GDPR, Privacidad)

#### 2.4 Documentación e informes de incidentes
1. **Introducción y Gestión** (Ciclo de vida)
2. **¿Por qué documentar?** (Inteligencia, Lecciones aprendidas)
3. **¿Qué debemos documentar?** (Información técnica, Gestión)
4. **Seguimiento y cierre formal**
5. **Lecciones aprendidas** (Análisis post-mortem)
6. **El arte de escribir informes técnicos** (Estructura y Redacción)

### 2.2) Conceptos clave (lista breve)
Para entender bien la unidad, es fundamental manejar con soltura estos términos técnicos:
- **Taxonomía de Incidentes**: Marco común (ej. Guía CCN-STIC 817) para que todos hablemos el mismo idioma al reportar.
- **IoC (Indicador de Compromiso)**: Evidencias técnicas (IPs, hashes, dominios) que señalan un posible compromiso.
- **SIEM (Security Information and Event Management)**: El corazón del SOC; correlaciona eventos para detectar anomalías.
- **SOAR**: Automatización y orquestación; permite responder a incidentes a la velocidad de la red.
- **Playbooks**: Manuales con los pasos exactos a seguir para cada tipo de alerta (ej: phishing, malware).
- **Verdadero/Falso Positivo**: La clave de la eficiencia del analista; distinguir un ataque real de un error de configuración.

### 2.3) Procesos / procedimientos (pasos o checklist)
En cuanto a la operativa diaria, los procesos principales que hemos estudiado se pueden resumir en este flujo de trabajo:
1. **Detección**: Consiste en la recopilación continua de logs mediante protocolos como Syslog o agentes instalados en los equipos.
2. **Análisis**: Aquí se realiza la correlación de eventos y el descarte de falsos positivos apoyándonos en los playbooks establecidos.
3. **Respuesta**: Finalmente, se procede a la contención de la amenaza y la recuperación del sistema para volver a la normalidad.

### 2.4) Herramientas / técnicas (si aplica)
Respecto al software y las metodologías utilizadas para llevar a cabo estas tareas, destacaríamos las siguientes:
- **Monitoreo/SIEM**: Splunk, Sentinel, QRadar, Elastic (Kibana).
- **Red/Endpoint**: Snort/Suricata (IDS), Crowdstrike (EDR).
- **Gestión**: TheHive (Casos), MISP (IoC), ServiceNow.
- **OSINT**: Shodan, Google Dorks, Maltego, Whois.
- **Técnicas**: Análisis de cola larga (identificar lo inusual) y listas blancas/negras.

### 2.5) Buenas prácticas y errores típicos
A raíz de lo analizado, estas son algunas de las recomendaciones y fallos más comunes que debemos tener en cuenta:
- **B.P.**: **Fine-tuning constante**: Las reglas del SIEM deben ajustarse semanalmente para reducir el ruido.
- **B.P.**: **Normalización (Parsing)**: Asegurar que todos los logs hablen el mismo idioma para que la correlación funcione.
- **Error**: Recopilar "todo" sin un objetivo: Saturar el almacenamiento con logs irrelevantes que no generan valor.
- **Error**: Ignorar la fatiga del analista: Un SOC con cientos de alertas diarias termina ignorando incidentes críticos.
- **Error**: Redactar informes técnicos con juicios de valor; la documentación debe ser objetiva, basada en evidencias y sin suposiciones.

### 2.6) Glosario mínimo (términos y definiciones cortas)
Por último, para que no queden dudas sobre el lenguaje técnico empleado, incluyo este pequeño glosario:
- **C&C (Command and Control)**: Servidor del atacante para dar órdenes a equipos infectados.
- **EPS (Events Per Second)**: Unidad de medida del volumen de tráfico que maneja el SIEM.
- **WORM (Write Once, Read Many)**: Tecnología de almacenamiento para garantizar la integridad forense de los logs.
- **TTPs**: Tácticas, Técnicas y Procedimientos; el "ADN" de cómo ataca un grupo específico.


## 3) (Opcional) Evidencias y recursos usados
Para consolidar este resumen me he apoyado en los documentos técnicos de la unidad:

### Recursos y Documentación
- **Guía Nacional de Notificación y Gestión de Ciberincidentes (INCIBE/CCN)**: Clave para la sección de taxonomía y procesos de escalado.
- **Guía CCN-STIC 817**: Para entender cómo se dimensiona operativamente un SOC.
- **MaGMa Use Case Framework**: Marco para la gestión estratégica de casos de uso financieros llevados a la ciberseguridad.

### Evidencia 1
- Archivo: `evidencias/evidencia-01.pdf`
- Qué demuestra: Este informe documenta la investigación OSINT (Open Source Intelligence) realizada para rastrear y perfilar varios objetivos mediante fuentes abiertas. Incluye el uso de técnicas de dorking, análisis de metadatos, búsqueda en registros WHOIS y redes sociales.
- Qué he aprendido: He aprendido a utilizar herramientas y técnicas avanzadas de búsqueda para obtener la información requerida de forma ética y legal, comprendiendo cómo el rastro digital puede ser utilizado tanto para la defensa como para la inteligencia de amenazas.

### Evidencia 2
- Archivo: `evidencias/evidencia-02.md`
- Qué demuestra: Se trata de un resumen ejecutivo y tabla comparativa de los principales proveedores de servicios SOC y CERT/CSIRT en España (S2 Grupo, Thales, Ackcent, etc.), analizando sus capacidades, stack tecnológico y certificaciones, según las necesidades que se requerían.
- Qué he aprendido: Este análisis me ha enseñado a evaluar qué características (como el modelo co-managed, la disponibilidad 24/7 o la especialización en OT) son críticas según el perfil y los riesgos de cada empresa, permitiendo una selección de proveedores mucho más alineada con sus necesidades reales.


## 4) Conclusión (cierre)
- Al final, esta unidad me ha servido para poner los pies en la tierra y ver cómo se trabaja de verdad. Me voy con la idea de que aunque el SIEM es el músculo, el analista es el cerebro que tiene que tomar las decisiones. Me ha encantado poder unir la criminología con la parte técnica y siento que ahora tengo una visión mucho más clara de cómo se defiende una empresa, más allá de lo que digan los libros.
