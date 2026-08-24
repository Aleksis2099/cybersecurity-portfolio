# 🐛 Bug Bounty — Hallazgos (ética y resumen)

> **Principio:** solo se comparte información ya pública, sin datos sensibles,
> sin PII, sin pasos que permitan re-explotar un target sin autorización.

---

## 📋 Mis hallazgos hasta ahora

### 1. Info Disclosure via OAuth2 (MercadoLibre)
- **Programa:** MercadoLibre / adminml.com
- **Tipo:** Information Disclosure (OAuth2 flow)
- **Impacto:** Exposición de URL interna (Okta admin) no accesible públicamente
- **Estado:** Reportado (informativo)
- **Año:** 2026

**¿Qué aprendí?**
- Escudriñar el flujo OAuth2 completo (redirect_uri, state, nonce)
- Los endpoints internos a veces se revelan en respuestas de terceros (Okta)
- El "info disclosure" suele ser informativo — la lección: buscar bugs con
  impacto real (XSS, IDOR, SQLi, SSRF, ATO)

### 2. Cookie Misconfiguration / CSP issues (MercadoLibre)
- **Programa:** MercadoLibre
- **Tipo:** Security misconfiguration (cookies / Content-Security-Policy)
- **Estado:** Reportado
- **Año:** 2026

---

## 🧠 Mi enfoque (metodología de caza)

1. **Recon amplio** — subdominios, headers, stack (automatizado con AleksTools)
2. **Superficie de ataque** — paneles, APIs, flujos de auth (OAuth2)
3. **Foco en impacto** — XSS / IDOR / SQLi / SSRF / ATO (lo que paga)
4. **Reporte profesional** — 1 bug por reporte, en inglés, con reproducción + impacto

---

## 🎯 Programas que exploro (públicos)

| Programa | Estado |
|----------|--------|
| MercadoLibre | Reportado (4) — defensas fuertes |
| Uber / Airbnb / Shopify / DoorDash / Reddit | En recon inicial |
| Rappi / Kavak / Cornershop | No públicos (404) |

---

## ⚠️ Disclaimer ético

Toda la investigación se realiza bajo los términos de los programas de bug bounty
autorizados, en cuentas propias, y con divulgación responsable. No hay re-explotación
ni divulgación de datos sensibles aquí.