---
title: Dashboard 🏠
created: 2025-07-23
modified: 2025-11-02
tags:
  - dashboard
---
# 📊 Dashboard 
[[Calendar View|Calendar]]  | [[Tasks Timeline]]  | [[Tasks Queries]]  

![[Calendar View]]

---

# ✅ Note Created Today
```dataview
TABLE title AS Title, created AS Created
FROM ""
WHERE date(created) = date(today)
SORT created DESC
```
# 📝 Last Notes Update Today
```dataview
TABLE title AS Title, modified AS Modified
FROM ""
WHERE date(modified) = date(today)
SORT modified DESC
```

---

# 🚩 CTF 

```dataview
TABLE title AS Title, created AS Created, modified AS Modified
FROM "CTF🚩" 
SORT modified DESC
```


# 📂 Journals 

```dataview
TABLE title AS Title, created AS Created, modified AS Modified
FROM "Journals🤓" 
SORT modified DESC
```

