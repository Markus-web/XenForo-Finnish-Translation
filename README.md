# XenForo suomeksi | XenForo Finnish Translation
**Täysin suomenkielinen käännöspaketti** XenForo-foorumialustalle, joka on tarkoitettu itse ylläpidettäville sivustoille. Tämän kielipaketin avulla voit käyttää XenForo-alustaa kokonaan suomen kielellä. Paketti tukee XenForo 2.x -versioita ja sisältää käännöksiä myös muutamille suosituimmille lisäosille ja tyyleille.

**Lisenssi:**
Tätä käännöspakettia saa vapaasti muokata ja käyttää omiin tarpeisiin. Jos haluat poistaa tekijänoikeusmaininnan, poista vain fraasi `extra_copyright` kielitiedostosta (ohjeet alempana).

## Julkaisut
- **[Kehitysversio](https://github.com/Markus-web/XenForo-suomeksi/archive/refs/heads/main.zip)** - Lataa viimeisin kehitysversio
- **[Viimeisin virallinen julkaisu](https://github.com/Markus-web/XenForo-suomeksi/releases)** - Lataa uusin virallinen julkaisu

## Asennusohjeet
Tämä kielipaketti on tarkoitettu XenForo 2.x+ -versioille. Vanhemmissa XenForo-versioissa voi esiintyä virheitä tai yhteensopivuusongelmia.

1. Lataa `language-Finnish-(FI).xml` -tiedosto.
2. Siirry XenForon hallintapaneeliin osoitteessa: `example.com/admin.php`.
3. Valitse **Appearance** > **Languages** > **Import**.
4. Lataa `language-Finnish-(FI).xml` -tiedosto käyttöön.

**Huom:** Jos latauksessa ilmenee virhe `Please upload a valid language XML file`, varmista, että palvelimen PHP:n `upload_max_filesize`-asetus on vähintään 3M (tai suurempi kuin ladattavan .xml-tiedoston koko).

### Markus Media -tekstin poistaminen
Kielipaketin mukana saattaa tulla ylimääräinen tekijänoikeusteksti ("Verkkosivun toteutus: Markus Media"), joka näkyy sivuston alalaidassa. Voit poistaa tai muokata tämän tekstin seuraavasti:
1. Siirry hallintapaneelissa: **Appearance** > **Languages** > **Finnish (FI)** > **Phrases**
2. Etsi fraasi nimeltä `extra_copyright`
3. Tyhjennä tai muokkaa fraasin sisältö haluamaksesi (esim. poista HTML-linkki kokonaan).

## Mukana olevat lisäosat ja tyylit
Tämä käännöspaketti sisältää suomennokset seuraaville lisäosille ja tyyleille. Huom! Kaikki käännökset eivät välttämättä ole täysin valmiita tai täydellisiä, ja osa lisäosista voi olla keskeneräisiä. Kehitystyö jatkuu ja parannuksia otetaan mielellään vastaan!

- [UI.X 2 tyyli & lisäosa](https://www.themehouse.com/xenforo/2/themes/ui-x) ([TH] UI.X 2.3.0 Patch Level 1)
- [Connected Account Providers](https://www.themehouse.com/xenforo/2/addons/connected-account-providers)
- [Donate](https://www.themehouse.com/xenforo/2/addons/donate)
- [Holidays](https://www.themehouse.com/xenforo/2/addons/holidays)
- [User Criteria Extended](https://www.themehouse.com/xenforo/2/addons/user-criteria-extended)
- [Email log](https://www.xf2addons.com/resources/email-log.97/) (2.6)
- [Forum statistics plus](https://www.xf2addons.com/resources/forum-statistics-plus.101/) (1.7)
- [Install & Upgrade](https://www.themehouse.com/xenforo/2/addons/install-and-upgrade)
- [History](https://www.xf2addons.com/resources/history.54/) (2.7)
- [Most posts](https://www.xf2addons.com/resources/most-posts.46/) (2.2)
- [s9e/MediaSites](https://xenforo.com/community/resources/s9e-media-sites.5973/) (2.18.6)
- [Weekly newsletter](https://www.xf2addons.com/resources/weekly-newsletter.584/) (2.1)
- [Similar threads](https://www.xf2addons.com/resources/similar-threads.17/) (8.8)
- [Trader](https://www.xf2addons.com/resources/trader.55/) (3.1)
- [Audentio Feeds](https://www.themehouse.com/xenforo/2/addons/feeds) (1.4.0 Patch Level 4)
- [Kirby Style Variation Default](https://xenforo.com/community/resources/style-variation-default.9504/) (1.1.0 Patch 1)
- [What's New Tweak](https://xenforo.com/community/resources/xb-whats-new-tweak.6809/) (2.2.2 Patch Level 1)
- [Add-on Update Notifier](https://xenforo.com/community/resources/add-on-update-notifier.9002/) (1.1.8 Patch Level 1)
- [Ads Manager Lite](https://siropu.com/products/ads-manager-2-lite/) (1.3.6)
- [App for Cloudflare®](https://xenforo.com/community/resources/digitalpoint-app-for-cloudflare-r.8750/) (1.9.1.1)
- [Attachment Improvements](https://xenforo.com/community/resources/attachment-improvements-by-xon.6629/) (2.6.7)
- [Auto close by prefix](https://www.xf2addons.com/) (1.2)
- [Email Queuing Enhancements](https://xenforo.com/community/resources/email-queuing-enhancements.6631/) (2.4.1)
- [Search Improvements](https://xenforo.com/community/resources/search-improvements.6838/) (2.17.0)
- [Standard Library](https://xenforo.com/community/resources/standard-library-by-xon.7915/) (1.22.4)
- [Version check](https://www.xf2addons.com/) (2.2)

## Haluatko auttaa käännöksessä?
Huomasitko kirjoitusvirheen tai parannettavaa käännöksissä? Voit auttaa parantamaan tätä projektia seuraavasti:

- **Pull Request**: Tee omat parannuksesi ja luo [pull request](https://github.com/Markus-web/XenForo-Finnish-Translation/compare).
- **Ilmoita ongelmasta**: Luo uusi [issue](https://github.com/Markus-web/XenForo-Finnish-Translation/issues/new/choose) ja kuvaile löytämäsi ongelma.

## Käännöspaketin käyttäjät
Alla on lista foorumeista, jotka käyttävät tätä suomenkielistä käännöspakettia:

- [AvantClub.fi](https://www.avantclub.fi/)

## Roadmap
- **Tavoite:** Kääntää koko XenForo ja mahdollisimman moni lisäosa suomeksi!
