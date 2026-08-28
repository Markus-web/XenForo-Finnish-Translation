# Osallistuminen

Kiitos avusta XenForon suomenkielisen kielipaketin ylläpidossa.

## Fraasien muokkaus

1. Muokkaa tiedostoa `language-Finnish-(FI).xml`.
2. Säilytä XML-rakenne: `title`, `addon_id`, `version_id`, `version_string` ja CDATA-sisältö.
3. Älä muuta `title`- tai `addon_id`-kenttiä.
4. Paikkamerkit `{...}` ja HTML/BB-koodi on pidettävä samoina kuin englanninkielisessä alkuperäisessä.
5. Älä lisää emoji-merkkejä fraaseihin.

## Pull request

- Yksi selkeä aihe per PR (esim. yksi lisäosa tai yksi UI-alue).
- Kuvaa lyhyesti: mikä muuttui ja miksi.
- Testaa tuonti XenForo 2.3.x:ssä **Overwrite language** -valinnalla, jos mahdollista.

## Issue

Kerro:

- XenForo-versio
- Lisäosan nimi ja `addon_id` (jos tiedossa)
- Fraasin `title` (Phrase title hallinnassa)
- Nykyinen suomi + ehdotettu korjaus
- Missä teksti näkyy (julkinen sivu, hallinta, sähköposti)

## Kieli

README ja fraasit ovat suomeksi. Issue- ja PR-tekstit voivat olla suomeksi tai englanniksi.
