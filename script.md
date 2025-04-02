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

### Ekosystem

## Wspaniałe oprogramowanie (10 minut)

## Jak zacząć? (10 minut)

## Podsumowanie (10 minut)

## Pytania i odpowiedzi (10 minut)

Dziękuję wam wszystkim za uwagę. Mam nadzieję, że udało mi się was zainteresować językiem Rust i zachęcić do jego nauki. Jeśli macie jakieś pytania, chętnie na nie teraz odpowiem. 

(Czekam na pytania publiczności)

Możecie także znaleźć mnie na GitHubie, gdzie znajdziecie moje projekty oraz inne ciekawe rzeczy. Zachęcam was do eksploracji tego języka i odkrywania jego potencjału. Dziękuję!
