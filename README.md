# 🧪 Övning: Responsiv design med `clamp()`

## 🎯 Mål
Att förstå och använda CSS-funktionen `clamp()` för att skapa responsiva egenskaper som skalar beroende på skärmens storlek – särskilt **textstorlek** och **spacing**.

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
🎨 CSS-uppgifter
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
