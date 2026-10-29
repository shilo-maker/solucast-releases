# SoluCast

Worship presentation software for congregations: songs, Scripture, presentations and media on the screens, with a
phone remote, a live room for the congregation's phones, and an NDI feed for streaming. Hebrew‑first and right‑to‑left,
and fully in English.

**[English guide](#user-guide)** · **[מדריך בעברית](#מדריך-למשתמש)** · **[Report a problem](https://github.com/shilo-maker/solucast-releases/issues/new)**

## Download

Get the latest version from **[Releases](https://github.com/shilo-maker/solucast-releases/releases/latest)**.

| File | What it is |
| --- | --- |
| `Solucast-<version>-x64.exe` | The Windows installer — **start here** |
| `latest.yml`, `*.blockmap` | Used by the app to update itself; you don't need to download them |
| `solucast-<version>-source.zip` | The source code of that version (SoluCast is free software under the GPL‑3 licence) |

Windows may show **"Windows protected your PC"** the first time, because the installer isn't signed yet. Click
**More info → Run anyway**. After that, SoluCast updates itself: when a new version is ready it tells you, and installs
it when you choose.

---

# User guide

## 1. First start

The first time SoluCast opens it asks a few things. You can change all of them later in **Settings**.

- **Language** — Hebrew or English for the app itself.
- **What songs show on the screens** — **Original** (the song's own language only) or **Multi‑lingual** (several
  languages under each other).
- **Layers** — in Multi‑lingual, which languages appear and in what order (for example Hebrew, transliteration,
  English). Add or remove languages here.
- **Data location** — where your songs, services and themes are kept (normally `Documents\Solucast`). Put it in a
  folder that is backed up.

Then a short **quick start** walks through the six things you need. Open it again any time from the menu at the
bottom of the left bar → **Quick start guide**.

## 2. The service screen

Everything for a service is on one screen:

| Area | What it's for |
| --- | --- |
| **Preview** (top) | Exactly what the room's screens show. Under it: the layer buttons (Background, Slide, Overlays, Audio, Timer), **Clear all**, and **Blackout** |
| **Service** (middle) | The order of today's service — songs, readings, videos, announcements |
| **Library** (side) | Songs, the Bible, media and presentations, each with its own search |
| **Slides** (bottom) | The slides of the item you clicked in the service |
| **Left bar** | **Screens**, **Messages**, **Devices**, and the menu at the bottom (settings, account, help) |

## 3. Before the service

**Choose the projector.** Click **Screens** on the left bar and pick which screen is the projector. The same window
has a **Themes** tab: how songs, Bible passages, points and presentations look on each screen.

**Build the service.** Find a song, passage or file in the library and **double‑click** it (or drag it) to add it to
the service. Click an item in the service to see its slides. Right‑click an item for more: details, rename, a
background for that song, a loop, remove.

**Songs.**
- Songs come from the **solucast.app** song library and stay up to date by themselves. Songs you changed on this
  computer are kept as you changed them and get a cloud mark; click the mark → **Restore the cloud version** to take
  the library's version instead.
- **+** creates a new song. The song editor takes the lyrics in each language, the song's **key** and **chords**
  (type them in square brackets, ChordPro style, for example `[G]Amazing [C]grace`), and its **Copyright and CCLI**
  details.
- **Import** brings songs from OpenLP, ProPresenter, EasyWorship, ChordPro, OpenSong and CCLI SongSelect text files.

**The Bible.** Type a reference in the Bible tab's search — in Hebrew or English, for example `John 3:16`,
`יוחנן ג 16` or `Psalm 23-24`. Click a verse to show it; Shift‑click to show several. To add another translation, open
the version list and choose **Add a translation…** (from a file or the internet).

**Media and presentations.** Pictures and videos go up as a background behind the words or on their own. PowerPoint
and PDF files become presentations you click through like songs.

## 4. During the service

- **Next, then Take.** Double‑click the next item in the service to make it **next**. **Take** puts it on the screens,
  and the item after it becomes next.
- **Slides of the item that is up** go on the screens with **one click**, or with the **arrow keys**. This is the
  press you'll make dozens of times — it's instant.
- **Blackout** (beside **Clear all**, or the **B** key) darkens the room's screens and keeps the slide underneath.
  Press it again and the same words come straight back. The band's stage screen and the stream are not blacked out.
- **Clear all** takes everything off the screens: the slide, the background, overlays and sound. The layer buttons
  clear one layer at a time.
- **Original / Multi‑lingual** can be switched in the middle of a song (Settings → General).
- **A loop** (announcements, a countdown, music before the service): right‑click an item → **Loop…**. While it runs,
  its row in the service shows a badge with the countdown; the strip above the service shows it too, with a ✕ to stop
  it. It stops by itself when the first item of the service goes up.
- **Messages** on the left bar: a short message to the **stage** (only the band sees it), or **calling a parent** — the
  child's number appears on the room's screens until you remove it.

## 5. Phones and other devices

Click **Devices** on the left bar. The window has tabs:

- **Phone remote** — scan the code with your own phone or tablet and run the service from anywhere in the room: what's
  on the screen, the next item, all the slides, the service order, the library. A new item is prepared on the phone
  and only goes up when you tap **Take**; the slides of the song that's already up go up with one tap. Phones on the
  same Wi‑Fi connect directly; to connect over the internet as well, switch on **Phones over the internet** in the same
  window.
- **Live room** — the words on the congregation's own phones, at `live.solucast.app` with your congregation's code.
  Each person can choose their language and Bible translation.
- **The band's screen** — a separate code for the musicians: the current and next slide, the stage message, notes,
  chords and a clock.

The lock switch stops every phone at once.

## 6. Streaming and the nursery (NDI)

SoluCast can send its picture as an **NDI** feed to OBS, a streaming PC or a screen in the nursery. In **Screens**,
add a screen and switch on **NDI**. A feed that has no window of its own is sent with a transparent background, so in
OBS the words lie over your camera.

**In OBS** (with the DistroAV / NDI plugin): open the NDI source's properties and set **Latency Mode → Normal**. In the
other latency modes OBS drops the transparency and shows the words on solid black.

## 7. Settings and help

The button at the bottom of the left bar opens a menu: your congregation account (sign in / out), **Settings**, the
**Quick start guide**, **Online help** (this page), **Report a problem** and **Check for updates**.

- **Settings → Songs** — the song library sync and the **Song usage report (CCLI)**: which songs were used and how
  often, exported for your licence report.
- **Report a problem** saves a diagnostics file (no passwords or keys) and opens a page where you can describe what
  happened and attach it.

## 8. When something doesn't work

- **A phone can't connect over the Wi‑Fi, or OBS doesn't see the NDI feed.** Windows Firewall is probably blocking
  SoluCast. If Windows calls your network **Public**, make it **Private** (Settings → Network & internet → Wi‑Fi → your
  network → Private network), or allow SoluCast on Public networks in Windows Firewall. SoluCast shows a note with
  these buttons when it detects this.
- **OBS shows the words on black.** Set the NDI source's **Latency Mode** to **Normal** (see above).
- **A song doesn't update from the library.** It was changed on this computer, so it's kept as it is. Click its cloud
  mark → **Restore the cloud version** to take the library's version.
- **The screen is on the wrong monitor.** Open **Screens** and pick the projector again. If the projector was unplugged
  during the service, SoluCast hides its window and brings it back when the projector returns.
- **Anything else** — use **Report a problem** in the menu, or
  [open an issue](https://github.com/shilo-maker/solucast-releases/issues/new).

---

<div dir="rtl">

# מדריך למשתמש

## 1. הפעלה ראשונה

בפעם הראשונה SoluCast שואלת כמה דברים. אפשר לשנות את כולם אחר כך ב**הגדרות**.

- **שפה** — עברית או אנגלית לתוכנה עצמה.
- **מה רואים על המסכים בשירים** — **מקור** (רק שפת השיר) או **רב־לשוני** (כמה שפות זו מתחת לזו).
- **שכבות** — ברב־לשוני: אילו שפות מופיעות ובאיזה סדר (למשל עברית, תעתיק, אנגלית). כאן מוסיפים ומסירים שפות.
- **מיקום הנתונים** — איפה נשמרים השירים, סדרי האסיפה וערכות העיצוב (בדרך כלל `Documents\Solucast`). כדאי לבחור תיקייה
  שמגובה.

אחר כך **מדריך התחלה מהיר** קצר מציג את ששת הדברים שצריך לדעת. אפשר לפתוח אותו שוב בכל זמן מהתפריט שבתחתית הסרגל
השמאלי ← **מדריך התחלה מהיר**.

## 2. מסך השירות

כל מה שצריך לאסיפה נמצא במסך אחד:

| אזור | בשביל מה |
| --- | --- |
| **תצוגה מקדימה** (למעלה) | בדיוק מה שמוצג על מסכי האולם. מתחתיה: כפתורי השכבות (רקע, שקופית, שכבות־על, שמע, טיימר), **נקה הכל** ו**מסך שחור** |
| **אסיפה** (באמצע) | סדר האסיפה של היום — שירים, קריאות, סרטונים, הודעות |
| **ספרייה** (בצד) | שירים, תנ״ך, מדיה ומצגות, לכל אחד חיפוש משלו |
| **שקופיות** (למטה) | השקופיות של הפריט שנבחר באסיפה |
| **הסרגל** | **מסכים**, **במה והורים**, **מכשירים**, והתפריט שבתחתית (הגדרות, חשבון, עזרה) |

## 3. לפני האסיפה

**בוחרים מקרן.** לוחצים על **מסכים** בסרגל ובוחרים איזה מסך הוא המקרן. באותו חלון יש לשונית **ערכות עיצוב**: איך
נראים שירים, פסוקים, נקודות ומצגות על כל מסך.

**בונים את האסיפה.** מוצאים בספרייה שיר, פסוק או קובץ ו**לוחצים עליו פעמיים** (או גוררים) כדי להוסיף לאסיפה. לחיצה
על פריט באסיפה מציגה את השקופיות שלו. לחיצה ימנית על פריט פותחת עוד אפשרויות: פרטים, שינוי שם, רקע לשיר, לולאה,
הסרה.

**שירים.**
- השירים מגיעים ממאגר השירים של **solucast.app** ומתעדכנים לבד. שיר ששיניתם במחשב הזה נשמר כפי ששיניתם ומקבל סימן ענן;
  לחיצה על הסימן ← **שחזר את גרסת הענן** לוקחת את הגרסה מהמאגר.
- **+** יוצר שיר חדש. בעורך השיר כותבים את המילים בכל שפה, את **הסולם** ו**האקורדים** (בסוגריים מרובעים, למשל
  `[G]Amazing [C]grace`), ואת פרטי **זכויות יוצרים ו־CCLI**.
- **ייבוא** מביא שירים מ־OpenLP, ProPresenter, EasyWorship, ChordPro, OpenSong ומקובצי טקסט של CCLI SongSelect.

**התנ״ך.** מקלידים הפניה בחיפוש של לשונית התנ״ך — בעברית או באנגלית, למשל `יוחנן ג 16`, `תהילים 23-24` או
`John 3:16`. לחיצה על פסוק מציגה אותו; Shift ולחיצה מציגים כמה. כדי להוסיף תרגום, פותחים את רשימת התרגומים ובוחרים
**הוסיפו תרגום…** (מקובץ או מהאינטרנט).

**מדיה ומצגות.** תמונות וסרטונים עולים כרקע מאחורי המילים או לבד. קובצי PowerPoint ו־PDF הופכים למצגות שעוברים
בהן כמו בשיר.

## 4. בזמן האסיפה

- **הבא, ואז "הצג".** לחיצה כפולה על הפריט הבא באסיפה מסמנת אותו **הבא**. **הצג** מעלה אותו למסכים, והפריט שאחריו
  הופך לבא.
- **שקופיות של הפריט שעל המסך** עולות ב**לחיצה אחת** או ב**חיצים במקלדת**. זו הלחיצה שתעשו עשרות פעמים — והיא
  מיידית.
- **מסך שחור** (ליד **נקה הכל**, או המקש **B**) מחשיך את מסכי האולם ומשאיר את השקופית מתחת. לחיצה נוספת מחזירה
  מיד את אותן מילים. מסך הבמה של הלהקה והשידור לא מוחשכים.
- **נקה הכל** מוריד הכל מהמסכים: השקופית, הרקע, שכבות־העל והשמע. כפתורי השכבות מנקים שכבה אחת בכל פעם.
- **מקור / רב־לשוני** אפשר להחליף גם באמצע שיר (הגדרות ← כללי).
- **לולאה** (הודעות, ספירה לאחור, מוזיקה לפני האסיפה): לחיצה ימנית על פריט ← **לולאה…**. בזמן שהיא פועלת, בשורה
  שלה באסיפה מופיע תג עם הספירה לאחור, וגם הפס שמעל האסיפה מציג אותה, עם ✕ לעצירה. היא נעצרת מעצמה כשהפריט הראשון
  של האסיפה עולה למסך.
- **במה והורים** בסרגל: הודעה קצרה ל**במה** (רק הלהקה רואה אותה), או **קריאה להורה** — מספר הילד מופיע על מסכי
  האולם עד שמסירים אותו.

## 5. טלפונים ומכשירים אחרים

לוחצים על **מכשירים** בסרגל. בחלון יש לשוניות:

- **שלט מהטלפון** — סורקים את הקוד בטלפון או בטאבלט שלכם ומפעילים את האסיפה מכל מקום באולם: מה על המסך, הפריט
  הבא, כל השקופיות, סדר האסיפה והספרייה. פריט חדש מוכן בטלפון ועולה רק בלחיצה על **הצג על המסך**; שקופיות של השיר
  שכבר על המסך עולות בהקשה אחת. טלפונים באותה רשת Wi‑Fi מתחברים ישירות; כדי להתחבר גם דרך האינטרנט, מפעילים
  **טלפונים דרך האינטרנט** באותו חלון.
- **חדר חי** — המילים בטלפונים של הקהל, בכתובת `live.solucast.app` עם הקוד של הקהילה. כל אחד בוחר את השפה ואת תרגום
  התנ״ך שלו.
- **המסך של הלהקה** — קוד נפרד לנגנים: השקופית הנוכחית והבאה, ההודעה לבמה, הערות, אקורדים ושעון.

מתג הנעילה עוצר את כל הטלפונים בבת אחת.

## 6. שידור ופעוטון (NDI)

SoluCast יכולה לשלוח את התמונה כ־**NDI** ל־OBS, למחשב שידור או למסך בפעוטון. ב**מסכים** מוסיפים מסך ומפעילים
**NDI**. משדר שאין לו חלון משלו נשלח עם רקע שקוף, כך שב־OBS המילים מונחות מעל המצלמה.

**ב־OBS** (עם התוסף DistroAV / NDI): פותחים את המאפיינים של מקור ה־NDI וקובעים **Latency Mode ← Normal**. בשאר
המצבים OBS מוריד את השקיפות ומציג את המילים על שחור.

## 7. הגדרות ועזרה

הכפתור בתחתית הסרגל פותח תפריט: חשבון הקהילה (כניסה / יציאה), **הגדרות**, **מדריך התחלה מהיר**, **עזרה באתר**
(הדף הזה), **דיווח על בעיה** ו**בדקו עדכונים**.

- **הגדרות ← שירים** — הסנכרון עם מאגר השירים ו**דוח שימוש בשירים (CCLI)**: אילו שירים שרתם וכמה פעמים, לייצוא
  לדוח הרישיון.
- **דיווח על בעיה** שומר קובץ אבחון (בלי סיסמאות או מפתחות) ופותח דף שבו מתארים מה קרה ומצרפים אותו.

## 8. כשמשהו לא עובד

- **טלפון לא מתחבר ב־Wi‑Fi, או ש־OBS לא רואה את משדר ה־NDI.** כנראה חומת האש של Windows חוסמת את SoluCast. אם
  Windows מגדירה את הרשת **ציבורית**, הפכו אותה ל**פרטית** (הגדרות ← רשת ואינטרנט ← Wi‑Fi ← הרשת שלכם ← רשת פרטית), או
  אשרו את SoluCast ברשתות ציבוריות בחומת האש. SoluCast מציגה הודעה עם הכפתורים האלה כשהיא מזהה את זה.
- **ב־OBS המילים מופיעות על שחור.** קבעו את **Latency Mode** של מקור ה־NDI ל־**Normal** (ראו למעלה).
- **שיר לא מתעדכן מהמאגר.** הוא שונה במחשב הזה, ולכן נשמר כפי שהוא. לחיצה על סימן הענן שלו ← **שחזר את גרסת הענן**
  לוקחת את הגרסה מהמאגר.
- **התמונה על המסך הלא נכון.** פתחו את **מסכים** ובחרו שוב את המקרן. אם המקרן התנתק באמצע האסיפה, SoluCast מסתירה
  את החלון שלו ומחזירה אותו כשהמקרן חוזר.
- **כל דבר אחר** — **דיווח על בעיה** בתפריט, או
  [פתיחת דיווח כאן](https://github.com/shilo-maker/solucast-releases/issues/new).

</div>
