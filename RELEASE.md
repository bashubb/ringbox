# Ringbox: release checklist

Stan na 17.10.2026. Strona gotowa (bashubb.com/ringbox/), film motion graphics (16:9 i 9:16), privacy i support w nowym stylu, karta podglądu linku zrobiona.

## Do potwierdzenia z aplikacją
- [ ] Cennik: Free (nielimitowane alarmy + 1 własny dźwięk) i **Ringbox Plus** „yearly or once”. Strona nie podaje kwot („price for your country in the app”). Zgadza się z wersją do review?
- [ ] Privacy „Last updated: October 13, 2026”: RevenueCat, subskrypcja roczna / dożywotnia, AlarmKit, widżety. Aktualne?
- [ ] Support: nazwy funkcji (Record & time / Quick timer, widżety Next alarm i Record & time, kontrolki Control Center, Action button). Aktualne?
- [ ] Fakty na stronie: 1:30 nagrania, 29 s dźwięku alarmu, Silent Mode i Focus. Aktualne?
- [ ] Film: jeśli zmieniły się nazwy funkcji, przerenderować (źródło: `PromoVideos/Ringbox/film/`, `render.js` + `blend.py`, ok. 26 s).

## Na stronie (wszystko w `docs/`)
- [ ] Link do App Store: podmień `https://apps.apple.com/us/search?term=…` na adres aplikacji (`…/app/idXXXXXXXXXX`) we wszystkich `data-store-link` (index, privacy, support).
- [ ] `<html data-store="soon">` → `"live"` w `index.html`. Jednym ruchem zamienia „Coming soon” na odznakę App Store w pasku, hero, stopce.
- [ ] Baner Safari: `<meta name="apple-itunes-app" content="app-id=XXXXXXXXXX">` w `<head>` strony głównej.
- [ ] JSON-LD `SoftwareApplication`: dodać/poprawić `offers` (cena lub usunąć) i link do App Store.
- [ ] Podbić `?v=` przy zmienionym CSS/JS, wypchnąć, sprawdzić na żywo: desktop, telefon pionowo, telefon poziomo.
- [ ] Odpalić `fit-audit.js` (desktop) i `phone-audit.js` (telefony) ze skilla `bashubb-app-sites` → „ALL … FIT”.

## bashubb.com (repo `Bashubb`)
- [ ] Przenieść kartę Ringbox z sekcji **Coming soon** do **Available now**, dodać odznakę App Store z linkiem.
- [ ] Dodać Ringbox do JSON-LD (`@graph`, jak Shrink) i do `sitemap.xml`.

## App Store Connect
- [ ] Privacy Policy URL: `https://bashubb.com/ringbox/privacy/`
- [ ] Support URL: `https://bashubb.com/ringbox/support/`
- [ ] Marketing URL: `https://bashubb.com/ringbox/`
