# Herramientas de Gestión Documental
## Revisión Administrativa de Cuentas Médicas – SGSSS
**Dirección de Integración Territorial · Secretaría Departamental de Salud del Cauca**

---

## Acceso a las herramientas

| Herramienta | Descripción | Enlace |
|---|---|---|
| Portal principal | Página de inicio con acceso a todas las herramientas | [Abrir portal](https://axemazon.github.io/salud-cauca-integracion-territorial/) |
| Árbol de Decisiones Interactivo | Guía paso a paso para la revisión y aprobación de cuentas médicas | [Abrir herramienta](https://axemazon.github.io/salud-cauca-integracion-territorial/Arbol_Decision_Cuentas_Medicas.html) |
| Vista Imprimible (Todas las rutas) | Mapa completo de todos los nodos y resultados para referencia e impresión | [Abrir vista](https://axemazon.github.io/salud-cauca-integracion-territorial/Capturas_Arbol_Decision_IMPRIMIR.html) |

---

## Árbol de decisiones — Flujo de revisión

El árbol cubre **9 puntos de decisión secuenciales** que abarcan el proceso completo de revisión administrativa de una cuenta médica radicada ante la Secretaría:

```
CUENTA MÉDICA RADICADA
        │
        ▼
[1] ¿Competencia departamental?
    ├── NO → Redirigir a entidad competente (EPS / ADRES / otro ente)
    └── SÍ ↓
[2] ¿Factura electrónica con CUFE válido?
    ├── NO → Devolver a IPS para corrección
    └── SÍ ↓
[3] ¿RIPS completos y coherentes con la factura?
    ├── NO → Devolver a IPS para corrección
    └── SÍ ↓
[4] ¿Prestador habilitado en REPS?
    ├── NO → Suspender — no procede pago sin habilitación
    └── SÍ ↓
[5] ¿Servicios de urgencias no asegurado?
    ├── SÍ → ¿Se agotó recobro a EPS/ADRES?
    │         ├── NO → Gestionar recobro primero (Art. 32 Ley 1438)
    │         └── SÍ ↓
    └── NO ↓
[6] ¿Tarifas según referente normativo vigente?
    ├── NO → Glosar diferencia y devolver
    └── SÍ ↓
[7] ¿Soportes clínicos y de elegibilidad completos?
    ├── NO → Devolver a IPS con glosa específica
    └── SÍ ↓
[8] ¿Prescripción / cuenta dentro del término legal?
    ├── NO → Verificar caducidad — posible rechazo
    └── SÍ ↓
[9] ¿Disponibilidad presupuestal confirmada?
    ├── NO → Registrar en lista de espera presupuestal
    └── SÍ ↓
    ✅ PROYECTAR ACTO ADMINISTRATIVO DE RECONOCIMIENTO Y PAGO
```

---

## Resultados posibles

| Resultado | Significado | Acción |
|---|---|---|
| ✅ Aprobar | Cuenta cumple todos los requisitos | Proyectar resolución de reconocimiento y pago |
| 🚫 Devolver | Faltan soportes o hay inconsistencias | Notificar a IPS con glosa detallada |
| ⚠️ Acción prioritaria | Requiere gestión urgente antes de decidir | Recobro a EPS/ADRES, verificación de sanción, etc. |
| 📤 Remitir | No es competencia de la Secretaría | Redirigir al ente correspondiente con oficio |

---

## Marco normativo aplicado

| Norma | Tema |
|---|---|
| Ley 715 de 2001, Art. 44 | Competencia departamental — población pobre no asegurada |
| Ley 1438 de 2011, Art. 32 | Atención de urgencias — obligación de atender y recobrar |
| Ley 1751 de 2015 | Derecho fundamental a la salud |
| Decreto 4747 de 2007 | Relaciones IPS-asegurador — condiciones de compra y pago |
| Resolución 3047 de 2008 | Formatos y mecanismos de remisión de información entre entidades |
| Resolución 3374 de 2000 | RIPS — estructura, campos obligatorios y validaciones |
| Resolución 1915 de 2018 | Actualización de reglas de validación RIPS |
| Decreto 358 de 2020 | Facturación electrónica en el sector salud (CUFE/DIAN) |
| Resolución 1995 de 1999 | Manejo y conservación de historias clínicas |
| Decreto 780 de 2016 | Compilación normativa única del sector salud |
| Acuerdo 256 de 2001 | Tarifas SOAT como referente para servicios no POS |
| Circular 030 de 2013 (SNS) | Control de recobros y glosas entre entidades |
| Ley 594 de 2000 | Ley General de Archivos — foliación y organización de expedientes |
| Decreto 2106 de 2019 | Simplificación de trámites en servicios del Estado |
| Ley 1474 de 2011, Art. 7 | Deber de selección objetiva y control en contratación pública |

---

## Tecnología

- **HTML5 + CSS3 + JavaScript puro** — sin dependencias externas, sin frameworks
- **Funciona sin conexión** — descarga el archivo y ábrelo directamente en el navegador
- **Diseño responsivo** — compatible con pantallas de escritorio, tablet y móvil
- **Accesible desde GitHub Pages** — sin necesidad de servidor ni instalación
- **Imprimible / exportable a PDF** — vista dedicada con todos los nodos en una sola página

---

## Estructura del repositorio

```
salud-cauca-integracion-territorial/
├── index.html                              # Portal de acceso a las herramientas
├── Arbol_Decision_Cuentas_Medicas.html     # Árbol de decisiones interactivo
├── Capturas_Arbol_Decision_IMPRIMIR.html   # Vista imprimible completa
└── README.md                               # Este archivo
```

---

## Uso local

1. Descargar este repositorio como ZIP (botón **Code → Download ZIP**)
2. Descomprimir en cualquier carpeta
3. Abrir `index.html` en el navegador (doble clic)
4. No se requiere internet ni instalación adicional

---

## Contexto

Estas herramientas apoyan la gestión de la **Dirección de Integración Territorial** de la Secretaría Departamental de Salud del Cauca en el proceso de revisión, validación y aprobación de cuentas médicas radicadas por IPS públicas y privadas para reconocimiento y pago con cargo a recursos de salud pública departamental.

El árbol de decisiones digitaliza y estandariza el proceso manual de revisión, reduciendo el riesgo de omisiones, asegurando la trazabilidad de cada expediente y sirviendo como instrumento de capacitación para el equipo técnico.
