---
title: "Jak nie dać się zhakować?"
slug: "jak-nie-dac-sie-zhakowac"
date: 2021-02-04T14:22:44+01:00
draft: false
tags: [informatyka, cyberbezpieczeństwo, szyfrowanie, "manager haseł", LastPass]
---

Jak nie dać się zhackować? Jak przechowywać swoje hasła?<!--more-->

# Jak nie dać się zhackować?
1. **Aktualizuj swoje oprogramowanie.** Nie ma sensu odwlekać aktualizacji swoich programów i systemów, ponieważ takie aktualizacje mogą zawierać krytyczne poprawki bezpieczeństwa. Aktualna przeglądarka, w miarę aktualny system operacyjny oraz aktualny anty-wirus to podstawa.
2. **Korzystaj z managera haseł.** Jeśli Twoje hasło to `123` to raczej nie możesz czuć się bezpiecznie. Jeśli korzystasz z tego samego hasła do kilku portali to wtedy **wyciek jednego hasła naraża Cię na stratę kont we wszystkich portalach**. Nie możesz również czuć się bezpiecznie jeśli masz to samo hasło, ale dodajesz do niego nazwę aktualnego portalu, np: `mojeHasło-facebook` oraz `mojeHasło-instagram`. Dodawanie jakiegoś wyrazu, cyfry, litery, znaku, nazwy własnej czy czegokolwiek po prostu nie jest tak bezpieczne jak nowe, losowe i unikalne hasło. **Najlepiej byłoby mieć wyjątkowo długie, skomplikowane i unikalne hasło do każdego serwisu osobno**, a że człowiek nie do końca dobrze sobie radzi z zapamiętywaniem losowych znaków to pomoże tutaj manager haseł, który:
   - wygeneruje niezwykle skomplikowane i unikalne hasło za Ciebie, np: `YC?HkPSwuNtU}Q]Yy*BBpP]]{2`,
   - zapisze w swojej bazie danych w taki sposób, że sam manager go nie zna, bo wysyłasz mu już zaszyfrowaną wartość,
   - sprawdzi czy na pewno jest ono unikalne i czy przypadkiem już go gdzieś nie używasz,
   - (czasami) nawet poinformuje Cię, że Twoje hasło wyciekło z jakiegoś portalu i zasugeruje Ci jego zmianę (*mimo, że sam manager nie wie jakie te hasło jest*),
   - (przeważnie) automatycznie zsynchronizuje się ze wszystkimi Twoimi urządzeniami, abyś miał dostęp do nowego hasła zarówno na PC, laptopie czy telefonie,
   - pokaże Ci w przybliżeniu jak bezpieczne jest hasło z którego korzystasz. Fantastyczne hasła są długie i skomplikowane,
   - (czasami) umożliwi Ci bezpieczne współdzielenie wybranch haseł z innymi użytkownikami,
   - (czasami) umożliwi Ci dostęp do wszystkich Twoich haseł komuś zaufanemu jeśli nie zalogujesz się przez *X* dni, więc gdy przydarzy Ci się nieszczęście to np. rodzina będzie miał dostęp do najważniejszych kont lub haseł.
3. **Korzystaj z drugiego składnika autoryzacyjnego wszędzie gdzie się da.** Czyli dodatkowego kodu, który musimy wpisać po podaniu hasła. Fajnie, gdy dostajemy taki kod SMS-em. Lepiej, gdy mamy aplikację, która wygeneruje ten kod (tzw. [TOTP](https://en.wikipedia.org/wiki/Time-based_One-Time_Password)) za nas - bo taka aplikacja nie wymaga, *żadnego medium* (ani internetu, ani sieci komórkowej). Najlepiej gdy mamy od tego specjalne urządzenie jak np. **[YubiKey](https://allegro.pl/listing?string=yubikey%20nfc)**, który (w skrócie) zanim wygeneruje taki kod to sprawdzi czy to aby na pewno poprawna strona. Gdy nie chcesz korzystać z drugiego składnika wszędzie to użyj go przynajmniej do zabezpieczenia swojego managera haseł.
4. **Nie klikaj we wszystko co znajdziesz w internecie.** Stosowanie popularnych rozszerzeń do przeglądarek typu *AdBlock* (dla [Firefoxa](https://addons.mozilla.org/en-US/firefox/addon/adblock-plus/) lub [Chrome](https://chrome.google.com/webstore/detail/adblock-%E2%80%94-best-ad-blocker/gighmmpiobklfepjocnamgkkbiglidom)) już w jakimś stopniu zablokuje niepożądane/niebezpieczne strony i reklamy.
5. **Nie otwieraj nieznanych załączników w e-mail'ach.** Dziwny mail z załączonym arkuszem Excel'a, PDF czy aplikacja z rozszerzeniem .exe może poczekać aż się upewnisz, że jest ten mail na jaki czekałeś i wiesz, że pochodzi z wiarygodnego źródła.
6. **Wymagaj hasła/PINu/odcisku palca przy każdym odblokowaniu telefonu.** Zwłaszcza, gdy korzystasz z niego do odbierania kodu z *drugiego składnika autoryzacyjnego*.
7. **Korzystaj z komunikatorów, które szanują Twoją prywatność.** Absolutnym liderem wśród komunikatorów oferujących rewelacyjne szyfrowanie jest **[Signal](https://www.signal.org/)** rozwijany przez organizację [non-profit](https://www.signal.org/donate/). WhatsApp też całkiem dobrze może szyfrować komunikację, natomiast może również zbierać znacznie więcej metadanych o osobach używających go.

# Skąd wiem, że manager haseł jest bezpieczny?
Większość managerów haseł uczestniczy w programach typu "Bug Bounty", czyli "Łowców Błędów". Taki program zakłada, że jeśli komuś uda się zhackować managera to sam manager wypłaci mu za to sporą kwotę (na dzień 03.02.2021r. jest to [~18 600 PLN](https://bugcrowd.com/lastpass) w przypadku LastPass'a), więc prawdopodobnie bardziej będzie się opłacać przestępcom zgłosić taki błąd, niż wykorzystać go do poznania czyjegoś hasła.

Ponadto takie managery w miarę często zatrudniają zewnętrzne firmy do przeprowadzenia testów bezpieczeństwa swoich aplikacji. Przykładowo LastPass przeprowadza takie testy przynajmniej [raz do roku](https://www.lastpass.com/security/what-if-lastpass-gets-hacked).

Cała architektura takiego oprogramowania jest tworzona z zamysłem, aby nawet sami twórcy nie byli w stanie odtworzyć Twojego hasła. Dlatego, gdy zapomnisz hasła głównego to absolutnie nikt Ci pomoże jeśli się przed tym nie zabezpieczyłeś.

Managery haseł przeważnie chwalą się [publicznie](https://www.lastpass.com/enterprise/security) użytymi przez siebie algorytmami szyfrującymi, a więc można sprawdzić jakość samych algorytmów, żeby się o tym przekonać. Przeważnie jest to *[Advanced Encryption Standard](https://pl.wikipedia.org/wiki/Advanced_Encryption_Standard)* z kluczem o długości 256 bitów (zer lub jedynek). Jest to tak dobre szyfrowanie, że od [czerwca 2003](https://web.archive.org/web/20101106122007/http://csrc.nist.gov/groups/ST/toolkit/documents/aes/CNSS15FS.pdf) jest zalecany przez amerykańską agencję bezpieczeństwa narodowego  (NSA) do szyfrowania dokumentów od których zależy bezpieczeństwo kraju.

Obrazowo rzecz ujmując: **gdyby zastosować AES 256-bit z odpowiednio skomplikowanym hasłem i zacząć je łamać od początku istnienia wszechświata z wykorzystaniem całego arsenału jakim dysponuje aktualnie Google to do dnia dzisiejszego by się to nie udało.**

{{< youtube S9JGmA5_unY >}}

*Film odnosi się do [SHA-2](https://en.wikipedia.org/wiki/SHA-2) 265-bit, natomiast szyfrowanie AES 256-bit będzie conajmniej równie trudne do złamania. Jest opcja polskich napisów.*

# Popularne managery haseł
**[LastPass](https://lastpass.com/)** - osobiście go polecam dla każdego. Dostępny jako plugin do przeglądarek oraz jako aplikacja na Android'a oraz iOS'a. Dodatkowo ma [LastPass Authenticator'a](https://play.google.com/store/apps/details?id=com.lastpass.authenticator&hl=en_US&gl=US), który działa jako drugi składnik autoryzacyjny i który zapisuje parametry niezbędne do generowania jednorazowych haseł w samym LastPass'ie, więc mamy wszystko zapisane w jednej aplikacji. Zaszyfrowane hasła są trzymane w chmurze automatycznie, więc nie musimy się przejmować synchronizacją. Jest w większości darmowy, opcja płatna jest dopiero gdy chcemy wykorzystać do niego klucz sprzętowy.<!--Napisałem też artykuł jak zacząć z niego korzystać: **[link]({{< ref "manager-hasel" >}})**.-->

[KeePassXC](https://keepassxc.org/) - otwarto-źródłowy manager haseł, który przechowuje zaszyfrowane hasło jako plik na komputerze/telefonie i sami musimy zadbać o jego odpowiednią synchronizację na innych urządzeniach. Działa kompletnie offline i nie wymaga żadnego połączenia z internetem. Najwiekszą zaletą jest to, że jest całkowicie darmowy.

[Dashlane](https://www.dashlane.com/) - jest darmowy tylko do 50 haseł i jednego urządzenia.

# Jak sam dbam o bezpieczeństwo?
- Korzystam osobiscie z LastPass'a do każdego hasła jakie mam, numerów kart kredytowych, PINów, haseł do banków, numeru dowodu osobistego, prawa jazdy, PESELu, itp. W skrócie do absolutnie wszystkiego.. z tym zastrzeżeniem, że *LastPass sam wygenerował wszystkie te hasła*.
- Ustawiłem LastPassa, żeby każde wygenerowane hasło składało się z ponad 30 znaków, dużych i małych liter, cyfr oraz znaków specjalnych
- Korzystam z drugiego składnika autoryzacyjnego na każdym portalu, który go wspiera.
- Korzystam z LastPass Authenticator do przechowywania tych składników.
- Kupiłem [YubiKey 5 NFC](https://allegro.pl/listing?string=yubikey%20nfc) z którego korzystam - jako sprzętowy drugi składnik autoryzacyjny - zarówno do zabezpieczenia samego LastPass'a oraz do wszystkich portali, które go wspierają (np. Facebook, Google, Twitter czy GitHub)
- Ustawiłem LastPass'a tak aby pozwalał na zalogowanie tylko z odpowiednich krajów oraz nie zezwalał na łączenie z sieci [Tor](https://pl.wikipedia.org/wiki/Tor_(sie%C4%87_anonimowa))
- Główne hasło ma ponad 20 znaków (małych i dużer liter, cyfr oraz znaków specjalnych) i jest w pełni losowe (nie zawiera żadnego wyrazu) i według [security.org](https://www.security.org/how-secure-is-my-password/) złamanie go zajęło by około 7 kwadrylionów (7 bilionów bilionów) lat. {{< img-nz "Security.org" "passwordSecurity.png" >}}
- Mój telefon jest zabezpieczony 6-cio cyfrowym pinem oraz odciskiem palca.
- Nauczyłem się jak szybko wyłączyć logowanie poprzez biometrię.
- Zaplanowałem kilka sposobów, aby odzyskać dostęp od LastPass'a w przypadku zgubienia telefonu lub Yubikey'a.
- Zarejestrowałem wszystkie swoje e-mail'e na portalu **[haveibeenpwned.com](https://haveibeenpwned.com/)**, który powiadomi mnie automatycznie gdy któryś z portali z którego korzystam zostanie zhackowany, a moje dane wypłyną do sieci. Dzięki temu szybko będę mógł zmienić wszystkie hasła.
- W przypadku, gdy muszę podłączyć się do nie zaufanej sieci korzystam z **[NordVPN](https://nordvpn.com)**, aby dodatkowo szyfrować cały ruch internetowy.
- Najbardziej istotne pliki trzymam w zaszyfrowanej postaci korzystając z **[VeraCrypt](https://www.veracrypt.fr/code/VeraCrypt/)**, który po podaniu hasła tworzy w komputerze osobny dysk z zawartością moich plików i mogę z niego korzystać do woli. Każda zmiana na tym dysku będzie z automatu zaszyfrowana. Takie rozwiązanie jest łatwe i intuicyjne, a przy tym VeraCrypt proponuje bardzo wysoki standard szyfrowania, a nawet "partycję ukrytą" ;) 

# Jak zacząć korzystać z managera haseł?
W osobnym artykule opiszę niedługo jak zainstalować oraz korzystać z LastPass - managera haseł z którego sam korzystam. <!--Artykuł jest dostępny tutaj: **[link]({{< ref "manager-hasel" >}})**-->