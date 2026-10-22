# מוריד השירים

<p align="center">
  <img src="shots/main.webp" alt="מוריד השירים — החלון הראשי" width="760">
</p>

תוכנה בעברית לווינדוס להורדת שירים ופלייליסטים כ-MP3 — עם חיפוש סגור, מגן תוכן מובנה, מאיץ הורדות ותמיכה מלאה ברשת נטפרי.

**[לדף התוכנה ←](https://hanyna.github.io/morid/)**

**גרסה נוכחית: 10.12**

## הורדה

| קובץ | למי |
|------|-----|
| [morid_setup_10.12.exe](https://github.com/hanyna/morid/releases/latest) | **התקנה ראשונה** — החבילה המלאה. כוללת את ffmpeg (ממיר ה-MP3), ומתקינה את רכיב WebView2 אם הוא חסר |
| [morid_update_10.12.exe](https://hanyna.github.io/morid/morid_update_10.12_web.exe) | **עדכון** של תוכנה שכבר מותקנת — קובץ קטן ומהיר (ובמחשב חדש הוא גם מתקין אותה) |

כל הגרסאות: [דף ההורדות](https://github.com/hanyna/morid/releases)

## צילומי מסך

| חיפוש | פלייליסט |
|:---:|:---:|
| <img src="shots/search.webp" alt="חיפוש" width="380"> | <img src="shots/playlist.webp" alt="פלייליסט" width="380"> |
| **תור הורדות** | **צלצולים** |
| <img src="shots/queue.webp" alt="תור הורדות" width="380"> | <img src="shots/ring.webp" alt="צלצולים" width="380"> |

## מה חדש בגרסה 10.12

### מהירות והורדות
- **"פותר החידות של יוטיוב" מובנה** בתוכנה ועובד מיד — בלעדיו יוטיוב האט את ההורדות בכוונה והסתיר איכויות
- **ההמרה ל-MP3** לא מחכה יותר לשרת שהסינון חוסם, ובמחשב חלש לא רצות שתי המרות בו-זמנית
- **מאיץ ההורדות** מהיר יותר (חלקים גדולים במקום בקשות קטנות) ונכנס לפעולה כבר מ-8MB
- **הורדות אמינות יותר** מול השינויים האחרונים ביוטיוב: מנוע עדכני עם חזרה אוטומטית לגרסה הקודמת אם עדכון לא עובד, ופחות המתנות חוזרות על שיר שנכשל

### נטפרי, רימון ואתרוג
- התוכנה פונה ליוטיוב קודם כמו דפדפן.
- כשהסינון מחליף קובץ בסרטון חסימה ("אנחנו מגנים עליך!") הוא לא נשמר בשם השיר, התוכנה מנסה דרך אחרת, ובסוף מוצגת הודעה ברורה.
- הפרדה ברורה בין המגן של התוכנה, הסינון ברשת והאנטי-וירוס — כל שורה שנכשלה מסומנת מי חסם.

### המגן
- **המגן לא חוסם סרטונים כשרים** בגלל מילה שמסתתרת בתוך מילה אחרת ("לבנות", "שירי ילדות", "פריטה") — כל מילה נבדקת כמילה שלמה

### תיקונים
- תוקנו קישורי ספוטיפיי
- שמירת התוספות (עטיפה, חיתוך שקט...) בין הפעלות
- "נסה שוב את הכושלים" אחרי ביטול, ו"בטל" שעוצר מיד
- פלייליסט שלא נטען נפתח בחלון הפלייליסט עם הסבר במקום להוריד בשקט רק שיר אחד

הגרסאות הקודמות: [היסטוריית גרסאות](CHANGELOG.md)

## In English

**Morid** is a Hebrew-language Windows app for downloading songs and playlists as MP3. It includes a curated search, a built-in content filter, a multi-connection download accelerator, and full support for filtered networks (NetFree). Download the installer from the [Releases page](https://github.com/hanyna/morid/releases) or visit the [project website](https://hanyna.github.io/morid/).

## איך מפרסמים גרסה חדשה (למפתח)
1. Releases ← Draft a new release ← תג `v<גרסה>` (למשל `v10.12`)
2. גוררים את `morid_update_<גרסה>.exe` ואת `morid_setup_<גרסה>.exe` (החבילה המלאה) — בשמות האלה בדיוק, באנגלית
3. Publish release — התוכנות מגרסה 10.6 ומעלה מוצאות את הגרסה לבד
4. בשביל גרסאות 10.5 ומטה ונטפרי: עותק של קובץ העדכון בשם `morid_update_<גרסה>_web.exe` בשורש המאגר, ועדכון `version.json`

## רישיון
כל הזכויות שמורות © LANDESBERG · ליצירת קשר: hanynalandesberg@gmail.com

התוכנה משתמשת ברכיבי קוד פתוח: [yt-dlp](https://github.com/yt-dlp/yt-dlp) (רישיון Unlicense) ו-[FFmpeg](https://ffmpeg.org) (רישיון GPL, גרסה 2 ואילך; ה-build המדויק שבשימוש: [BtbN/FFmpeg-Builds](https://github.com/BtbN/FFmpeg-Builds/releases)). נוסח הרישיונות המלא זמין גם בתוך התוכנה, בתפריט תחזוקה ← אודות.
