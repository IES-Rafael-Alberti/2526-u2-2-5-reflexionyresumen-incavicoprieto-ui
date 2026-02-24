# RESPUESTAS — Reflexión y Resumen (Plantilla genérica)

> **Actividad / ID:** IS-2.a..e-IVP 
> **Unidad / Tema:** 2: Análisis de incidentes.  
> **Alumno/a:**  Inca Vico Prieto
> **Fecha:**  20/02/2026

---

## 1) Reflexión crítica (preguntas)

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
    3.3. Peligrosidad e impacto
        3.3.1. Grado de gravedad/peligrosidad
        3.3.2. Impacto/Alcance del incidente
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
     2.4. Servicios principales: Flujo detallado de funcionamiento(Intelligence, Monitoring, Hunting)
3. **Diseño y estructura de un SOC**
     3.1. Organización interna vs. SOC tercerizado (MSSP)
     3.2. Relación entre capacidades, servicios y procesos
     3.3. Fases de implementación: Negocio, personas, tecnologías y servicios

#### 2.2.2 ¿Qué es un SIEM?
1. **Introducción a SIEM** 
   1.1 Productos SIEM
   1.2 Analista SIEM y SOC
2. **Recopilación de registros**
  2.1 Conceptos: log y logging
  2.2 Métodos de recopilación
    2.2.1. Agentes de registro
       2.2.1.1 Ventajas del método
       2.2.1.2. Contras del método
   2.2.2 Syslog
        2.2.2.1. Formato de registro del sistema
   2.2.3. Agentes de terceros
       2.2.4.1. Agentes de cógido abierto populares
   2.2.4. Sin agente (agentless)
       2.2.4.1. Recolección manual
3. **Agregación y análisis** 
  3.1. Agregador y EPS
     3.1.1. ¿Qué es EPS?
     3.1.2. Escalado del agregador
     3.1.3. Proceso del agregador de registros
     3.1.4. Modificación de registros
     3.1.5. Enriquecimiento de registros
       3.1.5.1. Geolocalización
       3.1.5.2. DNS
4. **Almacenamiento de registros**
5. **Creación de alertas** 
  5.1. Lista negra
  5.2. Lista blanca
  5.3. Análisis de registro de cola larga
6. **Gestión de incidentes** 
  6.1. Definiciones básicas sobre la gestión de incidentes
    6.1.1. Alerta
    6.1.2. Evento
    6.1.3. Incidente
    6.1.4. Alerta de verdadero positivo
    6.1.5. Alerta de falso positivo
   6.2. Sistemas de gestión de incidentes (IMS)
     6.2.1. ¿Cómo funciona un IMS?
   6.3. Nombre del caso/alerta
   6.4. Playbooks
     6.4.1. ¿Por qué son importantes los playbooks?
   6.5. ¿Qué hace el analista SOC cuando ocurre una alerta?

#### 2.2.2 Casos de Uso en un SOC
1. **¿Qué es un caso de uso?**
2. **¿Cómo se crean los casos de uso?**
3. **10 casos de uso que todo servicio SOC moderno debería tener**
4. **Cómo gestionar los casos de uso en un SOC**
5. **Conclusiones**

#### 2.2.3 Mejores prácticas para implementar una estrategia SIEM
1. **SIEM y componentes**
2. **Estrategia para implementar un SIEM**
    2.1. Fase de descubrimiento y planificación
    2.2. Fase piloto
    2.3. Fase de implementación
    2.4. Fase de mejora continua
3. **Las mejores prácticas para la implementación de SIEM**

#### 2.2.4 Evolución de SIEM y SOAR
1. **La evolución del SIEM**
2. **Herramientas SOAR**
3. **El SIEM del futuro**
4. **La necesidad de disponer de herramientas SOAR**

#### 2.3.1 Fuentes abiertas (OSINT)
1. **Introducción a OSINT**
    1.1. Importancia y Aplicaciones de OSINT en Ciberseguridad.
       1.1.1. Principales usos de OSINT en ciberseguridad
   1.2. Diferencias entre OSINT y otras metodologías de recopilación de información
   1.3. Proceso OSINT en una vista rápida
   1.4. Actividades
2. **Uso en Ciberseguridad** 
    2.1. OSINT en Auditoría de Seguridad e Investigación Forense
    2.2. OSINT en Pentesting y Hacking Ético
    2.3. OSINT en Prevención de Atques y Detección de Amenazas (Threat Intelligence)
    2.4. Riesgos y Límites Legales de OSINT
    2.5. Actividades
3. **Proceso de OSINT** 
  3.1. Ciclo OSINT: Fases y Estructura
  3.2. Planificación y Dirección
    3.2.1. Errores comunes en esta fase
   3.3. Identicación de Fuentes de Información
   3.4. Adquisición de Información
     3.4.1. Técnicas de adquisición OSINT
   3.5. Procesamiento y Organización de Datos
    3.5.1. Errores comunes en esta fase
   3.6. Análisis e Interpretación de Datos
     3.6.1. Métodos de análisis OSINT
   3.7. Difusión y Aplicación de la Inteligencia
    3.7.1. Formatos comunes de presentación
   3.8. Actividades
4. **Técnicas de OSINT** 
  4.1.Footprinting y Fingerprinting
  4.2. Google Dorking: Búsquedas Avanzadas en Google  
      4.2.1. Recursos para Google Dorking
   4.3. Recopilación de Metadatos en Documentos
     4.3.1. Herramientas OSINT para extraer metadatos
   4.4. Búsqueda de Información en Redes Sociales
     4.4.1. Herramientas para OSINT en redes sociales.
   4.5. Identificación de Insfraestructuras con WHOIS,DNS y Direcciones IP
     4.5.1. Métodos comunes
   4.6. Monitorización de la Deep y Dark Web
     4.6.1. Herramientas para exploración en la Dark Web
   4.7. Análisis de Imágenes y Vídeos con Técnicas Forenses
     4.7.1. Técnicas forenses en imágenes
   4.8. Actividades
5. **Herramientas** 
  5.1. Motores de Búsqueda Especializados
    5.1.1. Herramientas destacadas
   5.2. Shodan: Búsqueda de Dispositivos Conectados a Internet
     5.2.1. Características principales de Shodan
     5.2.2. Recursos útiles para Shodan
   5.3. Wayback Machine: Análisis de Versiones Antiguas de Sitios Web
   5.4. Maltego: Visualización y Análisis de Relaciones
     5.4.1. Usos de Maltego en OSINT
   5.5. SpiderFoot: Automatización de la Recopilación OSINT
   5.6. OSINT Framework: Repositorio de Herramientas OSINT
   5.7. Buscadores de Información en Redes Sociales
   5.8. Técnicas de Búsqueda en Telegram, Linkedin, Twitter, Facebook
   5.9. Actividades
6. **Casos Prácticos y Actividades de OSINT**
7. **Retos Éticos y Legales de OSINT**
    7.1. Privacidad y Derechos de los Usuarios
      7.1.1. Principales preocupaciones sobre privacidad en OSINT
   7.2. Regulaciones Legales (GDPR, Código Penal, Normativa de Privacidad)
     7.2.1. Principales regulaciones sobre privacidad
   7.3. Buenas Prácticas y Uso Responsable de OSINT
     7.3.1. Principios de uso ético de OSINT
   7.4. Actividades

#### 2.4.1 Documentación e informes de incidentes
1. **Introducción**
2. **La gestión de incidentes: marco legal**
    2.1. ¿Qué es un incidente de seguridad?
    2.2. ¿Qué es la gestión de incidentes?
    2.3. El ciclo de vida de un incidentes
3. **¿Por qué es tan importantedocumentar?** 
    3.1. Generación de inteligencia de amenazas
    3.2. Lecciones aprendiedas y mejora continua
    3.3. Análisis y parametrización de sistemas de seguridad
    3.4. Campañas de sensibilización efectivas
    3.5. Cumplimiento normativo y legal
    3.6. Conocimiento del adversario
4. **¿Qué debemos documentar?** 
   4.1. Información General del Incidente
   4.2. Clasificación y Valoración
   4.3. Detalles Técnicos
   4.4.Gestión y Respuesta
   4.5. Consecuencias y Análisis Post-Incidente
5. **Seguimiento de incidentes:más allá de la resolución**
   5.1. Seguimiento durante la resolución
     5.1.1. Información de estado a mantener
     5.1.2. Comunicación continua
   5.2. Seguimiento post-resolución
     5.2.1. Verificación de la resolución
       5.2.1.1. Monitorización intensiva post-incidente
       5.2.1.2. Verificación de IOCs
       5.2.1.3. Validación con usuarios
      5.2.2. Cierre formal del incidente
   5.3. Lecciones aprendidas: el verdadero valor del incidente
     5.3.1. Estructura del análisis de lecciones aprendidas
       5.3.1.1. ¿Qué salion bien? (Reforzar fortalezas)
       5.3.1.2. ¿Qué salió mal? (Identificar debilidades)
       5.3.1.3. ¿Qué podemos mejorar? (Plan de acción)
      5.3.2. Sesión de "post-mortem" o "restrospectiva"
        5.3.2.1. Organización de la sesión
        5.3.2.2. Reglas fundamentales
        5.3.2.3. Agenda típica
      5.3.3. Actualización de documentación y sistemas
        5.3.3.1. Actualización de políticas de seguridad
        5.3.3.2. Mejora de playbooks y runbooks
        5.3.3.3. Casos de uso nuevos en el SIEM
        5.3.3.4. Material para formación y concienciación
        5.3.3.5. Actualización de planes de respuesta a incidentes
      5.3.4. Seguimiento de mejoras implementadas
6. **¿Cómo documentar un incidente? El arte de escribir informes técnicos**
    6.1. La importancia de saber comunicar
    6.2. Del contenido a la forma: enlace con la guía de redacción
7. **Bibliografía**
#### 2.4.2. Cómo escribir informes técnicos
 1. Introducción
 2. Cómo escribir informes técnicos y no morir en el intento
    2.1. Consejos estratégicos
      2.1.1. Determina los objetivos del informe
      2.1.2. Identifica a tu audiencia
      2.1.3. KISS (Keep is Simple, Stupid)
      2.1.4. Ofrece valor
   2.2. Consejos de estructura
     2.2.1. Define una estructura base
     2.2.2. Define el resto de puntos del informe creando un índice
     2.2.3. El resumen ejecutivo es tu mejor amigo
     2.2.4. Los anexos son el trastero de tu informe
     2.2.5. Haz de tu informe una plantilla
     2.2.6. Huye de los múltiples niveles anidados
     2.2.7. Convierte tu informe en un recortable
   2.3. Consejos de redacción
     2.3.1. El corrector ortográfico no cuesta dinero
     2.3.2. Cuidado con las frases largas
     2.3.3. No escatimes con los párrafos
     2.3.4. Elige usar voz pasiva o activa
     2.3.5. Usa los tipos de letra con sabiduría
     2.3.6. Usa las sangrías para que tu informe se lea mejor
     2.3.7. Usa la terminología adecuada
     2.3.8. Los gráficos cuestan, pero merecen la pena
     2.3.9. Hazte con un libro de estilo
   2.4. Consejos "espirituales"
     2.4.1. Segundas y terceras lecturas nunca fueron malas
     2.4.2. Haz que tus compañeros lean tu informe
     2.4.3. Lee en voz alta tu informe/Explícaselo a alguien
     2.4.4. Deshazte de tus coletillas
     2.4.5. Practica, practica y practica
3. Cómo escribir informes de incidentes de seguridad
   3.1. Introducción a los informes de incidentes de seguridad
   3.2. Consejos para informes de incidentes de seguridad
     3.2.1. Conoce tus tipos de informe
     3.2.1. Estructura tu informe
     3.2.3. Exactitud por encima de todo
     3.2.4. Cuenta lo que se ha hecho
     3.2.5. Distingue claramente hechos de hipótesis
     3.2.6. Dat todas tus acciones y genera una timeline de eventos
     3.2.7. Crea un listado de equipos y ususarios afectados
4. Información adicional
5. Conclusiones

### 2.2) Conceptos clave (lista breve)
Para entender bien la unidad, es fundamental manejar con soltura estos términos técnicos:
- **Taxonomía de Incidentes**: Se trata de un marco común (ej. Guía CCN-STIC 817) para que todos hablemos el mismo idioma al reportar.
- **IoC (Indicador de Compromiso)**: Son evidencias técnicas (IPs, hashes, dominios) que señalan un posible compromiso.
- **SIEM (Security Information and Event Management)**: Es el corazón del SOC; correlaciona eventos para detectar anomalías.
- **SOAR**: Es la automatización y orquestación; permite responder a incidentes a la velocidad de la red.
- **Playbooks**: Son manuales con los pasos exactos a seguir para cada tipo de alerta (ej: phishing, malware).
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
- Como conclusión, puedo decir que esta unidad ha sido una puerta a nuevas ramas de la Ciberseguridad que desconocía y han acabado siendo mi objetivo principal. También me ha ayudado a diferenciar entre los distintos tipos de SOC y CERT/CSIRT, así como a entender mejor cómo funcionan y qué servicios ofrecen. He sentido que esta unidad ha sido el nexo de unión entre mis conocicmientos en criminalística y ciberseguridad, unido a mi experiencia previa como investigadora (en la redacción de informes, análisis de pruebas, etc.), por lo que me siento muy motivada a continuar por este camino. Quizás parezca que me estoy centrando demasiado en el apartado de fuentes abiertas de esta unidad y le esté dando menos importancia a los otros (que reconozco su importancia, aunque no lo mencione tanto), pero esto es porque realmente ha sido un punto de inflexión para mi. 
