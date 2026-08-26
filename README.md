# VajbPet

Digitální karta pro tvého mazlíčka.

## Live aplikace

Po povolení GitHub Pages bude dostupná na: `https://adamrykl.github.io/vajbpet/`

## Co je hotové

- [x] Supabase projekt s databází
- [x] Webová aplikace (SPA)
- [x] GitHub repozitář s kódem

## Zbývá udělat (2 minuty)

### 1. Povolit GitHub Pages

1. Otevři [nastavení repozitáře](https://github.com/adamrykl/vajbpet/settings/pages)
2. U **Source** vyber **Deploy from a branch**
3. Vyber branch **main** a folder **/(root)**
4. Klikni **Save**
5. Počkej 1–2 minuty, pak bude aplikace živá na `https://adamrykl.github.io/vajbpet/`

### 2. Nastavit Supabase Auth

1. Otevři [Supabase Dashboard](https://supabase.com/dashboard/project/uvrdnpexejccykgfjabq)
2. Jdi do **Authentication → URL Configuration**
3. Do **Site URL** zadej: `https://adamrykl.github.io/vajbpet/`
4. Do **Redirect URLs** přidej:
   - `https://adamrykl.github.io/vajbpet/`
   - `https://adamrykl.github.io/vajbpet/?pet=*`
5. Ulož

### 3. Povolit emailové potvrzení (volitelné)

V **Authentication → Providers → Email** můžeš vypnout **Confirm email** pro jednodušší registraci, nebo nechat zapnuté a uživatelé potvrdí email.

## Funkce aplikace

- **Registrace/Přihlášení** přes email + heslo
- **Dashboard** se seznamem mazlíčků
- **Přidání mazlíčka** – jméno, druh, plemeno, barva, datum narození
- **Kontaktní údaje** – telefon, adresa (zobrazené po naskenování NFC)
- **Zdravotní údaje** – očkování, alergie, další informace
- **NFC odkaz** – unikátní URL pro každého mazlíčka, které nahraješ do čipu
- **Veřejná stránka** – zobrazí se komukoli po naskenování NFC
- **Režim ztraceného mazlíčka** – označení + zpráva pro nálezce
- **Nalezení mazlíčka** – formulář pro nálezce s možností kontaktovat majitele
- **Notifikace** – možnost zapnout/vypnout upozornění při naskenování (příprava pro budoucí implementaci)
- **Profil uživatele** – jméno, telefon, adresa

## Supabase projekt

- **Project URL:** https://uvrdnpexejccykgfjabq.supabase.co
- **Project ID:** `uvrdnpexejccykgfjabq`

## Technologie

- Frontend: Vanilla HTML/CSS/JS (SPA)
- Backend: Supabase (PostgreSQL + Auth + Row Level Security)
- Hosting: GitHub Pages
