# Üzenet AI – nyilvános frissítések

Ez a tárhely kizárólag a **digitálisan aláírt Android APK-k** és a `latest.json` kiadási manifest nyilvános terjesztésére szolgál.

Az Üzenet AI forráskódja külön, **privát** GitHub-tárhelyen található.

## Frissítési csatorna

- Manifest: https://raw.githubusercontent.com/pcimpressz/Uzenet.AI-Updates/main/latest.json
- Telepítők: https://github.com/pcimpressz/Uzenet.AI-Updates/releases
- A `latest.json` fájlt a privát forráskód GitHub Actions release-folyamata állítja elő sikeres, aláírt APK fordítás után.
- A kliens HTTPS-en tölti le a manifestet és az APK-t, ellenőrzi az APK SHA-256 értékét, majd az Android rendszer telepítőjét indítja el. Az Android az APK digitális aláírását is ellenőrzi.

**Az első kiadás még nincs publikálva.** A `latest.json` az első sikeres közzétételkor jön létre. A közzétételhez a privát forráskód repójában `UZENET_PUBLISH_TOKEN` GitHub Actions Secret szükséges, amely kizárólag ennek a nyilvános tárhelynek a Contents: Read and write jogosultságát kapja.
