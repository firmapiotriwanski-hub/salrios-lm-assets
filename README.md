# SalriOS — Lead Magnet Assets

Hosting grafik wykorzystywanych w PDF-ach Lead Magnetów (Gamma API), grafikach LinkedIn/Instagram, landing pages SalriOS.

**Owner:** Piotr Iwański (firma.piotr.iwanski@gmail.com)
**Use case:** publiczny URL z rozszerzeniem `.png/.jpg/.webp` dla Gamma API (`developers.gamma.app/guides/image-url-best-practices`)

## URL pattern

```
https://raw.githubusercontent.com/firmapiotriwanski-hub/salrios-lm-assets/main/[spoke]/[file].png
```

✅ HTTPS · ✅ `.png` extension · ✅ public · ✅ permanent · ✅ free

## Struktura

```
salrios-lm-assets/
├── proces/         # SPOKE 1 PROCES (8 slajdów Lead Magnet)
├── follow-up/      # SPOKE 2 FOLLOW-UP
├── asystent/       # SPOKE 3 ASYSTENT (Morpheus piasta)
└── _shared/        # grafiki wspólne (logo, brand, Morpheus elements)
```

## Konwencja nazw

`slajd_[01-08]_[temat].png` — np. `slajd_04_proces1_followup.png`

**Wersjonowanie:** jeśli zmieniasz CONTENT pod tą samą nazwą, dodaj suffix `_v2`, `_v3` (CDN cache 30 dni).

## Workflow regularny

```bash
# 1. Wrzuć grafiki do odpowiedniego folderu
cp ~/Downloads/slajd_*.png ~/salrios-lm-assets/proces/

# 2. Push do GitHub (URL aktywny w ~30 sek)
cd ~/salrios-lm-assets
git add .
git commit -m "proces: 8 slajdów Lead Magnet"
git push

# 3. URL gotowy dla Gamma API:
# https://raw.githubusercontent.com/firmapiotriwanski-hub/salrios-lm-assets/main/proces/slajd_01_cover.png
```

## Linki referencyjne

- **Brand guide:** `core a-team/SALRIOS_BRAND_GUIDE_v1_1.md`
- **Character sheet "Właściciel":** `core a-team/CHARACTER_SHEET_WLASCICIEL.md`
- **Workflow Murdock+Gamma:** `Marketing/leadmagnety/_infrastruktura/BRIEF_MARKETINGCTO_LM_ASSETS_HOSTING.md`
- **Gamma API:** https://developers.gamma.app/guides/image-url-best-practices

---

🚐 *A-Team SalriOS*
