---
title: <% tp.file.title %>
aliases:
created: <% tp.date.now("YYYY-MM-DD") %>
modified: <% tp.file.last_modified_date("YYYY-MM-DD") %>
lab_url: ""
difficulty: ""
platform:
tags:
  - bug-bounty
---
# <% tp.file.title %>
  

---

  

## Metadata

- **Judul Lab:**

- **URL Lab:**

- **Tanggal:** <% tp.date.now("YYYY-MM-DD") %>

- **Difficulty:**

- **Kategori:** (e.g. SQLi, XSS, IDOR, SSRF)

- **Env / VM:** (mis. DVWA local, WebGoat, custom VM)

- **Status:** ☐ In Progress  ☐ Solved  ☐ Verified  ☐ Archived

  

> [!info]

> Gunakan _frontmatter_ untuk memudahkan indexing (Dataview). Jangan hapus properti `lab_url` & `difficulty`.

  

---

  

## 1) Objective

Tuliskan tujuan lab ini dan apa yang diminta (singkat).

  

## 2) Recon & Footprinting

- Target:

- Subpaths ditemukan:

- Parameter yang tampak berbahaya:

  - `param1` — catatan

  

> [!tip]

> Simpan semua request/response Burp sebagai file `.txt` terlampir (`attachments/`), dan embed di sini ketika perlu: `![[attachments/req-1.txt]]`.

  

---

  

## 3) Step-by-step Exploitation (Repro)

Tuliskan langkah-langkah yang dilakukan untuk mencapai exploit. Cantumkan setiap percobaan sebagai entri terpisah.

  

### Attempt 1 — Tanggal: <% tp.date.now("YYYY-MM-DD") %>

- **Payload:**

  

```txt

# Burp request (simpan juga di attachments)

GET /vulnerable?input=PAYLOAD HTTP/1.1

Host: vulnerable.local

...

```

  

- **Response (ringkasan):**

- **Observasi:**

- **Status:** ☐ Working  ☐ Partial  ☐ Failed

  

### Attempt 2 — ...

  

---

  

## 4) Proof of Concept (PoC)

Sertakan PoC lengkap (curl, Python, Burp intruder config, dll).

  

```bash

# contoh curl PoC

curl -i "http://vulnerable.local/vuln?input=<payload>"

```

  

---

  

## 5) Impact & Root Cause

- **Impact (mis. Remote code exec, data leak):**

- **CWE / CVE (jika relevan):**

- **Root cause:**

  

> [!warning]

> Jangan menyertakan exploit yang merusak atau data sensitif publik jika lab memuat data nyata.

  

---

  

## 6) Mitigation / Fix Recommendations

Tuliskan rekomendasi teknis yang jelas untuk developer / owner.

  

---

  

## 7) Artifacts & Evidence

- Screenshots: `![[screenshots/1.png]]` `![[screenshots/2.png]]`

- Burp file: `![[attachments/burp-state.xml]]`

- Request files: `![[attachments/req-1.txt]]`

  

---

  

## 8) CVSS & Disclosure Notes

- **CVSS (estimasi):**

- **Disclosure plan / notes:** (mis. private disclosure simulated)

  

---

  

## 9) Lessons Learned & Next Steps

- Hal apa yang dipelajari

- Follow-up lab / materi untuk dipelajari

  

---

  

## Checklist (use Tasks plugin)

```
- [ ] Save full Burp project

- [ ] Export vulnerable request/response to `attachments/`

- [ ] Take screenshots of successful payload

- [ ] Write PoC script

- [ ] Add tags & update YAML
```

  

---

  

## Dataview summary (letakkan di halaman index)

```dataview

TABLE difficulty, lab_url, file.mtime as updated

FROM "PortSwigger Labs"

WHERE contains(tags, "portswigger")

SORT file.mtime desc

```

  

---