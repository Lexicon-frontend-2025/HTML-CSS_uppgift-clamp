# 🧪 Övning: Responsiv design med `clamp()`

## 🎯 Mål
Att förstå och använda CSS-funktionen `clamp()` för att skapa responsiva egenskaper som skalar beroende på skärmens storlek – särskilt **textstorlek** och **spacing**.

 
## 🧠 Tips
* Syntax:
  * ```clamp(min-värde, idealvärde, max-värde)```

* Kombinera t.ex. ```rem``` och ```vw``` i mittenvärdet för bästa resultat.

* ```vw``` = 1% av viewportens bredd.

* Använd devtools för att testa olika skärmstorlekar!

---

## 📄 Instruktioner

1. **Skapa en ny HTML-fil** med följande innehåll:

```html
<!DOCTYPE html>
<html lang="sv">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Clamp-övning</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <h1>Välkommen till Clamp-land</h1>
    <p>Denna text ändrar storlek beroende på skärmens bredd.</p>
  </header>
  <main>
    <section>
      <h2>Responsiv sektion</h2>
      <p>Testa att ändra storleken på fönstret och se hur text och padding förändras.</p>
    </section>
  </main>
</body>
</html>
```

2. **Skapa en CSS-fil (style.css)** med grundläggande layout och lägg till egna ```clamp()```-uttryck enligt instruktionerna nedan:
## 🎨 CSS-uppgifter
* Ange en textstorlek för ```h1``` som:
  * Aldrig blir mindre än ```2rem```

  * Idealt baseras på viewportens bredd (t.ex. ```vw```)

  * Aldrig blir större än ```4rem```

* Ange en textstorlek för ```h2``` som:

  * Minimum ```1.5rem```

  * Max ```2.5rem```

  * Med en flexibel mittpunkt

* Lägg till padding på ```<body>``` med ```clamp()```:

  * Minst ```1rem```, max ```3rem```, skala med viewportbredd

* Lägg till padding på ```<section>```:

  * Använd ```clamp()``` för att skala mellan exempelvis ```1rem``` och ```2rem```
 
## 🪭 Extra
  #### Miniövning: `min()`, `max()` och `minmax()`

## 📄 Instruktioner

### ✅ Uppgift 1 – `min()` och `max()`

1. Skapa en `<div>` med klassen `box` i din HTML:

```html
<div class="box">
  <p>Jag har responsiv bredd och höjd!</p>
</div>
```

Lägg till CSS så att:

* Bredden blir 100% av föräldern, men aldrig större än ```600px``` (använd ```min()``` eller ```max()```)

* Höjden blir minst ```200px```, men växer vid behov (t.ex. vid mycket innehåll)

💡 Tips: Använd width: ```min(...);``` eller ```max(...)```, och ```min-height: ...```

### ✅ Uppgift 2 – minmax() med CSS Grid
1. Lägg till en container med flera barn:

```html
<div class="grid">
  <div>1</div>
  <div>2</div>
  <div>3</div>
</div>
```
2. I CSS:

* Använd CSS Grid och skapa 3 kolumner

* Kolumnerna ska vara minst 150px breda men fylla resten jämnt om plats finns

💡 Tips: Använd grid-template-columns: repeat(3, minmax(...));

📚 Läs mer
* [MDN – ```min()```](https://developer.mozilla.org/en-US/docs/Web/CSS/min)

* [MDN – ```max()```](https://developer.mozilla.org/en-US/docs/Web/CSS/max)

* [MDN – ```minmax()```](https://developer.mozilla.org/en-US/docs/Web/CSS/minmax)

---

