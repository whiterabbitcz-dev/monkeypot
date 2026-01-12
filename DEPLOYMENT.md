# 🚀 Návod na nasazení na GitHub Pages

## Rychlý start

### 1. Inicializace Git repozitáře

```bash
# Přejděte do složky projektu
cd /Users/martinsvoboda/Desktop/monkeypot_2

# Inicializujte git
git init

# Přidejte všechny soubory
git add .

# Proveďte první commit
git commit -m "Initial commit - Monkey Pot website"
```

### 2. Vytvoření GitHub repozitáře

1. Jděte na [GitHub.com](https://github.com)
2. Klikněte na "New repository" (zelené tlačítko)
3. Vyplňte:
   - Repository name: např. `monkeypot` nebo `monkeypot-website`
   - Description: "Prezentační web pro keramický ateliér Monkey Pot"
   - Visibility: Public (nutné pro GitHub Pages zdarma)
   - **NEVYTVÁŘEJTE** README, .gitignore nebo licenci (už je máte)
4. Klikněte "Create repository"

### 3. Propojení s GitHub

```bash
# Přidejte vzdálený repozitář (nahraďte USERNAME a REPO-NAME)
git remote add origin https://github.com/USERNAME/REPO-NAME.git

# Přejmenujte větev na main
git branch -M main

# Nahrajte kód na GitHub
git push -u origin main
```

### 4. Aktivace GitHub Pages

1. Na GitHubu jděte do vašeho repozitáře
2. Klikněte na **Settings** (nastavení)
3. V levém menu vyberte **Pages**
4. V sekci "Build and deployment":
   - **Source**: Deploy from a branch
   - **Branch**: main
   - **Folder**: / (root)
5. Klikněte **Save**

### 5. Hotovo! 🎉

Za 1-2 minuty bude web dostupný na adrese:
```
https://USERNAME.github.io/REPO-NAME/
```

GitHub vám zobrazí přesnou adresu nahoře na stránce Settings → Pages.

---

## Aktualizace webu

Když provedete změny v kódu:

```bash
# Přidejte změněné soubory
git add .

# Vytvořte commit s popisem změn
git commit -m "Popis změn"

# Nahrajte na GitHub
git push
```

Web se automaticky aktualizuje do 1-2 minut.

---

## Vlastní doména (volitelné)

Pokud chcete použít vlastní doménu (např. `monkeypot.cz`):

1. V nastavení GitHub Pages zadejte vaši doménu do pole "Custom domain"
2. V DNS nastavení vaší domény přidejte:
   - Pro apex doménu (monkeypot.cz):
     ```
     A záznam → 185.199.108.153
     A záznam → 185.199.109.153
     A záznam → 185.199.110.153
     A záznam → 185.199.111.153
     ```
   - Pro subdoménu (www.monkeypot.cz):
     ```
     CNAME → USERNAME.github.io
     ```

Více info: [GitHub Docs - Custom domains](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

---

## Řešení problémů

### Web není dostupný
- Zkontrolujte, že repozitář je **Public**
- Počkejte 2-3 minuty po aktivaci Pages
- Zkuste hard refresh (Cmd+Shift+R / Ctrl+Shift+R)

### Styly nefungují
- Zkontrolujte cesty k CSS souborům v HTML
- Měly by být relativní: `css/style.css` (ne `/css/style.css`)

### 404 chyba
- Zkontrolujte, že hlavní stránka se jmenuje `index.html`
- Ujistěte se, že všechny soubory byly nahrány (git push)

---

## Kontakt

Pro otázky nebo pomoc pište na martinsvoboda@example.com
