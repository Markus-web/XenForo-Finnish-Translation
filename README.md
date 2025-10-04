# XenForo suomeksi | XenForo Finnish Translation
**Täysin suomenkielinen käännöspaketti** XenForo-foorumialustalle, joka on tarkoitettu itse ylläpidettäville sivustoille. Tämän kielipaketin avulla voit käyttää XenForo-alustaa kokonaan suomen kielellä. Paketti tukee XenForo 2.x -versioita ja sisältää kattavat käännökset useille suosituille lisäosille ja tyyleille.

## Julkaisut
- **[Kehitysversio](https://github.com/Markus-web/XenForo-Finnish-Translation/archive/refs/heads/main.zip)** - Lataa viimeisin kehitysversio
- **[Viimeisin virallinen julkaisu](https://github.com/Markus-web/XenForo-Finnish-Translation/releases)** - Lataa uusin virallinen julkaisu

## Asennusohjeet
Tämä kielipaketti on tarkoitettu XenForo 2.x+ -versioille. Vanhemmissa XenForo-versioissa voi esiintyä virheitä tai yhteensopivuusongelmia.

1. Lataa `language-Finnish-(FI).xml` -tiedosto.
2. Siirry XenForon hallintapaneeliin osoitteessa: `example.com/admin.php`.
3. Valitse **Appearance** > **Languages** > **Import**.
4. Lataa `language-Finnish-(FI).xml` -tiedosto käyttöön.

**Huom:**
- Jos latauksessa ilmenee virhe `Please upload a valid language XML file`, varmista, että palvelimen PHP:n `upload_max_filesize`-asetus on vähintään 5M (tai suurempi kuin ladattavan .xml-tiedoston koko).
- Suosittelemme varmuuskopioimaan nykyisen kielipaketin ennen uuden asentamista.
- Jos haluat päivittää olemassa olevan kielipaketin, valitse **Overwrite language** -vaihtoehto tuonnin aikana.

## Päivittäminen
- Lataa uusin `language-Finnish-(FI).xml` julkaisuista.
- XenForon hallinnassa: **Appearance** > **Languages** > valitse nykyinen suomen kieli > **Import** > valitse tiedosto ja ruksaa **Overwrite language**.
- Tyhjennä välimuisti tarvittaessa: **Development** > **Clear caches**.

## Vianmääritys
- “Please upload a valid language XML file”: tiedostokoko ylittää PHP-rajan → nosta `upload_max_filesize` ja `post_max_size`.
- Merkkipolut/ääkköset sekaisin: varmista UTF-8 ilman BOM:ia.
- Templatet rikkoutuvat: tarkista, ettei fraaseihin ole lisätty tai poistettu HTML/BB-koodien rakenteita.

## Vaatimukset
- **XenForo 2.3.7+** suositeltu (toimii myös 2.2.x, pienin varauksin)
- **PHP 8.0+** suositus. Suurehko XML-tiedosto edellyttää riittäviä PHP rajoja
- **Vähintään 5MB** `upload_max_filesize` ja `post_max_size` PHP-asetuksissa
- **UTF-8** koodaus ilman BOM-merkintää

### Vinkkejä käännösfraaseihin (ylläpitäjille)
- Säilytä muuttujat sellaisenaan: `{username}`, `{board}`, `{date}`, `{tag}`, `{count}` jne.
- Säilytä printf-tyyliset paikat: `%d`, `%s`, `%1$s` jne. sekä BB-koodit ja HTML-tagit.
- Vältä johtavia tai perässä olevia ylimääräisiä välilyöntejä, jos fraseja verrataan tarkasti.

### Yhteensopivuus
- **Testattu XenForo-versioilla**: 2.3.7
- **Käännöksen kattavuus**: Kattava XenForo-ydin + useita lisäosia
- **Käännöksen laatu**: Luonnollinen suomen kieli, johdonmukainen termistö

### Tekijänoikeustekstin poistaminen
Kielipaketin mukana tulee tekijänoikeusteksti ("XenForo-sivuston suomenkielinen lokalisointi – Markus Media"), joka näkyy sivuston alalaidassa. Voit poistaa tai muokata tämän tekstin seuraavasti:
1. Siirry hallintapaneelissa: **Appearance** > **Languages** > **Finnish (FI)** > **Phrases**
2. Etsi fraasi nimeltä `extra_copyright`
3. Tyhjennä tai muokkaa fraasin sisältö haluamaksesi (esim. poista HTML-linkki kokonaan)

## Mukana olevat lisäosat ja tyylit
Tämä käännöspaketti sisältää kattavat suomennokset seuraaville lisäosille ja tyyleille.

**ThemeHouse Suite:**
- [UI.X 2 tyyli & lisäosa](https://www.themehouse.com/xenforo/2/themes/ui-x) - Tehokas ja moderni teema
- [Connected Account Providers](https://www.themehouse.com/xenforo/2/addons/connected-account-providers) - Ulkoiset kirjautumispalvelut
- [Donate](https://www.themehouse.com/xenforo/2/addons/donate) - Lahjoitustoiminnallisuus
- [Holidays](https://www.themehouse.com/xenforo/2/addons/holidays) - Lomateemat ja -toiminnot
- [User Criteria Extended](https://www.themehouse.com/xenforo/2/addons/user-criteria-extended) - Laajennetut käyttäjäkriteerit
- [Install & Upgrade](https://www.themehouse.com/xenforo/2/addons/install-and-upgrade) - Lisäosien hallinta

**XF2 Addons Suite:**
- [Email log](https://www.xf2addons.com/resources/email-log.97/) - Sähköpostiloki
- [Forum statistics plus](https://www.xf2addons.com/resources/forum-statistics-plus.101/) - Lisätilastot
- [History](https://www.xf2addons.com/resources/history.54/) - Käyttäjien katsomat ketjut
- [Most posts](https://www.xf2addons.com/resources/most-posts.46/) - Aktiivisimmat käyttäjät
- [Weekly newsletter](https://www.xf2addons.com/resources/weekly-newsletter.584/) - Uutiskirjeet
- [Similar threads](https://www.xf2addons.com/resources/similar-threads.17/) - Samankaltaiset ketjut
- [Trader](https://www.xf2addons.com/resources/trader.55/) - Kauppatoiminnallisuus

**Muut lisäosat:**
- [s9e/MediaSites](https://xenforo.com/community/resources/s9e-media-sites.5973/) - Median upotus
- [App for Cloudflare®](https://xenforo.com/community/resources/digitalpoint-app-for-cloudflare-r.8750/) - Cloudflare-integraatio
- [Attachment Improvements](https://xenforo.com/community/resources/attachment-improvements-by-xon.6629/) - Liitetiedostojen parannukset
- [Search Improvements](https://xenforo.com/community/resources/search-improvements.6838/) - Hakutoiminnon parannukset
- [Standard Library](https://xenforo.com/community/resources/standard-library-by-xon.7915/) - Apukirjasto
- [Ads Manager Lite](https://siropu.com/products/ads-manager-2-lite/) - Mainosten hallinta
- [What's New Tweak](https://xenforo.com/community/resources/xb-whats-new-tweak.6809/) - "Mitä uutta" -sivun muokkaus

## Haluatko auttaa käännöksessä?
Vaikka käännöspaketti on jo hyvin kattava, voit auttaa parantamaan sitä edelleen:

- **Ilmoita ongelmasta**: Luo [issue](https://github.com/Markus-web/XenForo-Finnish-Translation/issues/new/choose) jos löydät kirjoitusvirheen tai parannettavaa
- **Pull Request**: Tee omat parannuksesi ja luo [pull request](https://github.com/Markus-web/XenForo-Finnish-Translation/compare)
- **Ehdotus**: Ehdota uusia lisäosia kääntämistä varten
- **Tähti**: Anna tähti GitHub-repositoriolle jos pidät projektista

## Käännöstyyliohje ja termistö
- Käytä luonnollista, selkeää yleiskieltä. Vältä liian teknisiä anglismeja, kun suomenkielinen vastine on vakiintunut.
- Säilytä termit johdonmukaisina: thread = keskustelu/ketju, post = viesti, attachment = liite, tag = tunniste, reaction = reaktio.
- Pidä tekstit lyhyinä käyttöliittymässä; vältä toistoa.

## Lisenssi
Tämä projekti on lisensoitu MIT-lisenssillä. Katso tiedosto [LICENSE](LICENSE).

## Käännöspaketin käyttäjät
Alla on lista foorumeista, jotka käyttävät tätä suomenkielistä käännöspakettia:

- [AvantClub.fi](https://www.avantclub.fi/)

*Haluatko listata foorumisi tähän? Ota yhteyttä!*

## Roadmap
- **Jatkuva ylläpito**: Päivitykset uusille XenForo-versioille ja lisäosille
- **Laadun parantaminen**: Käännösten hienosäätö käyttäjäpalautteen perusteella
- **Uudet lisäosat**: Kääntäminen uusille suosituille lisäosille
