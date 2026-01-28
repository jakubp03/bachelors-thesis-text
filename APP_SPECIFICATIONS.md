# Test Management Application - Základní Specifikace

## Cíl

Navrhnout a vytvořit Full-stack webovou aplikaci pro tvorbu, správu a absolvování testů s pokročilými funkcemi pro sledování pokroku a sdílení. Inspirováno Moodle testy.

---

## Hlavní Funkce

### 1. **Autentizace a Správa Uživatelů**

- Registrace
- Přihlášení/Odhlášení

### 2. **Tvorba Testů**

- **Základní informace testu:**
    - Název a popis
    - Kategorie/tagy
    - Časový limit (volitelný)
    - Hodnocení (bodování, procenta)
- **Typy otázek:**
    - Jednoduchá volba (radio buttons)
    - Vícenásobná volba (checkboxes)
    - Textová odpověď (krátká/dlouhá)
    - Pravda/Nepravda
    - Párování (matching)
    - Uspořádání (ordering)
    - Flashcard
- **Multimediální obsah:**
    - Přidávání obrázků k otázkám
- **Správa otázek:**
    - Drag & drop přeuspořádání
    - Duplikování otázek
    - Banka otázek pro opakované použití
    - Bodování jednotlivých otázek

### 3. **Absolvování Testů**

- Průvodce testem (progress bar)
- Ukládání rozpracovaného testu
- Časovač s upozorněním
- Navigace mezi otázkami
- Okamžité vyhodnocení po odeslání
- Zobrazení správných odpovědí (volitelné)

### 4. **Statistiky a Analytics**

- **Pro absolventa:**
    - Historie pokusů
    - Grafické zobrazení pokroku v čase
    - Průměrné skóre
    - Čas strávený na testu
- **Pro autora testu:**
    - Počet absolvování
    - Průměrné skóre všech uživatelů
    - Nejčastěji chybné otázky
    - Časová analýza
    - výsledky jednotlivých uživatelů

### 5. **Sdílení a Spolupráce**

- **Možnosti sdílení:**
    - Veřejný odkaz (kdokoliv s odkazem)
- **Anonymní režim:**
    - Absolvování bez registrace
    - Omezené funkce (bez historie)
    - Volitelné zadání jména/nicku

---

## User Stories

### Epic 1: Registrace a Autentizace

**US-1.1:** Jako nový uživatel chci se zaregistrovat, abych mohl vytvářet a ukládat své testy.

**US-1.2:** Jako registrovaný uživatel chci se přihlásit, abych měl přístup ke svým testům.

---

### Epic 2: Tvorba Testů

**US-2.1:** Jako uživatel chci vytvořit nový test se základními informacemi.

**US-2.2:** Jako autor testu chci přidat otázku s jednou správnou odpovědí.

**US-2.3:** Jako autor testu chci přidat otázku s více správnými odpověďmi.

**US-2.4:** Jako autor testu chci přidat textovou otázku.

**US-2.5:** Jako autor testu chci přidat obrázek k otázce.

**US-2.6:** Jako autor testu chci uspořádat otázky drag & drop.

---

### Epic 3: Absolvování Testů

**US-3.1:** Jako uživatel chci spustit test a vidět první otázku.

**US-3.2:** Jako absolvující chci navigovat mezi otázkami.

**US-3.3:** Jako absolvující chci označit otázku k pozdějšímu přezkoumání.

**US-3.5:** Jako absolvující chci uložit rozpracovaný test a pokračovat později.

**US-3.6:** Jako absolvující chci odeslat test a vidět výsledky.

**US-3.7:** Jako absolvující chci vidět správné odpovědi po dokončení.

---

### Epic 4: Statistiky a Analytics

**US-4.1:** Jako uživatel chci vidět historii všech mých pokusů.

**US-4.2:** Jako uživatel chci vidět svůj pokrok v čase.

**US-4.4:** Jako autor testu chci vidět přehled všech absolvování.

---

### Epic 5: Sdílení a Spolupráce

**US-5.1:** Jako autor testu chci sdílet test veřejným odkazem.

**US-5.5:** Jako anonymní uživatel chci absolvovat sdílený test bez registrace.

**US-5.6:** Jako autor testu chci vidět kdo můj test absolvoval.

---

### Epic 6: Pokročilé Funkce

**US-6.3:** Jako autor testu chci importovat test z Moodle.

**US-6.5:** Jako uživatel chci vidět žebříček nejlepších.

---

## UI/UX Wireframe Návrhy

**Hlavní Stránky:**

1. Dashboard (přehled testů)
2. Tvorba testu (editor)
3. Absolvování testu (clean, focused view)
4. Výsledky (s grafickými prvky)
5. Statistiky (charts & graphs)
6. Profil uživatele

---

## Tech Stack

**Frontend: React**

**Backend: Spring Boot**

**Database: MySQL**

---