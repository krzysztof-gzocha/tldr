---
title: "Jak zacząć korzystać z managera haseł?"
slug: "jak-zaczac-korzystac-z-managera-hasel"
date: 2021-02-04T14:48:26+01:00
draft: false
tags: [informatyka, "manager haseł", LastPass]
---

Jak założyć konto, zainstalować oraz korzystać z polecanego przeze mnie managera haseł - LastPass. W artykule **[jak nie dać się zhakować]({{< ref "jak-nie-dac-sie-zhackowac" >}})** opisałem zalety korzystania z managera haseł oraz dlaczego uważam, że są one bezpieczne i zalecane. W tym artykule pokażę w miarę krótko jak zacząć korzystać z jednego z nich - LastPass.<!--more-->

# Wymagania
- W miarę aktualna przeglądarka. Najlepiej *[Mozilla Firefox](https://www.mozilla.org/pl/firefox/new/)*, *[Opera](https://www.opera.com/pl)*, *[Brave](https://brave.com/)* lub *[Google Chrome](https://www.google.com/chrome/index.html)*.
- Opcjonalnie telefon z systemem: *Android* lub *iOS*

# Wymyśl hasło główne
Aby zapewnić bezpieczeństwo na najwyższym standardzie należy zwrócić uwagę na poziom skomplikowania swojego głównego hasła. **Nie powinno** ono zawierać żadnego wyrazu, a być raczej zbitkiem pseudo-losowych znaków.

Hasła typu: `klopsik123`, `klopsik123-facebook` czy nawet swój [PESEL](https://niebezpiecznik.pl/post/jak-zlamac-haslo-do-zipa-pesel/) na prawdę nie stanowią większego problemu do złamania w przypadku wycieku danych z jakiegoś portalu, ponieważ pozwalają na zastosowanie gotowych "słowników" haseł lub "[tablic tęczowych](https://pl.wikipedia.org/wiki/T%C4%99czowe_tablice)" (zależnie od zastosowanego przez portal algorytmu do "szyfrowania" hasła).

### Jak stworzyć dobre hasło i go nie zapomnieć? {#dobre-haslo}
Znacznie prościej będzie zapamiętać całe zdanie, prawda? Może to być tekst piosenki, cytat czy nawet zdanie nie mające sensu: **`W dwatysiąceosiemnastym powiedziałem: skorpiony latają kluczem`**. Mając takie zdanie możemy je przerobić tak, aby hasło wydawało się losowe (było pseudo-losowe) na przykład poprzez łączenie ze sobą kilku liter z każdego wyrazu i dodanie między nie znaków specjalnych jak na przykład: **`w@0!8Pow:SKoLATaąklU`**. Oczywiście znaki `@0!8` powstały przez przytrzymanie klawisza "shift" podczas pisania pierwszej i trzeciej cyfry roku 2018. Według [security.org](https://www.security.org/how-secure-is-my-password/) złamanie takiego hasła zajęłoby około *66 septylionów* (66 i 42 zera) lat, więc można przyznać, że hasło jest wystarczająco dobre.

[{{< img-nz "security.org" "manager.haslo.png" >}}](https://www.security.org/how-secure-is-my-password/)

# Zarejestruj się
Formularz rejestracji nowego użytkownika znajduje się [tutaj](https://lastpass.com/create-account.php). Formularz prosi jedynie o podstawowe dane czyli email, hasło główne oraz tzw. *"Reminder"* czyli coś co pozwoli Ci przypomnieć sobie hasło. Nie może to oczywiście być [zdanie użyte do stworzenia hasła]({{< ref "#dobre-haslo" >}}) ani samo hasło. Po rejestracji LastPass wyśle Ci email na wskazany w rejestracji adres z linkiem do potwierdzenia konta. Po kliknięciu w link konto powinno być aktywne i gotowe do użycia.

{{< img-nz "Rejestracja w LastPass" "lastpass.register.png">}}

# Skonfiguruj odzyskiwanie konta
Po zalogowaniu się na stronie LastPass pokaże się Nam nasz - na razie pusty - sejf (ang. vault). Przed zapisaniem jakiegokolwiek hasła w sejfie warto skonfigurować dodatkową metodę odzyskania konta w LastPass. 

### Odzyskanie konta poprzez SMS
Aby to zrobić należy wybrać z menu po lewej *Account Settings*, pokaże się Nam nowe okno na dole którego będzie pole *SMS Account Recovery*, które służy do podania (lub w przyszłości aktualizacji) numeru telefonu, który będzie mógł zrestartować hasło w przypadku jego zapomnienia. Myślę, że warto go podać, aby zadbać o bezpieczeństwo swojego konta.

# Dodatkowe zabezpieczenia
Możemy do nich przejść wchodząć do swojego sejfu, klikając *Account Settings*, a następnie *Show Advanced Settings*. Pojawią się Nam wtedy na dole kranu dodatkowe opcje. Interesuje Nas teraz tabelka *Security* bo niej możemy skonfigurować:
- *Security Email*: dodatkowy email zabezpieczający jeśli masz drugie, bezpieczne konto, 
- *Country Restrictions*: restrykcję co do kraju z którego będzie można się zalogować do LastPass'a - polecam wybrać kraje z których będziesz się logował,
- *Tor Networks*: blokada logowania z anonimowej sieci [Tor](https://pl.wikipedia.org/wiki/Tor_(sie%C4%87_anonimowa)) - polecam włączyć,
- *Revert Master Password*: umożliwienie wycofania zmiany hasła głównego - polecam włączyć,
- *Disable Email Verification*: wyłączenie weryfikacji mailowej podczas logowanie z nowego urządzenia lub lokalizacji - polecam wyłączyć,
- *Disable Multifactor Trust Expiration*: wyłączenie czasowego limitu zaufania urządzeń po 30 dniach - polecam wyłączyć,
- *Auto-Logoff Other Devices* - wylogowanie innych urządzeń, gdy zalogujesz się z innego IP - polecam włączyć obydwa,
- *Password Iterations*: ile razy użyć funkcji zaciemniającej (hasującej) hasło - polecam ponad 100 tysięcy,

{{< img-nz "LastPass: Security" "lastpass.security.png" >}}

# Zainstaluj plugin do przeglądarki
Na stronie *[Downloads](https://lastpass.com/misc_download2.php)* możemy znaleźć wszystkie oficjalnie wspierane pluginy do przeglądarek. Korzystając z tej strony będziemy pewni, że zaistalowaliśmy oficjalny plugin. Po wybraniu odpowiedniego systemu operacyjnego oraz przeglądarki możemy kliknąć "Download", a przeglądarka sama przeprowadzi Cię przez szybki proces instalacji pluginu. Jeśli w trakcie instalacji pluginu przeglądarka zapyta Cię o dodatkowę zgody to należy ich udzielić, aby zapewnić poprawne działanie pluginu. 

Po pomyślnej instalacji plugin będzie dostępny jako czerwona ikonka koło pasku adresu. Teraz zostało Nam jedynie zalogować się na swoje konto poprzez plugin. Wystarczy kliknąć w jego ikonkę i podać login oraz hasło.

# Dodaj pierwsze hasła
Od tej pory LastPass będzie sprawdzał strony, które przeglądamy i gdy wykryje, że podajemy w jakimś formularzu hasło zapyta się Nas czy powinien je zapisać. Pytanie to pojawi się jako małe okienko w prawym, górnym rogu. Po kliknięciu "*Add*" hasło zostanie zapisane i LastPass będzie mógł już je podpowiadać przy kolejnym wejściu na tę stronę.

{{< img-nz "LastPass: dodawanie nowego hasła" "lastpass.nowe.png" >}}

To niestety nie gwarantuje, że te hasła są najlepsze ponieważ zapisaliśmy w LastPass'ie hasła, które sami stworzyliśmy i pamiętamy, a idealnie byłoby gdyby to właśnie LastPass je wygenerował.

# Pozmieniaj wszystkie swoje hasła
Powinniśmy teraz zadbać, aby wszystkie nasze hasła były wygenerowane w bezpieczny sposób przez samego LastPass'a. W tym celu musimy przejść na formularz zmianę hasła w jakimś wybranym portalu. W polu do wpisania hasła pojawi Nam się teraz dodatkowa ikonka po kliknięciu której możemy zdefiniować siłę hasła, a następnie kliknąć "*Fill Password*", które z automatu uzupełni wszystkie pola na hasło.

{{< img-nz "LastPass: wygeneruj nowe hasło" "lastpass.generate.png" >}}

Na powyższym zdjęciu widzimy jak LastPass generuje hasło o długości 37-miu znaków, składające się z zarówno wielkich oraz małych liter, jak również z liczb oraz symboli.

## Jaka długość hasła jest odpowiednia?
Zalecana długość hasła to 16 znaków [[1](https://www.security.org/how-secure-is-my-password/)][[2](https://www.lmgsecurity.com/how-long-should-your-password-be-a-technical-guide-to-a-safe-password-length-policy/)]. Natomiast osobiscie stosuje hasła o długości nawet 30-stu czy 40-stu znaków, no bo to dla mnie i tak bez różnicy skoro LastPass je pamięta za mnie.

Warto zwrócić uwage, że niektóre hasła będziemy musieli czasami (dość rzadko) **przepisać ręcznie**, np. przy logowaniu się do Google po kupnie nowego telefonu z Androidem.

# LastPass w telefonie
Oczywiście chcemy też mieć możliwość używania naszych haseł nie tylko na laptopie, ale również na telefonie. W tym celu LastPass stworzył aplikację pod Androida ([link](https://play.google.com/store/apps/details?id=com.lastpass.lpandroid)) oraz iOS'a ([link](https://itunes.apple.com/us/app/lastpass-for-premium-customers/id324613447?mt=8&uo=4)). Po ściągnięciu musimy się oczywiście zalogować oraz skonfigurować aplikację tak, aby podpowiadała nam odpowiednie hasła podczas normalnego użytkowania telefonu. Włączyć tę funkcję można poprzez wejście do ustawień, czyli "*Settings*", nastepnie "*Advanced*" oraz włączyć opcję "*Enable LastPass input method*". Gdy pojawi się okienko z informacją klikamy na nim "*OK*", po czym będziemy przekierowani do ustawień samego Androida w których musimy znaleźć ustawienia klawiatury i wybrać tam LastPass'a.

#### LastPass nie podpowiada mi haseł w telefonie..
Jeśli tak się stanie to zawsze można wejść bezpośrednio do aplikacji LastPass'a, zalogować się, znaleźć odpowiednie hasło w swoim sejfie, kliknąć w nie oraz wybrać opcję "*Copy Password*", która skopiuje hasło do schowka, więc będziemy mogli je następnie wkleić w odpowiednie miejsce.

## Drugi składnik autentykacyjny
Na tym etapie zakładamy, że nasze hasła są wygenerowane i przechowywane przez LastPass'a, co już jest całkiem dobre z punktu widzenia bezpieczeństwa. Natomiast, jeśli chcemy być bezpieczni to powinniśmy zadbać o jeszcze jedną rzecz: *drugi składnik autentykacyjny*.

Gdy po zalogowaniu dostajemy dodatkowy kod SMS'em, który musimy podać w aplikacji - to właśnie jest drugi składnik. Dodatkowe, krótkie losowe hasło. Jest to na tyle istotna kwestia, że poleca ją sama Unia Europejska w dyrektywie [2015/2366/EU, artykuł 4](https://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=CELEX:32015L2366).

Natomiast problem stanowi.. SMS. Abyśmy mogli przepisać taki kod z SMS'a musimy go najpierw dostać, a to oznacza dodatkowe medium od którego jesteśmy uzależnieni. Medium, które jest na tyle niezpieczne, że [już je wykorzystano](https://www.nytimes.com/2019/09/05/technology/sim-swap-jack-dorsey-hack.html), aby przejąć konto na Twitterze od jego właściciela [Jacka Dorsey'a](https://pl.wikipedia.org/wiki/Jack_Dorsey).

Znacznie lepszą alternatywą byłoby samemu wygenerować taki tymczasowy kod i właśnie do teog namawia Dyrektor ds. Bezpieczeństwa Tożsamości Microsoft'u, Alex Weinert, na [oficjalnych stronach Microsoftu](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/it-s-time-to-hang-up-on-phone-transports-for-authentication/ba-p/1751752).

### Zainstaluj LastPass Authenticator w telefonie

LastPass wesprze Nas i w tej kwestii dzięki swojej aplikacji **LastPass Authenticator**, która oczywiście jest również dostępna na [Androida](https://play.google.com/store/apps/details?id=com.lastpass.authenticator&hl=en_US&gl=US) oraz [iOS'a](https://apps.apple.com/us/app/lastpass-authenticator/id1079110004). Aplikacja te nie tylko będzie generować tymczasowe hasła, ale też zapisze parametry użyte do ich stworzenia w Twoim sejfie LastPass'a, a więc wszystko będzie w jednym miejscu.

Warto podkreślić, że generowanie takich kodów (tzw. TOTP, czyli [Time-based One-Time Password](https://en.wikipedia.org/wiki/Time-based_One-Time_Password)) nie wymaga żadnego połączenia: ani z internetem, ani siecią GSM. Kody są w 100% generowane na Twoim telefonie.

### Skonfiguruj drugi składnik autentykacyjny
Niestety ustawienia każdego portalu delikatnie się od siebie różnią, więc nie ma jednego przewodnika konfigurowania drugiego składnika autentykacyjnego dla każdego. Powinno to natomiast być dość intuicyjne. Warto pamiętać, że drugi składnik można skrótowo opisać jako "**2FA**", "**MFA**", więc można szukać tego ustawienia między innymi pod takimi właśnie nazwami. Gdy już dojdziemy do takiego ustawienia musimy go włączyć, a wtedy wyświetli się [QR kod](https://pl.wikipedia.org/wiki/Kod_QR) wyglądający podobnie do tego:

{{< img-nz "Kod QR" "qr.code.png" >}}

Teraz zostało Nam jedynie zeskanować ten kod aparatem w telefonie poprzez aplikację LastPass Authenticator. Gdy ją włączymy to na prawym, dolnym rogu będzie przycisk plusa "+" i po jego kliknięciu uruchomi się aparat, który musimy "nacelować" na obrazek z QR kodem i gotowe.

{{< img-nz "LastPass Authenticator" "lastpass.authenticator.png" >}}

Zdjęcię wzięte z [Apple Store](https://apps.apple.com/us/app/lastpass-authenticator/id1079110004)

Od teraz za każdym razem jak dany portal będzie Cię prosił o jednorazowy klucz możesz go pobrać bezpośrednio z tej aplikacji.