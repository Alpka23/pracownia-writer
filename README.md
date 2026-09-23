# Pracownia Writer

Kompletna strona w języku polskim dla uczniów około 12. roku życia. Sześć ćwiczeń w LibreOffice Writer, test z 20 pytaniami i automatyczną oceną 1–5 z plusami i minusami.

## Uruchomienie

Otwórz `index.html` w przeglądarce. Nie wymaga instalacji, bibliotek, serwera ani kluczy API. Plik zawiera HTML, CSS i JavaScript. Przy wyłączonym JavaScript dostępne pozostają ćwiczenia.

## Punktacja

Każde pytanie jest warte 1 punkt. Punkty przyznawane są tylko za dokładny zestaw poprawnych odpowiedzi. Nie ma punktów częściowych ani ujemnych. Wymagane jest imię, klasa i odpowiedź na każde pytanie. Wynik procentowy = punkty / 20 × 100. Skala w tablicy `SCALE` obejmuje 0–100%, bez luk. Progi są pokazane na stronie przed przystąpieniem do testu. Ocena dotyczy tylko testu, nie ćwiczeń praktycznych.

## E-mail i prywatność

Przycisk „Wyślij wynik nauczycielowi” wywołuje przez JavaScript HTTPS POST do `https://formsubmit.co/ajax/rafal.edu@outlook.com`. Usługa FormSubmit przekazuje zgłoszenie na pocztę nauczyciela. Uczeń nie potrzebuje konta e-mail ani programu pocztowego. Wysyłanie wymaga internetu.

Treść żądania zawiera dokładnie cztery pola: `Imię`, `Klasa`, `Procenty` i `Ocena`. Nie są wysyłane odpowiedzi, liczba punktów ani data. Usługa może dodać własną stopkę, nagłówki i metadane techniczne wiadomości. Kopiowanie wyniku pozostaje jako opcja awaryjna.

### Jednorazowa aktywacja — nauczyciel

Po pierwszym zgłoszeniu FormSubmit wysyła wiadomość aktywacyjną do rafal.edu@outlook.com. Odbiorca musi kliknąć link potwierdzający (sprawdź również Spam). Przed użyciem z klasą sprawdź odbiór wyniku próbnego. Do chwili aktywacji przyjęcie zgłoszenia nie oznacza dostarczenia wiadomości z wynikiem. Nie wpisuj haseł do poczty na stronie testu.

Obsługiwane są: blokada wielokrotnego kliknięcia, odpowiedź błędu, limit oczekiwania 20 sekund i ręczne ponowienie. Przyjęcie przez usługę nie jest potwierdzeniem doręczenia. Przy błędzie sieci nie wiadomo, czy zgłoszenie dotarło; ponowienie może spowodować duplikat.

Nie umieszczaj haseł SMTP ani sekretów API w tym kodzie. Strona nie utrwala danych ucznia w cookies ani localStorage. Odświeżenie usuwa wynik. FormSubmit przechowuje zgłoszenia przez 30 dni. Hosting, usługa i poczta mogą przetwarzać techniczne dane połączenia. Używaj rozwiązania zgodnie z zasadami szkoły dotyczącymi przetwarzania danych uczniów.

Test ćwiczeniowy nie zapewnia odporności na oszustwa: publiczny kod zawiera klucz odpowiedzi i użytkownik może zmienić wysyłany wynik za pomocą narzędzi programistycznych. Do ocenianego sprawdzianu nauczyciel powinien zweryfikować wynik na ekranie ucznia.

Dokumentacja usługi: https://formsubmit.co/ajax-documentation i https://formsubmit.co/help

## Publikacja w GitHub Pages

Wgraj `index.html` i ten plik do głównego katalogu publicznego repozytorium. W Settings → Pages wybierz Deploy from a branch, gałąź main, katalog / (root), następnie Save. Po zakończeniu publikacji GitHub wyświetli publiczny adres strony.

## Edycja

Ćwiczenia: sekcja HTML `cwiczenia`. Pytania i odpowiedzi: tablica `QUESTIONS`; indeksy w `correct` są liczone od zera. Progi: `SCALE`. Adres odbiorcy: wystąpienia `rafal.edu@outlook.com`. Przy zmianie liczby pytań zaktualizuj także opis punktacji i widoczne teksty strony.

Źródła merytoryczne: oficjalna pomoc LibreOffice https://help.libreoffice.org/latest/pl/text/swriter/guide/main.html oraz strony dotyczące stylów i eksportu PDF podlinkowane na stronie.
