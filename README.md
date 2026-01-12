# Monkey Pot - Keramika na Letné

Prezentační webové stránky pro keramický ateliér Monkey Pot v Praze 7.

## 🎨 O projektu

Tento web je prezentace pro keramický ateliér Monkey Pot, kde Martin Minks vytváří užitkovou keramiku a pořádá kurzy točení.

### Hlavní sekce webu:
- **Domů** - Úvodní stránka s přehledem služeb
- **O mně** - Představení Martina a ateliéru
- **Kurzy** - Informace o kurzech točení keramiky
- **E-shop** - Přehled produktů z ateliéru
- **Spolupráce** - B2B nabídka pro gastro provozy
- **Kontakt** - Kontaktní informace a formulář

## 🚀 Nasazení na GitHub Pages

1. Vytvořte nový repozitář na GitHubu
2. Nahrajte všechny soubory do repozitáře:
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/VASE_JMENO/NAZEV_REPO.git
git push -u origin main
```

3. V nastavení repozitáře (Settings → Pages) nastavte:
   - Source: Deploy from a branch
   - Branch: main
   - Folder: / (root)

4. Web bude dostupný na: `https://VASE_JMENO.github.io/NAZEV_REPO/`

## 📁 Struktura projektu

```
monkeypot_2/
├── index.html          # Hlavní stránka
├── o-mne.html         # O mně
├── kurzy.html         # Kurzy
├── shop.html          # E-shop
├── spoluprace.html    # Spolupráce
├── kontakt.html       # Kontakt
├── css/
│   └── style.css      # Styling
├── js/
│   └── main.js        # JavaScript
├── images/            # Složka pro obrázky (zatím prázdná)
└── README.md          # Tento soubor
```

## 🎨 Design

Web je inspirován elegantním keramickým designem s čistou typografií a minimalistickým přístupem:

- **Fonty**: Cormorant Garamond (nadpisy) a Montserrat (text)
- **Barevná paleta**: 
  - Primární: #8B7355 (teplá hnědá)
  - Sekundární: #D4C5B9 (světle béžová)
  - Pozadí: #FAF8F6 (krémová)

## 📝 Poznámky

- **Obrázky**: Aktuálně jsou použity placeholdery. Nahraďte je skutečnými fotografiemi z ateliéru.
- **Kontaktní údaje**: V kontaktní stránce doplňte skutečné telefonní číslo a e-mail.
- **Formulář**: Kontaktní formulář zatím není funkční - slouží pouze k prezentaci.
- **E-shop**: Pro funkční e-shop bude potřeba implementovat platební bránu nebo propojení s externí službou.

## 🔧 Další kroky

1. **Přidat skutečné fotografie** do složky `images/` a aktualizovat odkazy v HTML
2. **Doplnit kontaktní údaje** (telefon, e-mail)
3. **Implementovat funkční formulář** (např. pomocí Formspree, Netlify Forms, nebo vlastního backendu)
4. **Přidat Google Maps** na kontaktní stránku
5. **Implementovat e-shop funkcionalitu** (košík, platební brána)
6. **SEO optimalizace** (meta tagy, Open Graph, strukturovaná data)
7. **Google Analytics** pro sledování návštěvnosti

## 📱 Responzivita

Web je plně responzivní a funguje na:
- Desktop (1920px+)
- Laptop (1366px - 1920px)
- Tablet (768px - 1366px)
- Mobile (320px - 768px)

## 📄 Licence

© 2026 Monkey Pot. Všechna práva vyhrazena.

---

**Vytvořeno pro prezentační účely**
