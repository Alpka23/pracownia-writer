# Pracownia Writer

Kompletna strona w języku polskim dla uczniów około 12. roku życia. Sześć ćwiczeń w LibreOffice Writer, test z 20 pytaniami i automatyczną oceną 1–5 z plusami i minusami.

## Uruchomienie

Otwórz `index.html` w przeglądarce. Nie wymaga instalacji, bibliotek, serwera ani kluczy API. Plik zawiera HTML, CSS i JavaScript. Przy wyłączonym JavaScript dostępne pozostają ćwiczenia.

## Punktacja

Każde pytanie jest warte 1 punkt. Punkty przyznawane są tylko za dokładny zestaw poprawnych odpowiedzi. Nie ma punktów częściowych ani ujemnych. Wymagane jest imię, klasa i odpowiedź na każde pytanie. Wynik procentowy = punkty / 20 × 100. Skala w tablicy `SCALE` obejmuje 0–100%, bez luk. Progi są pokazane na stronie przed przystąpieniem do testu. Ocena dotyczy tylko testu, nie ćwiczeń praktycznych.

## E-mail i prywatność

JavaScript generuje adres `mailto:rafal.edu@outlook.com` z zakodowanym tematem i treścią. Otwiera program pocztowy; uczeń musi sam nacisnąć Wyślij. Strona nie wysyła wiadomości w tle ani nie potwierdza doręczenia. Jeśli obsługa mailto nie jest skonfigurowana, można skopiować wynik do poczty internetowej. Kopiowanie ma awaryjne zaznaczanie tekstu w przypadku braku dostępu do schowka.

Nie umieszczaj haseł SMTP ani sekretów API w tym kodzie. Strona nie utrwala danych ucznia w cookies ani localStorage. Odświeżenie usuwa wynik. Hosting może prowadzić standardowe dzienniki ruchu. Poczta przetwarza wiadomość po wysłaniu przez użytkownika.

Test ćwiczeniowy nie zapewnia odporności na oszustwa: publiczny kod zawiera klucz odpowiedzi, a wiadomość e-mail można edytować. Do ocenianego sprawdzianu nauczyciel powinien zweryfikować wynik na ekranie ucznia.

## Publikacja w GitHub Pages

Wgraj `index.html` i ten plik do głównego katalogu publicznego repozytorium. W Settings → Pages wybierz Deploy from a branch, gałąź main, katalog / (root), następnie Save. Po zakończeniu publikacji GitHub wyświetli publiczny adres strony.

## Edycja

Ćwiczenia: sekcja HTML `cwiczenia`. Pytania i odpowiedzi: tablica `QUESTIONS`; indeksy w `correct` są liczone od zera. Progi: `SCALE`. Adres odbiorcy: wystąpienia `rafal.edu@outlook.com`. Przy zmianie liczby pytań zaktualizuj także opis punktacji i widoczne teksty strony.

Źródła merytoryczne: oficjalna pomoc LibreOffice https://help.libreoffice.org/latest/pl/text/swriter/guide/main.html oraz strony dotyczące stylów i eksportu PDF podlinkowane na stronie.
