# 🏴 Writeup — [Nombre de la máquina/room]

> **Plataforma:** TryHackMe / HackTheBox
> **Dificultad:** Easy / Medium / Hard
> **Fecha:** [DD-MM-YYYY]
> **Estado:** Resuelta / In progress

---

## 🎯 Resumen (TL;DR)

[2-3 líneas: qué máquina es, qué vulnerabilidad la compromete, qué consigues al final]

---

## 🗺️ Metodología

### 1. Reconocimiento

**Nmap:**
```bash
nmap -sV -sC -p- <IP>
```

**Resultado:**
| Puerto | Servicio | Versión |
|--------|----------|---------|
| 22/TCP | SSH | OpenSSH 8.2 |
| 80/TCP | HTTP | Apache 2.4.41 |
| 8080/TCP | ... | ... |

**Tecnologías detectadas:** [Apache? Nginx? WordPress? API?]

---

### 2. Enumeración / Análisis

[Qué encontraste: subdominios, directorios, parámetros, leaks...]

**Herramientas usadas:**
```bash
# mis propias tools
python3 subenum.py ejemplo.com -w wordlist.txt
python3 dir_scanner.py ...
```

**Hallazgo clave:** [la vulnerabilidad que abrirá la puerta]

---

### 3. Explotación

[El paso a paso del exploit — con comandos y explicación de POR QUÉ funciona]

```bash
# p.ej.: SQLi, LFI, credenciales débiles...
```

**Resultado:** [acceso obtenido / shell / dato crítico]

---

### 4. Post-explotación

[Escalada de privilegios, movimientos laterales, flags]

---

### 5. Banderas / Conclusión

| Flag | Validación |
|------|-----------|
| user.txt | ✅ |
| root.txt | ✅ |

---

## 🧠 Qué aprendí

- [Lección 1: técnica nueva / herramienta nueva]
- [Lección 2: qué haría distinto]
- [Lección 3: conexión con un CVE o técnica real]

---

## 🛠️ Herramientas usadas

`nmap` · `gobuster` · `burp` · `sqlmap` · `python3` · `my own tools (subenum, dir_scanner...)`

---

## ⚠️ Nota ética

Máquina resuelta en entorno autorizado (TryHackMe/HackTheBox). Toda la práctica se realiza únicamente en entornos legales.