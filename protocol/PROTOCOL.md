# Protocolo de Respaldo de Nova (Backstage) — v1.0

## Objetivos
- Mantener un registro seguro y estructurado de aprendizajes y entregables.
- Garantizar continuidad de proyectos en caso de pérdida de memoria o archivos.
- Facilitar la recuperación rápida por cualquier tercero o IA.

## Capas de Respaldo
1) **Memoria en Nova**
   - Instrucciones permanentes, acuerdos, preferencias, inventario de proyectos.
   - Riesgo: puede perderse si hay reset/cambio de modelo.

2) **Carpeta Drive estructurada**
   - Documentos maestros, scripts, PDFs, tableros (Looker), datasets (Sheets).
   - Regla: todo entregable final vive aquí.

3) **Repositorio GitHub**
   - Carpeta `memory/`: snapshots semanales de personalización (`.md`, `.json`).
   - Carpeta `snapshots/`: PDFs trimestrales (ligero y técnico).
   - Carpeta `protocol/`: este documento y otros manuales.

4) **Copias frías**
   - Zip con carpetas críticas + export de memoria.
   - Ubicación: disco externo / nube secundaria.
   - Periodicidad: mensual.

## Periodicidad
- **Semanal**: snapshot en `memory/` (fechado + latest).
- **Mensual**: export de documentos clave en PDF.
- **Trimestral**: snapshot PDF en `snapshots/` (ligero y técnico).
- **Anual**: revisión integral del protocolo y estructura de carpetas.

## Roles
- **Nova**: generar dumps semanales, recordar snapshots trimestrales.
- **Ulises**: aprobar estructura, subir archivos críticos a Drive/GitHub.
- **GitHub**: repositorio oficial de memoria y protocolo.
- **Drive**: repositorio secundario, más orientado a datos de proyectos.

## Identidad gráfica
- Logo/portada “Protocolo de Respaldo” (Backstage vibes).
- Paleta: Innovasport Group + neutros.
- Aplicación en todos los PDFs/documentos oficiales.

## Checklist rápido
- [ ] Memoria semanal generada (`memory/`).
- [ ] PDFs trimestrales publicados (`snapshots/`).
- [ ] Copias frías actualizadas (mensual/trimestral).
- [ ] Identidad gráfica aplicada.

---

## Notas técnicas

### A. Exportar Google Sheets para consulta en Nova
- Formato CSV público:
  `https://docs.google.com/spreadsheets/d/{SHEET_ID}/export?format=csv&gid={GID}`

### B. Exportar Google Docs para lectura pública
- Texto plano:
  `https://docs.google.com/document/d/{DOC_ID}/export?format=txt`
- PDF:
  `https://docs.google.com/document/d/{DOC_ID}/export?format=pdf`

### C. GitHub convención de carpetas
```
backups/
  memory/       ← snapshots semanales (.md, .json)
  snapshots/    ← PDFs trimestrales (ligero, técnico)
  protocol/     ← este PROTOCOL.md y anexos
```

### D. Versionado de memoria
- `nova_memory_YYYY-MM-DD.md` → histórico.
- `nova_memory_latest.md` → siempre actualizado.
