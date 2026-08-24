# 🧪 Proyectos independientes

> Scripts y herramientas que no viven en AleksTools pero demuestran
> mi trabajo autónomo en automatización y seguridad.

---

## 1. Threat Intel Monitor (Python) ⭐

**Proyecto:** Monitor automático de amenazas que consulta CISA KEV + NVD API y reporta CVEs explotadas activamente.

**Por qué existe:** aprendo lo que se explota HOY (la vanguardia real) sin pisar foros oscuros — todo de fuentes públicas y verificadas.

```bash
python3 threat_intel_monitor.py
# → 🛡️ CISA KEV — vulnerabilidades explotadas activamente
# → 🐛 CVEs publicadas últimas 48h (CVSS >= 7)
```

**Skills:** Python, API REST, JSON, parsing, automatización cron
**Uso real:** los equipos SOC/CTI hacen exactamente esto — monitorear feeds de amenazas

---

## 2. Kali desechable en Docker (Bash)

**Proyecto:** Script que levanta una instancia Kali efímera en Docker para labs sin dejar rastro.

```bash
./kali-docker.sh run    # → Kali temporal
./kali-docker.sh stop   # → borra TODO (cero rastro)
```

**Skills:** Docker, Bash, automatización de entornos efímeros

---

## 3. Suite de recon automatizada (Bash + Python)

**Proyecto:** Pipeline que orquesta las herramientas de AleksTools (subenum → alive_checker → headers)
para hacer recon completo del target con un solo comando.

**Skills:** Bash scripting, pipes, orquestación de herramientas

---

## 📌 Cómo agrego un proyecto

1. Explico el problema que resuelve
2. Muestro el uso real
3. Adjunto (si aplica) el repo/enlace
4. Listo los skills que demuestra

> Nuevos proyectos en camino: **SQLi tester (Python)**, **Bash recon automator**, **AI prompt-injection toolkit**