# Method Enterprise Builder Planning

> **Metodología universal de 8 fases para planificar y construir software enterprise-grade, de misión crítica y alta disponibilidad. Compatible con los principales agentes de IA para desarrollo.**

[![Licencia: MIT](https://img.shields.io/badge/Licencia-MIT-blue.svg)](LICENSE)
[![Tests](https://img.shields.io/badge/tests-75%20pasando-success)](.)
[![Cobertura](https://img.shields.io/badge/cobertura-%E2%89%A599%25-success)](.)
[![Multi-Agente](https://img.shields.io/badge/agentes-5%20plataformas-purple)](agents/)

**Versión:** 2.0.0 | **Licencia:** MIT | **Idioma:** 🇬🇧 EN / 🇪🇸 ES

**Autor:** Francisco J Bernades  
**GitHub:** [@exchanet](https://github.com/exchanet)  
**Repositorio:** [method_enterprise_builder_planning](https://github.com/exchanet/method_enterprise_builder_planning)

---

## 🌟 ¿Por qué usar este método?

### Para equipos que construyen:
- **Banca y Fintech**: Pasarelas de pago, plataformas de trading, sistemas de compliance regulatorio
- **Salud**: Historiales clínicos HIPAA, plataformas de telemedicina, software de dispositivos médicos
- **E-commerce a escala**: SaaS multi-tenant, marketplaces de alto tráfico, inventario distribuido
- **Gobierno y Defensa**: Sistemas security-first, audit trails, infraestructura de misión crítica
- **SaaS Enterprise**: Despliegues multi-región, SLA 99.99%, compliance RGPD/SOC2

### Qué obtienes:
- ✅ **Decisiones de arquitectura sistemáticas** documentadas como ADRs con alternativas rechazadas
- ✅ **Identificación de riesgos** (modelo de amenazas STRIDE) antes de escribir código
- ✅ **Descomposición en micro-tareas** (≤50 líneas) para desarrollo paralelo
- ✅ **Estrategia de tests** con requisito de cobertura ≥99%
- ✅ **Mapeo de compliance** (ISO 27001, RGPD, PCI-DSS, SOC2)
- ✅ **Quality gates automatizados** vía templates CI/CD
- ✅ **Entrega basada en evidencia** con métricas y reportes de sign-off

---

## Métodos complementarios recomendados

- [Method Modular Design](https://github.com/exchanet/method_modular_design) — Patrón de arquitectura Core + Packs
- [Método PDCA-T](https://github.com/exchanet/method_pdca-t_coding) — Ciclo de aseguramiento de calidad (cobertura de tests ≥99%)

---

## ¿Qué es esto?

**Method Enterprise Builder Planning** es un **framework híbrido universal** que combina:
- **Sistema de prompts estructurados** para agentes de IA (Cursor AI, Claude Code, Kimi Code, Windsurf, Google Antigravity)
- **Herramientas ejecutables independientes** (ADR Validator, Microtask Linter) para quality gates automatizados
- **Templates de integración CI/CD** para GitHub Actions, GitLab CI, Azure DevOps y Jenkins

El nombre **Builder** refleja el alcance integral del método: no solo *planifica* — orquesta la *construcción completa* de software enterprise-grade, desde el análisis inicial de stakeholders hasta las decisiones de arquitectura, endurecimiento de seguridad, descomposición en micro-tareas, estrategia de tests (≥99% cobertura) y sign-off de entrega basado en evidencia.

### Arquitectura multi-agente

A diferencia de frameworks específicos de un solo agente, esta metodología funciona con **5 plataformas líderes de IA para desarrollo**:

| Plataforma | Adaptador | Instalación |
|---|---|---|
| **Cursor AI** | `.cursor/` rules + skills | Express o manual |
| **Claude Code** | `CLAUDE.md` + `.claude/` | Copiar a raíz del proyecto |
| **Kimi Code** | `KIMI.md` | Archivo único |
| **Windsurf Cascade** | `WINDSURF.md` | Archivo único |
| **Google Antigravity** | `AGENTS.md` + `GEMINI.md` + `.agent/skills/` | Paquete completo de skills |

Todos los adaptadores siguen el **mismo protocolo de 8 fases**, garantizando consistencia independientemente del agente de IA que uses.

### Naturaleza híbrida: Prompts + Ejecutables

**Prompts estructurados** guían al agente en fases de planificación sistemática.  
**Herramientas ejecutables** proporcionan validación determinista que complementa el criterio del agente:

- **ADR Validator**: 11 reglas enterprise (estructurales, negocio, compliance) — bloquea estado Accepted si no cumple requisitos
- **Microtask Linter**: Fuerza ≤50 líneas efectivas por archivo, sugiere divisiones automáticas
- **Gates CI/CD**: Checks de calidad automatizados en tu pipeline

**Qué garantiza esto:** Proceso sistemático de 8 fases con cumplimiento de calidad automatizado en gates críticos.

**Qué no garantiza:** Outputs idénticos bit a bit en cada ejecución. El agente aplica juicio arquitectónico dentro de la estructura — el comportamiento intencionado para diseño de sistemas complejos.

### Niveles de calidad de software objetivo

| Estándar | Descripción |
|---|---|
| Enterprise-grade | Alta carga de usuarios, transacciones complejas, estándares de seguridad estrictos |
| Software de misión crítica | Tolerancia cero al tiempo de inactividad, prevención de fallos catastróficos |
| Alta disponibilidad (HA) | Arquitectura con 99.999% de uptime (5 nines) |
| Seguridad por diseño | Seguridad integrada desde la arquitectura, no añadida al final |
| Ingeniería de sistemas escalables | Capacidad para manejar crecimiento masivo de datos y transacciones |
| Cumplimiento ACID | Atomicidad, Consistencia, Aislamiento, Durabilidad en todas las transacciones |
| RegTech / Compliance | ISO 27001, ISO/IEC 25000 (SQuaRE), CMMI nivel 3+, RGPD, SOC2, PCI-DSS |

---

## 🚀 v2.0.0 — De solo-Cursor a framework universal multi-agente

| Componente | Qué hace | Por qué importa |
|---|---|---|
| **Soporte Multi-Agente** | Cursor AI, Claude Code, Kimi Code, Windsurf, Google Antigravity | Usa con **cualquier agente líder de IA** — misma metodología, mismas 8 fases |
| **ADR Validator** | CLI: 11 reglas enterprise (estructurales, negocio, compliance) | **Quality gate de arquitectura automatizado** — bloquea Accepted si no cumple requisitos |
| **Microtask Linter** | Fuerza ≤50 líneas efectivas por archivo | **Habilita desarrollo paralelo** — sugiere divisiones automáticas para archivos grandes |
| **Templates CI/CD** | Listos para usar: GitHub Actions, GitLab CI, Azure DevOps, Jenkins | **Quality gates en tu pipeline**: check de cobertura, linting de micro-tareas, validación de entrega |
| **Herramientas Ejecutables** | Validadores TypeScript con ≥99% cobertura de tests | **Validación determinista** — no solo prompts, automatización real |

### Migración desde v1.x

> **Breaking change:** Estructura de directorios refactorizada para soporte multi-agente.  
> **Antiguo:** `.cursor/` en raíz  
> **Nuevo:** `agents/cursor/.cursor/`, `agents/claude-code/`, `agents/antigravity/`, etc.

**Migración automática:**
```bash
# Windows
powershell -File scripts/migrate-to-v2.ps1

# macOS / Linux
bash scripts/migrate-to-v2.sh
```

Ver [MIGRATION-v2.md](docs/MIGRATION-v2.md) para guía de migración detallada.

---

## 📚 Véelo en acción

### Walkthrough completo ejecutado

Lee el **[walkthrough de Autorización de Pagos Bancarios](examples/banking-walkthrough.md)** — una **sesión real de agente** construyendo un sistema de pagos enterprise desde cero:

- **Fase 1**: Mapa de stakeholders (producto, seguridad, compliance, DevOps)
- **Fase 2**: Backlog de micro-tareas (32 tareas, ≤50 líneas cada una)
- **Fase 3**: Análisis de riesgos (modelo de amenazas STRIDE: SQL injection, MITM, escalada de privilegios)
- **Fase 4-5**: 7 ADRs con alternativas rechazadas (elección de BD, cifrado, idempotencia)
- **Fase 6**: Implementación TypeScript con ≥99% cobertura de tests
- **Fase 7**: Reporte de entrega con métricas y evidencia de compliance
- **Fase 8**: Documentación de handover para despliegue en producción

**Sin placeholders, sin ejemplos sintéticos.** Outputs reales generados por la metodología.

---

## 🏗️ Qué puedes construir con esto

### Ejemplos por industria

| Dominio | Ejemplo de Sistema | Requisitos Clave Abordados |
|---|---|---|
| **Banca** | Pasarela de autorización de pagos | Compliance PCI-DSS, transacciones ACID, detección de fraude, audit trails |
| **Salud** | Historiales clínicos electrónicos (EHR) | Compliance HIPAA, cifrado de datos, acceso basado en roles, gestión de consentimiento |
| **E-commerce** | Marketplace multi-tenant | Escalado horizontal, consistencia eventual, idempotencia, rate limiting |
| **Seguros** | Workflow de procesamiento de reclamaciones | Diseño de máquina de estados, tracking de SLA, reporting regulatorio, disaster recovery |
| **Cadena de Suministro** | Tracking de inventario en tiempo real | Arquitectura de alta disponibilidad, transacciones distribuidas, resolución de conflictos |
| **Gobierno** | Verificación de identidad de ciudadanos | Seguridad por diseño, arquitectura zero-trust, compliance RGPD, pruebas de penetración |

### Patrones técnicos cubiertos

- **Arquitectura**: Microservicios, event-driven, CQRS, patrones saga, API gateway
- **Datos**: Transacciones ACID, consistencia eventual, sharding, replicación, data lakes
- **Seguridad**: Zero-trust, cifrado en reposo/tránsito, RBAC, OAuth2/OIDC, logs de auditoría
- **Escalabilidad**: Escalado horizontal, estrategias de caché, CDN, balanceo de carga
- **Compliance**: Mapeo de RGPD, HIPAA, PCI-DSS, SOC2, ISO 27001

---

## Inicio rápido

### Instalación express (recomendado)

**Para Cursor AI**:
1. Descarga el repositorio como `.zip` desde [GitHub](https://github.com/exchanet/method_enterprise_builder_planning) → descomprime
2. Copia la ruta de la carpeta (ej: `C:\Users\tu-nombre\Downloads\method-enterprise_builder_planning`)
3. Cursor → Nuevo chat de agente → Pega la ruta:
   ```
   Instala este método globalmente: C:\Users\tu-nombre\Downloads\method-enterprise_builder_planning
   ```
4. Reinicia Cursor → Usa con: `/method-enterprise_builder`

**Para otros agentes**:

```bash
# Clona el repositorio
git clone https://github.com/exchanet/method_enterprise_builder_planning.git
cd method_enterprise_builder_planning

# Instala para tu agente
bash scripts/migrate-to-v2.sh --project=/ruta/a/tu-proyecto --agent=cursor
# Opciones: cursor, claude-code, kimi-code, windsurf, antigravity
```

**Instalación global** (disponible en todos los proyectos):
```bash
# Cursor AI
cp -r agents/cursor/.cursor ~/.cursor/

# Claude Code
cp agents/claude-code/CLAUDE.md ~/.config/claude/
cp -r agents/claude-code/.claude ~/.config/claude/

# Antigravity
cp agents/antigravity/AGENTS.md ~/.config/antigravity/
cp -r agents/antigravity/.agent ~/.config/antigravity/
```

Ver [agents/README.md](agents/README.md) para instalación detallada por plataforma.

### Instalación manual

```bash
# Clonar repositorio
git clone https://github.com/exchanet/method_enterprise_builder_planning.git
cd method_enterprise_builder_planning

# Copiar a tu proyecto
cp -r .cursor /ruta/a/tu/proyecto/
```

Instala también los métodos complementarios:

```bash
# Method Modular Design (patrón Core + Packs)
git clone https://github.com/exchanet/method_modular_design_cursor.git
cp -r method_modular_design_cursor/.cursor /ruta/a/tu/proyecto/

# Método PDCA-T (ciclo de aseguramiento de calidad)
git clone https://github.com/exchanet/method_pdca-t_coding_Cursor.git
cp -r method_pdca-t_coding_Cursor/.cursor/rules/METODO-PDCA-T.md /ruta/a/tu/proyecto/.cursor/rules/
cp -r method_pdca-t_coding_Cursor/.cursor/skills/metodo-pdca-t /ruta/a/tu/proyecto/.cursor/skills/
```

---

## Activación

Una vez instalado, activa con cualquiera de estas frases:

```
/method-enterprise_builder

"Planifica feature enterprise: [descripción]"
"Diseña sistema de misión crítica: [tipo de sistema]"
"Crea módulo ACID-compliant para [feature]"
"Construye componente de alta disponibilidad con SLA 99.99%"
"Implementa módulo con seguridad por diseño, audit trail y cumplimiento RGPD"
```

Cursor te guiará automáticamente a través del ciclo completo de 8 fases.

---

## El Ciclo Builder de 8 Fases

```
FASE 1: Análisis de Contexto Enterprise
         │  Clasificación del sistema · Stakeholders · Entorno regulatorio
         ▼
FASE 2: Requisitos No Funcionales (RNF)
         │  SLOs de rendimiento · SLA de disponibilidad · Escalabilidad · Seguridad
         ▼
FASE 3: Matriz de Riesgos
         │  Modelo de amenazas STRIDE · Catálogo de riesgos técnicos · Mitigaciones
         ▼
FASE 4: Descomposición en Micro-Tareas (PDCA-T)
         │  Feature → Dominio → Capa → Micro-tareas ≤50 líneas con DAG de dependencias
         ▼
FASE 5: Decisiones de Arquitectura (ADR)
         │  Selección de patrón · Diagramas C4 · Mapeo a Packs · ADR por decisión
         ▼
FASE 6: Seguridad y Mapeo de Compliance
         │  STRIDE por módulo · Matriz RBAC · Fronteras ACID · Matriz de compliance
         ▼
FASE 7: Estrategia de Tests
         │  Pirámide de tests · Quality gates · Tests de carga · CI/CD gates
         ▼
FASE 8: Reporte de Entrega
         │  Sign-off con evidencia · Métricas de tests · Seguridad · Checklist de compliance
```

---

## Estructura del Repositorio

```
method-enterprise_builder_planning/
├── .cursor/
│   ├── rules/
│   │   ├── METHOD-ENTERPRISE-BUILDER-PLANNING.md  ← regla principal (trigger: manual)
│   │   ├── ENTERPRISE_ARCHITECTURE.md
│   │   ├── ENTERPRISE_SECURITY.md
│   │   ├── ENTERPRISE_SCALABILITY.md
│   │   ├── ENTERPRISE_COMPLIANCE.md
│   │   ├── ENTERPRISE_TESTING.md
│   │   └── ENTERPRISE_MICROTASK_PLANNER.md
│   └── skills/
│       └── method-enterprise-builder-planning/
│           ├── SKILL.md                        ← skill orquestador principal
│           ├── architecture-planning.md
│           ├── security-planning.md
│           ├── scalability-planning.md
│           ├── compliance-planning.md
│           ├── microtask-decomposition.md
│           ├── testing-strategy.md
│           └── delivery-report.md
├── core/
│   └── planning-engine/                        ← capa Core (solo infraestructura)
├── packs/
│   ├── enterprise-architecture-pack/
│   ├── security-compliance-pack/
│   ├── high-availability-pack/
│   ├── testing-coverage-pack/
│   └── acid-compliance-pack/
├── examples/
│   ├── banking-walkthrough.md        ← ✅ walkthrough ejecutado completo (empieza aquí)
│   ├── banking-system-plan.md
│   ├── high-availability-saas-plan.md
│   └── mission-critical-api-plan.md
├── docs/
│   ├── INSTALLATION.md
│   ├── USAGE.md
│   └── ENTERPRISE-STANDARDS-REFERENCE.md
├── README.md
└── README.es.md
```

---

## Schemas de configuración y propiedades `x-ui`

Cada pack y el Core incluyen un `config.schema.json` que documenta los parámetros configurables.
Algunos campos llevan anotaciones `x-ui` (por ejemplo `"widget": "slider"`, `"widget": "checkbox-group"`).

**Estos son marcadores de diseño para una futura interfaz de configuración — actualmente no existe ninguna GUI que los renderice.** Sirven para dos propósitos hoy: documentar la UX prevista para cada campo y ayudar al agente Cursor AI a describir las opciones en lenguaje natural. No tienen ningún efecto en tiempo de ejecución.

---

## Packs disponibles

| Pack | Activado en fase | Proporciona |
|---|---|---|
| `enterprise-architecture-pack` | Fase 5 | Plantillas ADR, diagramas C4, árboles de decisión |
| `security-compliance-pack` | Fase 3, 6 | Plantillas STRIDE, matrices RBAC, checklists de auditoría |
| `high-availability-pack` | Fase 2, 5 | Definiciones SLA/SLO, estrategias de failover, chaos engineering |
| `testing-coverage-pack` | Fase 4, 7 | Pirámide de tests, requisitos de cobertura, plantillas k6 |
| `acid-compliance-pack` | Fase 4, 6 | Fronteras de transacción, estrategias rollback, idempotencia |

---

## Métodos relacionados

| Método | Rol |
|---|---|
| [Method Modular Design](https://github.com/exchanet/method_modular_design_cursor) | Patrón de arquitectura (Core + Packs) usado en todo el código generado |
| [Método PDCA-T](https://github.com/exchanet/method_pdca-t_coding_Cursor) | Ciclo de calidad (cobertura ≥99%) aplicado a cada micro-tarea |

---

## Licencia

MIT — ver archivo [LICENSE](LICENSE).

---

## Autor

**Francisco J Bernades**  
GitHub: [@exchanet](https://github.com/exchanet)
