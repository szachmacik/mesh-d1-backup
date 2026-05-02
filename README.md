# HOLON Mesh D1→Turso Backup

**Database Backup & Export**

- `kb-metadata-turso.sql` - SQL INSERT statements (476KB)
- `kb-metadata-turso.csv` - CSV export (317KB)

**Info:**
- Records: 5800
- Tables: 11 (mesh_metrics, morphic_field, kv_store, task_queue, routing_cache, holon_lessons, mesh_devices, sentinel_logs, dev_tasks, dev_workers, dev_budget)
- Source: D1 (Cloudflare)
- Destination: Turso
- Date: 2026-05-02

**Usage:**

Import to Turso:
```bash
turso db shell kb-metadata-turso < kb-metadata-turso.sql
```

Or in Turso Studio SQL Console:
```
Copy-paste content of kb-metadata-turso.sql
```
