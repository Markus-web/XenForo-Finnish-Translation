# XenForo suomeksi | XenForo Finnish Translation

Täysin suomenkielinen kielipaketti [XenForo](https://xenforo.com/)-foorumialustalle. Paketti on tarkoitettu itse ylläpidettäville sivustoille: tuonnin jälkeen hallinta ja julkinen käyttöliittymä toimivat suomeksi. Mukana on XenForo-ydin sekä käännöksiä suosituille lisäosille ja tyyleille.

- **Testattu:** XenForo **2.3.12** (`base_version_id` 2031270)
- **Fraaseja:** noin 19 700
- **Kieli:** Finnish (FI), `fi-FI`, UTF-8 ilman BOM:ia
- **Lisenssi:** [MIT](LICENSE)

## Julkaisut

- **[Viimeisin julkaisu](https://github.com/Markus-web/XenForo-Finnish-Translation/releases/latest)** — suositeltu asennustiedosto
- **[Kehitysversio (main)](https://github.com/Markus-web/XenForo-Finnish-Translation/blob/main/language-Finnish-(FI).xml)** — suora XML-tiedosto haarasta `main`

Julkaisun liitetiedosto on nimeltään **`language-Finnish-FI.xml`** (GitHub poistaa sulkeet tiedostonimestä). Repositoriossa tiedosto on `language-Finnish-(FI).xml`. Sisältö on sama.

## Vaatimukset

- **XenForo 2.3.12** suositeltu (2.3.x toimii; 2.2.x mahdollinen, osa fraaseista voi puuttua tai olla ylimääräisiä)
- **PHP 8.0.2+** (XenForo 2.3:n vaatimus)
- **`upload_max_filesize` ja `post_max_size` vähintään 5M** (tiedosto on noin 3,5 MB)
- Hallintapaneelin oikeus kielten tuontiin

## Asennus

1. Lataa `language-Finnish-FI.xml` [viimeisimmästä julkaisusta](https://github.com/Markus-web/XenForo-Finnish-Translation/releases/latest) tai `language-Finnish-(FI).xml` tästä repositoriosta.
2. Avaa XenForon hallinta: `https://esimerkki.fi/admin.php`.
3. **Appearance** → **Languages** → **Import**.
4. Valitse tiedosto ja tuo se.
5. Aseta kieli **Finnish (FI)** oletukseksi (Options → Setup / user defaults) ja/tai käyttäjän valittavaksi.

**Huom:**

- Virhe `Please upload a valid language XML file` tarkoittaa yleensä PHP:n latausrajaa. Nosta `upload_max_filesize` ja `post_max_size` vähintään 5M:iin ja käynnistä PHP-FPM / palvelin uudelleen.
- Varmuuskopioi nykyinen kielipaketti ennen tuontia (Languages → Export).
- Päivityksessä valitse **Overwrite language**.

## Päivittäminen

1. Lataa uusin XML julkaisuista.
2. **Appearance** → **Languages** → valitse **Finnish (FI)** → **Import** → tiedosto + **Overwrite language**.
3. Tyhjennä välimuisti tarvittaessa: **Tools** → **Rebuild caches** (tai Development → Clear caches, jos kehitystila on päällä).

Fraasit, joita et ole muokannut hallinnassa, korvautuvat paketilla. Omat muokkaukset kannattaa merkitä tai viedä talteen ennen ylikirjoitusta.

## Tekijänoikeusrivi (`extra_copyright`)

Paketti lisää alatunnisteeseen fraasin `extra_copyright` (linkki: XenForo-sivuston suomenkielinen lokalisointi, Markus Media). Voit tyhjentää tai muuttaa sen:

1. **Appearance** → **Languages** → **Finnish (FI)** → **Phrases**
2. Hae `extra_copyright`
3. Tyhjennä sisältö tai vaihda oma teksti

Sama fraasi on XML-tiedostossa; voit poistaa sen myös ennen tuontia.

## Käännösfraasit (ylläpitäjille)

- Säilytä paikkamerkit ennallaan: `{username}`, `{board}`, `{date}`, `{title}`, `{count}` jne.
- Säilytä printf-muodot (`%d`, `%s`, `%1$s`) sekä HTML- ja BB-koodirakenne.
- Älä lisää tai poista tägejä (`<a>`, `<strong>`, `<br />`) ellei alkuperäinen fraasi niitä käytä.
- Vältä ylimääräisiä välilyöntejä alussa ja lopussa.

## Vianmääritys

| Oire | Toimenpide |
|------|------------|
| `Please upload a valid language XML file` | Nosta PHP `upload_max_filesize` ja `post_max_size` (≥ 5M). |
| Ääkköset rikki | Tiedosto UTF-8 ilman BOM:ia; älä tallenna ANSI/Latin-1:nä. |
| Osa käyttöliittymästä englanniksi | Ylikirjoittava tuonti; tyhjennä XF-välimuisti; tarkista että käyttäjän kieli on Finnish (FI). |
| Lisäosan fraasit englanniksi | Lisäosa ei ole tässä paketissa tai sen `addon_id` on eri. Avaa issue ja kerro lisäosan tunnus. |
| Rikkoutunut sivupohja sähköpostissa / HTML-fraasissa | Palauta fraasi XML:stä; tarkista ettei HTML-rakenne ole muuttunut. |

## Mukana olevat lisäosat ja tyylit

Paketti sisältää suomennoksia seuraaville (ei-tyhjentävä lista; ydin XenForo on aina mukana). Käyttämättömien lisäosien fraasit eivät haittaa: XenForo näyttää ne vain, jos lisäosa on asennettu.

**ThemeHouse**

- [UI.X 2](https://www.themehouse.com/xenforo/2/themes/ui-x) — teema ja lisäosa
- [Connected Account Providers](https://www.themehouse.com/xenforo/2/addons/connected-account-providers)
- [Donate](https://www.themehouse.com/xenforo/2/addons/donate)
- [Holidays](https://www.themehouse.com/xenforo/2/addons/holidays)
- [User Criteria Extended](https://www.themehouse.com/xenforo/2/addons/user-criteria-extended)
- [Install & Upgrade](https://www.themehouse.com/xenforo/2/addons/install-and-upgrade)
- [Username Color](https://www.themehouse.com/xenforo/2/addons/username-color)

**Siropu**

- [Chat](https://siropu.com/products/chat/)
- [Ads Manager Lite](https://siropu.com/products/ads-manager-2-lite/)

**XF2 Addons (AndyB)**

- [Email log](https://www.xf2addons.com/resources/email-log.97/)
- [Forum statistics plus](https://www.xf2addons.com/resources/forum-statistics-plus.101/)
- [History](https://www.xf2addons.com/resources/history.54/)
- [Most posts](https://www.xf2addons.com/resources/most-posts.46/)
- [Weekly newsletter](https://www.xf2addons.com/resources/weekly-newsletter.584/)
- [Similar threads](https://www.xf2addons.com/resources/similar-threads.17/)
- [Trader](https://www.xf2addons.com/resources/trader.55/)
- [Calendar](https://www.xf2addons.com/resources/calendar.696/)
- [Members recently online](https://www.xf2addons.com/resources/members-recently-online.51/)
- [Direct message search plus](https://www.xf2addons.com/resources/direct-message-search-plus.809/)
- [Auto close](https://www.xf2addons.com/resources/auto-close.80/)
- [Logo email](https://www.xf2addons.com/resources/logo-email.593/) (logo onnistuu myös tyylin `MAIL_CONTAINER`-pohjalla ilman lisäosaa)

**Xon / SV**

- [Attachment Improvements](https://xenforo.com/community/resources/attachment-improvements-by-xon.6629/)
- [Search Improvements](https://xenforo.com/community/resources/search-improvements.6838/)
- [Standard Library](https://xenforo.com/community/resources/standard-library-by-xon.7915/)
- [Alert Improvements](https://xenforo.com/community/resources/alert-improvements-by-xon.6203/)
- [User Mentions Improvements](https://xenforo.com/community/resources/user-mentions-improvements-by-xon.6147/)
- [Word Count Search](https://xenforo.com/community/resources/word-count-search.5690/)

**Muut**

- [s9e/MediaSites](https://xenforo.com/community/resources/s9e-media-sites.5973/)
- [App for Cloudflare](https://xenforo.com/community/resources/digitalpoint-app-for-cloudflare-r.8750/)
- [Known Bots](https://xenforo.com/community/resources/known-bots.6546/) (Hampel)
- [What's New Tweak](https://xenforo.com/community/resources/whats-new-tweak.6809/) (MrJinx)
- [XenForo Enhanced Search](https://xenforo.com/docs/xf2/enhanced-search/) (XFES)
- [Password Tools](https://xenforo.com/community/resources/kl-password-tools.5703/) (KL)
- [Change Content Owner](https://xenforo.com/community/resources/change-content-owner.5574/) (TickTackk)
- [Conversation Button](https://xenforo.com/community/resources/conversation-button.5570/) (BassMan)
- [Widget Framework / EWRporta2](https://xenforo.com/community/resources/widget-framework-2-ewrporta.5791/)

Paketissa on myös vanhempia tai harvinaisempia lisäosafraaseja (esim. vanhat XF1-jäänteet). Ne voi jättää paikalleen.

## Käännöstyyli

- Luonnollinen yleiskieli. Vakiintunut suomenkielinen termi ensin, anglismi vain jos se on alan vakiosana (OAuth, webhook).
- Johdonmukaiset termit: thread = ketju, post = viesti, attachment = liite, tag = tunniste, reaction = reaktio, prefix = etuliite.
- Lyhyet UI-tekstit; älä toista samaa asiaa kahteen kertaan.

## Osallistuminen

- Ilmoita virheestä: [uusi issue](https://github.com/Markus-web/XenForo-Finnish-Translation/issues/new/choose)
- Lähetä korjaus: [pull request](https://github.com/Markus-web/XenForo-Finnish-Translation/compare)
- Ehdota uutta lisäosaa issuella (liitä `addon_id` ja englanninkielinen XML tai fraasilista)

Katso myös [CONTRIBUTING.md](CONTRIBUTING.md).

## Käyttäjät

- [AvantClub.fi](https://www.avantclub.fi/)

Haluatko foorumisi listalle? Avaa issue tai lähetä pull request tähän README-tiedostoon.

## Changelog

### v2.3.12-1 (2026-08-28)

- Kielipaketin `base_version_id` päivitetty XenForo **2.3.12**:een (2031270).
- Puuttuvia lisäosafraaseja täydennetty (mm. ThemeHouse Holidays, Connected Account Providers).
- Aiemmin englanniksi jääneitä fraaseja suomennettu.
- README, asennusohjeet ja julkaisun tiedostonimi dokumentoitu.

Vanhemmat merkit: [Releases](https://github.com/Markus-web/XenForo-Finnish-Translation/releases).
