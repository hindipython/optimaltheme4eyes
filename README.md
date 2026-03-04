# IPS Dark Modern — High Focus Theme (Antigravity)

Минималистичная тёмная тема под IPS.  
Оптимизирована для долгой работы без головной боли и перегруза.
---

## 🎯 Цветовая схема

```json
{
  "background": "#141414",
  "text": "#CFCFCF",
  "keywords": "#A3BE8C",
  "strings": "#8FBCBB",
  "functions": "#81A1C1",
  "warnings": "#D08770",
  "fontSize": 15,
  "lineHeight": 1.5
}
```

## 1️⃣ Найти папку установки Antigravity
```powershell
Get-ChildItem "C:\" -Directory -Filter "*Antigravity*" -Recurse -ErrorAction SilentlyContinue | Select FullName

## 2️⃣ Найти папку extensions внутри установки
```powershell
Get-ChildItem "ПУТЬ_К_ANTIGRAVITY" -Directory -Recurse -Filter "extensions" | Select FullName

##3️⃣ Создать файл темы
```powershell
New-Item -ItemType File -Path "ПУТЬ_К_EXTENSIONS\my-theme\package.json" -Force
```powershell
New-Item -ItemType File -Path "ПУТЬ_К_EXTENSIONS\my-theme\themes\theme.json" -Force

📁 Итоговая структура
extensions\
  └── my-theme\
      ├── package.json
      └── themes\
          └── theme.json
