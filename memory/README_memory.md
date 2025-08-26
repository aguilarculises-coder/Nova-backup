# 📂 Carpeta `memory/`

Esta carpeta contiene los **snapshots semanales de memoria de Nova**.

## Convención de archivos
- `nova_memory_YYYY-MM-DD.md` → Snapshot histórico con fecha (ejemplo: `nova_memory_2025-08-25.md`).
- `nova_memory_latest.md` → Copia siempre actualizada del snapshot más reciente.

## Frecuencia
- **Semanal**: se genera un nuevo archivo con fecha.
- Se actualiza también el archivo `latest` para que apunte a la última versión.

## Uso
- Para consultas rápidas en GitHub/Raw, usar siempre `nova_memory_latest.md`.
- Para auditoría o recuperar un estado previo, revisar los archivos con fecha.

---

✦ Esta carpeta forma parte del **Protocolo de Respaldo de Nova (Backstage)**.
