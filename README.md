# yos-kl-download — הורדות ועדכונים

ערוץ ההפצה הציבורי של **KioskLock**.
כאן מתפרסמות גרסאות השחרור בלבד. קוד המקור נמצא במאגר פרטי נפרד.

## הורדת הגרסה האחרונה

עמוד השחרורים: **[Releases](../../releases/latest)**

| קובץ | תיאור |
|------|-------|
| `KioskLock.exe` | תוכנת הקיוסק |
| `KioskAdmin.exe` | תוכנת הניהול |
| `SHA256SUMS.txt` | חתימות לאימות הקבצים |

## עדכון אוטומטי

הקיוסק בודק את הגרסה האחרונה דרך ה-API הציבורי של GitHub:

```
https://api.github.com/repos/yossi-computers/yos-kl-download/releases/latest
```

מספר הגרסה נלקח מתגית השחרור בתבנית `vX.Y.Z`, וקובצי ההתקנה מצורפים
כ-assets לאותו שחרור. הבדיקה אינה דורשת התחברות.

## אימות קובץ שהורדתם

```powershell
Get-FileHash .\KioskLock.exe -Algorithm SHA256
```

ההשוואה מול השורה המתאימה ב-`SHA256SUMS.txt` של אותו שחרור.
