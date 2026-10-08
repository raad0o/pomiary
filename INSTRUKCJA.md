# Karta pomiaru: instrukcja

Aplikacja to 5 plików: `index.html`, `sw.js`, `manifest.webmanifest`, `icon-192.png`, `icon-512.png`.
Nie ma serwera ani bazy danych. Pomiary i zdjęcia zapisują się tylko w przeglądarce urządzenia, na którym je wpisujesz.

## 1. Wgranie na GitHub Pages (raz, ok. 15 minut)

Na GitHub trafia tylko pusty formularz. Danych klientów tam nie ma.

1. Załóż darmowe konto na github.com.
2. Utwórz nowe repozytorium (przycisk „New”), np. o nazwie `pomiary`. Ustaw je jako **Public**, bo darmowe Pages działa tylko dla publicznych repozytoriów. Publiczny jest tylko kod formularza.
3. W repozytorium kliknij „Add file” → „Upload files”, przeciągnij wszystkie 5 plików i kliknij „Commit changes”.
4. Wejdź w „Settings” → „Pages”. W polu „Branch” wybierz `main` i folder `/ (root)`, kliknij „Save”.
5. Po 1–2 minutach aplikacja będzie pod adresem `https://TWOJA-NAZWA.github.io/pomiary/`.

## 2. Telefon (Android)

1. Otwórz ten adres w Chrome.
2. Menu (trzy kropki) → „Dodaj do ekranu głównego” / „Zainstaluj aplikację”.
3. Od teraz aplikacja otwiera się z ikonki i działa bez internetu.

## 3. Komputer

Otwórz ten sam adres w Chrome lub Edge. W pasku adresu kliknij ikonę instalacji, a aplikacja pojawi się jako program.
Używaj zawsze tego samego adresu. Ten sam plik otwarty z dysku ma osobną, pustą pamięć.

## 4. Praca z pomiarem

- **Po każdym pomiarze, jeszcze u klienta: „Plik dla mnie”.** To jedyna kopia zapasowa. Na liście pomiar bez aktualnego pliku ma znaczek „bez kopii”.
- „Wyślij plik dla mnie” otwiera menu udostępniania Androida (Dysk, e-mail).
- **Przeniesienie na komputer:** na komputerze „Importuj plik” i wybierasz plik `.json`. Jeśli na komputerze jest nowsza wersja, aplikacja zapyta przed nadpisaniem.
- **Zasada:** po przeniesieniu na komputer dalsze zmiany rób tylko tam, żeby nie powstały dwie różne wersje.
- **„Plik dla Claude”:** same wymiary, bez klienta, telefonu, adresu i zdjęć. Wybrane zdjęcia dołączasz osobno.
- „Drukuj” na komputerze pozwala zapisać kartę do PDF.

## 5. Czego pilnować

- Nie czyść danych przeglądarki Chrome na telefonie, bo usuniesz pomiary. Bezpieczne są tylko te, które mają plik.
- Pomiar wpisuj na jednym urządzeniu. Telefon i tablet nie widzą nawzajem swoich danych.
- Po zmianie plików aplikacji wgraj je ponownie na GitHub i podnieś numer wersji w `sw.js` (`karta-pomiaru-v1` → `v2`). Telefon pobierze nową wersję przy najbliższym otwarciu z internetem. Twoje pomiary zostają.
