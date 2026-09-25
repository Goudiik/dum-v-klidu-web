# Veřejné stránky aplikací Adivio

Statický web pro aplikace **Dům v klidu** a **Auto v klidu**. Neobsahuje analytiku, cookies, formuláře ani externí skripty.

## Adresy pro App Store Connect

| Aplikace | Privacy Policy URL | Support URL |
| --- | --- | --- |
| Dům v klidu | `https://adivio.cloud/dum-v-klidu/privacy/` | `https://adivio.cloud/dum-v-klidu/support/` |
| Auto v klidu | `https://adivio.cloud/auto-v-klidu/privacy/` | `https://adivio.cloud/auto-v-klidu/support/` |

Obě stránky zásad popisují ukládání dat, exporty, oprávnění, zálohy, smazání a kontakt. Obě stránky podpory uvádějí skutečný e-mailový kontakt. Texty Auto v klidu vycházejí z projektu `Auto v klidu/docs/PRIVACY_POLICY_CS.md`, `docs/SUPPORT_CS.md` a aktuálních funkcí aplikace. Funkce skenování a PDF výpisu jsou popsány podmíněně, protože se mohou lišit podle vydané verze.

## Publikování a kontrola

Git remote tohoto adresáře je `https://github.com/Goudiik/dum-v-klidu-web.git` a větev `main`. Soubor `CNAME` nastavuje doménu `adivio.cloud`. Otevřený draft PR #1 z 12. září pro Auto v klidu ukazuje integraci Cloudflare Workers and Pages a neúspěšný build. Starší README v `main` uvádí GitHub Pages; skutečné produkční napojení a chybu buildu je nutné ověřit v Cloudflare.

Před touto aktualizací živé zásady Domu v klidu stále obsahovaly staré tvrzení, že aplikace nepoužívá fotoaparát. Po každém nasazení je nutné otevřít všechna čtyři URL bez přihlášení a ověřit jejich aktuální obsah.

Před odesláním aplikací ke kontrole Applem je dále potřeba ověřit odkazy uvnitř obou aplikací a zadat tyto URL i pravdivé údaje App Privacy do App Store Connect. V projektu Auto v klidu zatím chybí konfigurační klíč `PrivacyPolicyURL`; vydání se skenerem bude vyžadovat také `NSCameraUsageDescription` a nový audit soukromí. Provozovatel má potvrdit znění o uchování e-mailů zaslaných podpoře.
