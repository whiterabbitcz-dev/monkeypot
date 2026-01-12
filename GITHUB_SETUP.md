# 🚀 Jak dostat web na internet - Kompletní návod

## Krok 1: Vytvořte GitHub účet (pokud nemáte)

1. Jděte na **[github.com/signup](https://github.com/signup)**
2. Zaregistrujte se (email, heslo, username)
3. Ověřte email
4. ✅ Máte účet!

---

## Krok 2: Vytvořte nový repozitář

1. Jděte na **[github.com/new](https://github.com/new)**
   - Nebo klikněte na "+" v pravém horním rohu → "New repository"

2. Vyplňte formulář:
   ```
   Repository name: monkeypot
   Description: Prezentační web pro keramický ateliér Monkey Pot
   Public: ✅ (zatrhněte)
   
   ❌ NEZATRHÁVEJTE:
   - Add a README file
   - Add .gitignore
   - Choose a license
   ```

3. Klikněte **"Create repository"**

---

## Krok 3: Připojte lokální projekt na GitHub

Po vytvoření repozitáře uvidíte stránku s instrukcemi. GitHub vám ukáže něco jako:

```bash
git remote add origin https://github.com/USERNAME/monkeypot.git
git branch -M main
git push -u origin main
```

**SPUSŤTE TYTO PŘÍKAZY:**

```bash
cd /Users/martinsvoboda/Desktop/monkeypot_2

# Nahraďte USERNAME svým GitHub username!
git remote add origin https://github.com/USERNAME/monkeypot.git

git branch -M main

git push -u origin main
```

Systém vás vyzve k přihlášení:
- **Username**: váš GitHub username
- **Password**: použijte **Personal Access Token** (ne heslo!)

### 🔑 Jak získat Personal Access Token:

1. Jděte na: **[github.com/settings/tokens](https://github.com/settings/tokens)**
2. Klikněte **"Generate new token"** → "Generate new token (classic)"
3. Nastavte:
   - Note: "Monkey Pot Web"
   - Expiration: 90 days
   - Zatrhněte: ✅ **repo** (všechna práva)
4. Klikněte **"Generate token"**
5. **ZKOPÍRUJTE TOKEN** (už ho neuvidíte!)
6. Použijte ho jako heslo při `git push`

---

## Krok 4: Aktivujte GitHub Pages

1. Jděte do vašeho repozitáře na GitHubu
2. Klikněte na **"Settings"** (nastavení)
3. V levém menu najděte **"Pages"**
4. V sekci "Build and deployment":
   - **Source**: Deploy from a branch
   - **Branch**: main
   - **Folder**: / (root)
5. Klikněte **"Save"**

---

## Krok 5: Web je živý! 🎉

Za 1-2 minuty bude web dostupný na:

```
https://USERNAME.github.io/monkeypot/
```

GitHub vám přesnou URL ukáže nahoře na stránce Settings → Pages.

---

## 🆘 Pomoc při problémech

### Push nefunguje?
- Zkontrolujte, že používáte Personal Access Token (ne heslo)
- Zkontrolujte, že jste nahradili USERNAME svým skutečným jménem

### Web není dostupný?
- Počkejte 2-3 minuty
- Zkontrolujte, že repozitář je **Public**
- Zkuste hard refresh (Cmd+Shift+R)

### Další problémy?
- Napište mi a pomůžu!

---

## 📝 Rychlý checklist

- [ ] Mám GitHub účet
- [ ] Vytvořil jsem repozitář (Public)
- [ ] Spustil jsem git push
- [ ] Aktivoval jsem GitHub Pages v Settings
- [ ] Počkal jsem 2 minuty
- [ ] ✅ Web běží na internetu!
