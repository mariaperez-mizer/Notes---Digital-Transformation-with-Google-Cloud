
---

## 1. Soberanía de Datos vs. Residencia de Datos

Cuando una empresa opera a nivel global o en sectores regulados (como gobierno, finanzas o salud), no basta con que los datos estén seguros; es obligatorio saber **dónde están físicamente** y **qué leyes los rigen**. El examen evalúa la diferencia exacta entre estos dos conceptos:

*   **Soberanía de Datos (Data Sovereignty):** Es un concepto **legal**. Establece que los datos están sujetos a las leyes y regulaciones del país donde están físicamente almacenados. 
    *   *Ejemplo:* El GDPR de la Unión Europea obliga a cualquier empresa del mundo que procese o guarde datos de ciudadanos de la UE a cumplir con sus leyes de protección de datos para garantizar que las personas mantengan el control de su información.
*   **Residencia de Datos (Data Residency):** Es un concepto **físico/geográfico**. Se refiere al lugar geográfico exacto donde se almacenan o procesan los datos. Muchos países exigen por ley que los datos personales de sus ciudadanos se queden estrictamente dentro de sus fronteras territoriales.

---

## 2. Herramientas de Control Geográfico en Google Cloud

Google ofrece múltiples mecanismos para asegurar que tus cargas de trabajo cumplan con las fronteras legales requeridas:

*   **Regiones de Google Cloud:** Cada región está compuesta por uno o más centros de datos. Al elegir una región específica (ej. Fráncfort o Bélgica dentro de la UE), Google garantiza por contrato (*Service Specific Terms*) que tus datos no saldrán de ahí.
*   **Restricciones de Políticas de Organización (Organization Policy Constraints) + IAM:** Permiten a los administradores prohibir que los desarrolladores creen recursos fuera de ciertas regiones geográficas permitidas, evitando errores humanos de almacenamiento accidental.
*   **VPC Service Controls:** Permite crear perímetros de seguridad de red para restringir el acceso a los datos basándose en la ubicación de red o filtrado por direcciones IP.
*   **Google Cloud Armor:** Restringe o bloquea el tráfico web hacia tus balanceadores de carga según la ubicación geográfica desde donde provenga la petición.

---

## 3. Recursos de Cumplimiento e Industria (Compliance)

No cumplir con las obligaciones regulatorias puede acarrear multas masivas y pérdida de reputación. Google Cloud ofrece tres herramientas clave para simplificar el proceso de auditoría y cumplimiento:

### A) Sensitive Data Protection (Protección de Datos Sensibles)
Es un servicio totalmente administrado diseñado para **descubrir, clasificar y proteger** activos de datos valiosos.
*   **¿Qué hace?** Escanea de forma automática tus bases de datos y archivos para identificar información regulada como PII (datos de identificación personal) o PHI (información de salud protegida) y permite **desidentificarla** (anonimizarla) para reducir riesgos de privacidad.

### B) Centro de Recursos de Cumplimiento (Compliance Resource Center)
Funciona como el **hub central** de Google Cloud para verificar certificaciones y la adherencia a estándares globales. 
*   **¿Qué contiene?** Mapeos detallados de controles de seguridad y documentación esencial para navegar regulaciones específicas de la industria, como **HIPAA** (Salud en EE.UU.) o **PCI DSS** (Estándar para la industria de tarjetas de pago en finanzas).

### C) Gestor de Informes de Cumplimiento (Compliance Reports Manager)
Es la plataforma para obtener **acceso bajo demanda a documentación y pruebas físicas de seguridad**.
*   **¿Qué descargas de aquí?** Certificaciones ISO/IEC (como ISO 27001), reportes **SOC** (Service Organization Control) y autoevaluaciones. Sirve para entregar evidencia dura e inmediata a tus auditores internos o externos, acelerando los procesos de certificación de tu empresa.

---

##  Enfoque de Negocio (Toma de Decisiones para el Examen)

*   **¿A qué concepto se refiere la regla legal que dice que los datos de los usuarios europeos deben regirse bajo las leyes de la UE?** ➡️ **Soberanía de Datos (Data Sovereignty)**.
*   **¿Cómo asegura un administrador que ningún empleado cree un disco de almacenamiento fuera de la Unión Europea por accidente?** ➡️ Usando **Organization Policy Constraints** junto con la selección de la **Región** correcta.
*   **¿Qué herramienta automatiza el descubrimiento de números de seguridad social o registros de salud ocultos en tus archivos para anonimizarlos?** ➡️ **Sensitive Data Protection**.
*   **Si un auditor externo te exige ver el certificado ISO 27001 de la infraestructura de Google Cloud, ¿de dónde lo descargas?** ➡️ Del **Compliance Reports Manager**.