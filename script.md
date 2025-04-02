# Nie taki zardzewiały jak myślisz - odkryj potencjał Rusta

Katowice, 2025-04-03 12:00
Czas: 1 godzina

## Wprowadzenie (10 minut)

Cześć wszystkim, mam na imię Michał, i jestem studentem Informatyki na wydziale AEI w Gliwicach.

Od dziecka kocham programować i tworzyć wspaniałe rzeczy. Dodatkowo bardzo lubię być niezależny i mieć pełną kontrolę nad urządzeniami, na których pracuję, dlatego jak już pewnie zdążyliście zauważyć, używam na co dzień systemu Linux, jestem zapalonym fascynatem terminala i wszystkiego co z nim związane. Od wielu lat, hostuje na własnych serwerach i VPSach różne otwartźródłowe usługi, poczynając od prostych stron internetowych, przez serwisy do zarządzania dokumentami, aż po własny serwer poczty.

Jako student, jestem także członkiem Studenckiego Koła Naukowego Wirtualnego Latania vFly. Razem, tworzymy wspaniałe i ciekawe projekty, zaczynając symulatorów lotu, przez elektronikę, wirtualną rzeczywistość, aż po programowanie.

Dziś, korzystając z tej wspaniałej okazji, jaką są Dni Otwarte naszego wydziału AEI w Katowicach, chciałbym was zainteresować i zapalić programowaniem. Ale to nie będzie takie zwykłe programowanie jak w C, C++, Pythonie albo w Javie. Dziś opowiem wam o języku, który coraz bardziej zyskuje na popularności, posiada wiele ciekawych rozwiązań, jest bardzo przyjemny w użyciu, a także jest bardzo wydajny i bezpieczny. Mowa tu o języku Rust!

Na początku, chciałbym was zapytać, czy znacie ten język? Czy ktoś z was miał z nim do czynienia? Proszę, podnieście rękę, jeśli tak. (Czekam na reakcję publiczności)

Świetnie! Widzę, że niektórzy z was znają ten język, a niektórzy być może słyszeli o nim. Dla tych, którzy jeszcze go nie znają, postaram się w prosty sposób przybliżyć jego możliwości i zachęcić do nauki.

Ale na początek krótka anegdotka.

### Anegdota o nazwie "Rust"

Czy wiecie, że nazwa 'Rust' pochodzi od grzyba? Graydon Hoare, twórca języka, wybrał ją, (bo był ogromnym nerdem z biologii), ale chciał aby Rust był właśnie jak ten grzyb: odporny na bardzo nieprzyjazne warunki.

> <graydon> >> I love the name. I take it that it refers to your scavenging the
> <graydon> >> skeletal hulks of dead languages, now covered in vines...?
> <graydon> >
> <graydon> > A little. Also big metallic things. And rusts and smuts, fungi. And it's a
> <graydon> > nice substring of "robust".
> <jonanin> hah
> <jonanin> interesting
> <graydon> IOW I don't have a really good explanation. it seemed like a good name. (also a substring
>           of "trust", "frustrating", "rustic" and ... "thrust"?)
> <graydon> I think I named it after fungi. rusts are amazing creatures.
> <graydon> Five-lifecycle-phase heteroecious parasites. I mean, that's just _crazy_.
> <graydon> talk about over-engineered for survival
> <jonanin> what does that mean? :]
> <graydon> fungi are amazingly robust

W takim razie, powstaje pytanie, dlaczego Rust?

## Dlaczego Rust? (10 minut)

Rust jest językiem programowania zaprojektowany z myślą o bezpieczeństwie tego co piszemy, wydajności i szybkości programu, który tworzymy, oraz wygodzie dla programisty. Na przykład jak często zdarza się wam widzieć coś takiego?

### Bezpieczeństwo

Podczas pisania w C, musimy być ostrożni, pamiętać o wszystkich regułach, co zaalokowaliśmy, czy rozmiary, które zdefiniowaliśmy są odpowiednie, C++ pozwala nam na rozwiązanie tych problemów poprzez korzystanie z inteligentnych wzkaźników, lub innych specialnych struktur, ale jako że jest to język wstecznie kompatybilny, niestety musi bazować na starym paradygmacie programowania.

Dla porówniania, w Rust wiele rzeczy mamy zapewnione domyślnie, kompilator jest naszym przyjacielem, a błędy, które wywołują panic, są opisane przez co łatwo możemy znaleźć problem w naszym kodzie.

(Prezentacja slajdów)

Jeśli tylko minimalnie utrudnimy złożoność kodu, kompilator nie zauważy przepełnienia bufora i nie ostrzeże nas o tym. To może spowodować wiele nieprzewidzianych problemów i błędów. A nikt z nas raczej nie przepada za debuggowaniem aplikacji o 4:00 rano, prawda?

Krótko jeszcze przedstawię także inne przykłady, związane z Rustem.

Ownership - każda dana ma swojego właściciela, który odpowiada za jej zwolnienie. Nie możemy mieć dwóch właścicieli tej samej danej, co zapobiega wielu problemom związanym z zarządzaniem pamięcią, tj. przepełnienie bufora, dangling pointer, double free, use after free.

Borrowing - możemy pożyczać dane, ale tylko na czas, w którym ich używamy. Kompilator dba o to, aby nie było konfliktów między różnymi właścicielami danych.

Brak null pointerów - w Rust nie ma wskaźników null, co eliminuje wiele problemów związanych z dereferencją wskaźników. Zamiast tego mamy typ Option, który może być None lub Some(value). Dzięki temu możemy łatwo sprawdzić, czy dany wskaźnik jest pusty, czy nie.

### Wydajność vs Wygoda

Rust jest językiem nie oszczędzający na swoich możliwościach. Brak garbage collectora, oraz jego system typów sprawia, że Rust jest bardzo wydajny. Kompilator optymalizuje kod do poziomu C/C++, a często nawet nieco szybszego od C, jednocześnie nie wymaga od nas implementacji skomplikowanych struktur danych, które są trudne do zrozumienia i użycia.

Porównanie prędkości Rusta do C++ i innych;

Dodatkowo Rust oferuje wiele wygodnych rozwiązań, takich jak:
- Wbudowane makra, które pozwalają na generowanie kodu w czasie kompilacji
- Wbudowane testy jednostkowe, które pozwalają na łatwe testowanie kodu
- Wbudowane dokumentowanie kodu, które pozwala na łatwe generowanie dokumentacji
- Wbudowane narzędzia do analizy kodu, które pozwalają na łatwe wykrywanie błędów i problemów w kodzie
- Wbudowane narzędzia do zarządzania zależnościami, które pozwalają na łatwe zarządzanie bibliotekami i pakietami
- Wbudowane narzędzia do zarządzania wersjami, które pozwalają na łatwe zarządzanie wersjami kodu
- Wbudowane narzędzia do zarządzania projektami, które pozwalają na łatwe zarządzanie projektami i ich strukturą
- Funkcje wysokopoziomowe, które pozwalają na łatwe pisanie kodu w stylu funkcyjnym
- Statements i Expressions - w Rust wszystko jest wyrażeniem, co pozwala na łatwe pisanie kodu w stylu funkcyjnym
- Iteratory - w Rust mamy wiele wbudowanych iteratorów, które pozwalają na łatwe iterowanie po kolekcjach danych
- Opcje - w Rust mamy wiele wbudowanych opcji, które pozwalają na łatwe zarządzanie danymi i ich typami
- Struktury i enumy - w Rust mamy wiele wbudowanych struktur i enumów, które pozwalają na łatwe zarządzanie danymi i ich typami. Dodatkowo, precyzowanie danych w enumach pozwala na bezpieczeństwo, że nie pomylimy się w typach danych, które przekazujemy do funkcji.
- Asynchroniczność - dobrze stworzona asynchroniczność, która pozwala na łatwe pisanie kodu asynchronicznego i równoległego. Dla porównania z JavaScriptem, tutaj bardziej intuicyjnie await jest stawiany jako kolejny łańcuch, a nie jako osobny blok kodu.
- Przyjazny kompilator - kompilator Rusta jest bardzo przyjazny dla programisty, a jego komunikaty o błędach są bardzo pomocne i zrozumiałe. Dzięki temu łatwiej jest znaleźć i naprawić błędy w kodzie.

### Ekosystem

Rozwinięty ekosystem bibliotek i narzędzi, które pozwalają na łatwe pisanie kodu w Rust. Wiele popularnych bibliotek i narzędzi jest dostępnych w Rust. Wszystko znajdziemy na crates.io, czyli oficjalnym repozytorium bibliotek i narzędzi w Rust. Możemy tam znaleźć wiele popularnych bibliotek, takich jak Serde, Tokio, Actix, Diesel, Rocket i wiele innych.

Dodanie biblioteki lub instalacja programu z crates.io jest równie prosta jak dodanie do pliku Cargo.toml lub wykorzystanie komend cargo add i cargo install

clippy - narzędzie do analizy kodu, które pozwala na łatwe wykrywanie błędów i problemów w kodzie. Dodatkowo dodaje wiele przydatnych wskazówek i sugestii dotyczących poprawy jakości pisanego kodu.

cargo fmt - narzędzie do formatowania kodu, które pozwala na łatwe formatowanie kodu w Rust. Dzięki temu możemy łatwo utrzymać spójny styl kodu w całym projekcie.


## Wspaniałe oprogramowanie (10 minut)

Rust jest używany w wielu popularnych projektach i aplikacjach, takich jak:
- Wezterm - terminal napisany w Rust, który jest bardzo szybki i wydajny. Posiada wiele przydatnych funkcji, takich jak wsparcie dla GPU i wiele zakładek.
- Zellij - multiplekser terminala napisany w Rust, który pozwala na łatwe zarządzanie wieloma terminalami w jednym oknie.
- ncspot - odtwarzacz muzyki napisany w Rust, który pozwala na łatwe odtwarzanie muzyki z serwisu Spotify.
- ripgrep - narzędzie do przeszukiwania plików, które jest bardzo szybkie i wydajne.
- rmk - alternatywa do qmk, firmaware do klawiatur mechanicznych, który pozwala na łatwe programowanie klawiatur mechanicznych.
- MartyPC - cross-platformowy emulator PC, który pozwala na uruchamianie gier i aplikacji z architektury IBM PC.
- ruffle - emulator Flash, który pozwala na uruchamianie gier i aplikacji napisanych w technologii Flash.
- Helix - edytor tekstu napisany w Rust, alternatywa do Vima.
- Zed - edytor tekstu, alternatywa do Visual Studio Code.
- Ratatui - biblioteka do tworzenia aplikacji terminalowych w Rust, która pozwala na łatwe tworzenie aplikacji z interfejsem graficznym w terminalu.

Po więcej wspaniałego oprogramowania zapraszam na repozytorium awesome-rust, które zawiera wiele ciekawych projektów i aplikacji napisanych w Rust. Znajdziecie tam wiele różnych kategorii, takich jak web development, systemy operacyjne, gry, narzędzia i wiele innych.

## Jak zacząć? (10 minut)

Jeśli chcecie zacząć przygodę z Rustem, polecam wam kilka rzeczy:
- Zainstalujcie Rust, korzystając z oficjalnej strony https://www.rust-lang.org/tools/install. Możecie także skorzystać z menedżera pakietów, takiego jak Homebrew, APT, DNF, Pacman lub Chocolatey.
- Przeczytajcie dokumentację, która jest bardzo dobrze napisana i zawiera wiele przykładów. Znajdziecie ją na stronie https://doc.rust-lang.org/book/.
- Zainstalujcie edytor kodu, który wspiera Rust. Polecam Visual Studio Code z dodatkiem Rust Analyzer, który oferuje wiele przydatnych funkcji, takich jak autouzupełnianie kodu, podpowiedzi i wiele innych.
- Dołączcie do społeczności Rust, która jest bardzo pomocna i przyjazna. Możecie znaleźć wiele grup na Facebooku, Discordzie, Redditcie i innych platformach społecznościowych.
- Pracujcie nad projektami, które was interesują. Możecie znaleźć wiele projektów open source w Rust, które możecie wspierać lub rozwijać. Możecie także stworzyć własny projekt i podzielić się nim z innymi.
- Rustlings

## Podsumowanie (10 minut)

## Pytania i odpowiedzi (10 minut)

Dziękuję wam wszystkim za uwagę. Mam nadzieję, że udało mi się was zainteresować językiem Rust i zachęcić do jego nauki. Jeśli macie jakieś pytania, chętnie na nie teraz odpowiem. 

(Czekam na pytania publiczności)

Możecie także znaleźć mnie na GitHubie, gdzie znajdziecie moje projekty oraz inne ciekawe rzeczy. Zachęcam was do eksploracji tego języka i odkrywania jego potencjału. Dziękuję!
