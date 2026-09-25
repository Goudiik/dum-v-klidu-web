# Veřejné stránky aplikací Adivio

Statický web pro aplikace **Dům v klidu** a **Auto v klidu**. Neobsahuje analytiku, cookies, formuláře ani externí skripty.

## Adresy pro App Store Connect

| Aplikace | Privacy Policy URL | Support URL |
| --- | --- | --- |
| Dům v klidu | `https://adivio.cloud/dum-v-klidu/privacy/` | `https://adivio.cloud/dum-v-klidu/support/` |
| Auto v klidu | `https://adivio.cloud/auto-v-klidu/privacy/` | `https://adivio.cloud/auto-v-klidu/support/` |

Obě stránky zásad popisují ukládání dat, exporty, oprávnění, zálohy, smazání a kontakt. Obě stránky podpory uvádějí skutečný e-mailový kontakt. Texty Auto v klidu vycházejí z projektu `Auto v klidu/docs/PRIVACY_POLICY_CS.md`, `docs/SUPPORT_CS.md` a aktuálních funkcí aplikace. Funkce skenování a PDF výpisu jsou popsány podmíněně, protože se mohou lišit podle vydané verze.

## Jazykové verze a grafika

České adresy zůstávají stejné. Anglické stránky mají odpovídající cesty pod `/en/` včetně úvodu `/en/`. Každá stránka má viditelné přepnutí jazyka, správný atribut `lang`, kanonickou adresu a odkazy `hreflang` na obě verze. Překlad musí zůstat věcně shodný s českými zásadami.

Grafika v `assets/images/` obsahuje dvě ilustrativní fotografie vytvořené nástrojem OpenAI imagegen pro tento web a ikony převzaté z příslušných projektů aplikací. Fotografie nepředstavují obrazovky aplikací ani konkrétní majetek uživatele.

## Publikování a kontrola

Git remote tohoto adresáře je `https://github.com/Goudiik/dum-v-klidu-web.git` a větev `main`. Soubor `CNAME` nastavuje doménu `adivio.cloud`. Po nahrání stránek 25. září 2026 prošly kontroly GitHub Pages i Cloudflare Workers and Pages a nový obsah byl ověřen na živé doméně. Starší draft PR #1 z 12. září zůstává otevřený s již překonaným neúspěšným buildem a staršími texty Auto v klidu.

Před touto aktualizací živé zásady Domu v klidu stále obsahovaly staré tvrzení, že aplikace nepoužívá fotoaparát. Po každém dalším nasazení je nutné otevřít všech deset českých a anglických adres bez přihlášení a ověřit jejich aktuální obsah.

Před odesláním aplikací ke kontrole Applem je dále potřeba ověřit odkazy uvnitř obou aplikací a zadat tyto URL i pravdivé údaje App Privacy do App Store Connect. V projektu Auto v klidu zatím chybí konfigurační klíč `PrivacyPolicyURL`; vydání se skenerem bude vyžadovat také `NSCameraUsageDescription` a nový audit soukromí. Provozovatel má potvrdit znění o uchování e-mailů zaslaných podpoře.
