# Deployment prerequisites

Render backend service: srv-dak191e1egvs73960so0
Backend URL: https://t332-v2-ramsey-infill.onrender.com
Vercel portal project: prj_RqE6qYyTRd7OjXfhFtymQ41qPY7T
Vercel team: team_fy6FPplKTSfbW0kv9dpIC39t
PostgreSQL instance: dpg-dak183bm8hqs73915e00-a
Region: singapore
Isolated schema: t332_v2

Database and auth values are already configured privately in Render/Vercel environment variables. Do not expose them. Retain the configured bearer and Basic authentication checks. No real customer credentials or customer history is represented. All source parcel data comes from a public official GIS endpoint and excludes owner fields.

The free database expires 2026-10-14; source readiness must be rechecked if running after that date. No paid plan or automatic disk scaling is enabled. Do not upgrade plans.

To deploy changed backend code, use this exact Render service and verify actual deployed commit/state. To deploy portal code without Git auto-integration, send the portal directory files to this exact Vercel project and record actual source commit metadata. Do not infer a successful deploy from a commit. The initial scanner and portal integration return unavailable by design and are the contributor's implementation work.

Baseline rollback uses immutable repository commits and observed deployment IDs. Do not rollback other variations, shared database extensions or unrelated resources.
