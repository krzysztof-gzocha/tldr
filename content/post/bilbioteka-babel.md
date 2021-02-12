---
title: "Bilbioteka Babel"
date: 2021-02-12T11:25:56+01:00
draft: false
tags: [babel, algorytm, ciekawostka]
---

W 1941 roku Argentyński autor, tłumacz i poeta - [Jorge Francisco Isidoro Luis Borges Acevedo](https://pl.wikipedia.org/wiki/Jorge_Luis_Borges) - wydał krótką opowieść fantasy pod tytułem "Biblioteka Babel". Czy możemy dalej traktować tę opowieść jako fantasy?<!--more-->

# O czym jest ta opowieść?

> "Dzięki tej sztuce możesz kontemplować wariacje 23 liter..."

Opowieść mówi o sferycznym wszechświecie nazywanym Biblioteką, który składa się z bliżej nieokreślonej (i przypuszczalnie nieskończonej) liczby sześciokątnych (heksagonalnych) galerii. Na 2 ścianach każdej galerii jest korytarz do kolejnych galerii, a na pozostałych 4 ścianach jest po 20 półek, po 32 książki na każdej półce, każda książka składa się z 410 stron, każda strona z 40 linii, a każda linia z 80 czarnych znaków. Z każdej galerii widać również galerie znajdujące się bezpośrednio nad nią oraz pod nią. Wszystkie książki mają taki sam format oraz krój czcionki.

{{< img-nz "Biblioteka Babel: Galeria" "babel.galeria.png" >}}

Dodatkowo każda książka ma litery na grzbiecie, ale nie definiują one zawartości książki, a raczej są czymś w rodzaju "adresu" danej książki. Czymś co identyfikuje jej miejsce w bibliotece. Dana książka może się znajdować tylko na jednym, wyznaczonym dla siebie miejscu.
Cała zawartość każdej z książek skłąda się z 25 znaków: 22 małych liter alfabetu, odstępu ("spacji"), kropki oraz przecinka.

> Na każdy sensowny wers prostego stwierdzenia przypadają tysiące bezsensownych kakofonii, słownego bałaganu oraz niespójności. [..] Ludzie sprzeczali się w jakim języku są napisane. Portugalski? Yiidish? [..] Litewski? Arabski?

W całej bibliotece nie ma dwóch identycznych książek, ale istnieją całe tysiące różniące się jedynie kropką lub przecinkiem.

{{< img-nz "Biblioteka Babel: Galeria" "babel.strona.png" >}}

To oznacza, że "biblioteka" jest w 100% kompletna, czyli zawiera wszystkie możliwe wariacje 25 znaków jakie zmieszczą się na każdą ze stron, a to niesie ze sobą całkiem ciekawe konsekwencje. W słowach autora: (Tłumaczone na angielski przez James E. Irby)
> [..] the Library is total and that its shelves register all the possible combinations of the twenty-odd orthographical symbols (a number which, though extremely vast, is not infinite): Everything: the minutely detailed history of the future, the archangels’ autobiographies, the faithful catalogues of the Library, thousands and thousands of false catalogues, the demonstration of the fallacy of those catalogues, the demonstration of the fallacy of the true catalogue, the Gnostic gospel of Basilides, the commentary on that gospel, the commentary on the commentary on that gospel, the true story of your death, the translation of every book in all languages, the interpolations of every book in all books, the treatise that Bede could have written (and did not) about the mythology of the Saxons, the lost works of Tacitus.

Co można luźno przetłumaczyć na polski:
> Biblioteka jest kompletna i zawiera wszystkie możliwe kombinacje znaków, a więc zawiera całą historię świata zapisaną co do minuty, tysiące fałszywych katalogów, dowód błędu tych katalogów, "Gnostyczną ewangelię Bazylidesa", komentarz do tej ewangelii, komentarz do komentarza do tej ewenagelii, prawdziwą historię Twojej śmierci, tłumaczenie każdej książki na każdy język, interpretacje każdej książki, utracone prace Tacyta.

Wyobraź sobie bibliotekę w której jest dosłownie wszystko, cała historia Twojego życia, zapisany los ludzi, ziemi i kosmosu. Twoja pierwsza miłość, opis nauczyciela z matematyki, odpowiedź na pytanie o sens życia - na prawdę wszystko. 

> Odkąd poznałeś alfabet cała wiedza wszechświata jest tylko remixem tego co już znasz. (Autor nieznany)

# Czy to na pewno fantasy?

Stworzenie tak opisanej biblioteki w fizycznym świecie jest praktycznie niewykonalne.. a w świecie cyfrowym?

Istnieją [algorytmy](https://stackoverflow.com/questions/127704/algorithm-to-return-all-combinations-of-k-elements-from-n/127856#127856), które są w stanie wygenerować wszystkie kombinacje N-elementowego zbioru. Natomiast, wygenerowanie takiego zbioru i przechowanie go byłoby trudne nawet dla nowoczesnych technologii.

Możemy natomiast stwierdzić, że użycie algorytmu X do generowania takich kombinacji spowoduje, że na stronie Y w książce Z będzie tekst "MCV" i w skrócie taką właśnie wiedzę wykorzystał [Jonathan Basile](https://jonathanbasile.info) tworząc współczesną bibliotekę Babel. Według autora jego biblioteka aktualnie obejmuje około 10 do potęgi 4677 książek.

Stworzył on stronę internetową dzięki której możemy się przejść przez wirtualną bibliotekę, wejść do odpowiedniej galerii, wybrać odpowiednią ścianę, potem półkę, potem książkę i w końcu stronę, a wtedy strona pokaże Nam całą zawartość takiej strony.

Oczywiście poruszanie się wśród tak olbrzymiej ilości książek jest niepraktyczne, więc autor zaimplementował coś o czym Jorge Borges nie pomyślał, czyli **automatyczne szukanie strony na której znaduje się zadany przez gościa tekst**. A to znaczy, że jeśli chcesz to możesz znaleźć książkę i konkretną stronę, która mówi o tym jak cudowne jest Twoje dziecko, jak straszny jest Twój szef, jaka była pogoda, gdy się urodziłeś czy absolutnie cokolwiek innego składającego się z liter, przecinka i kropki o długości do 3260 znaków. Formularz wyszukiwania zadanego tekstu w bibliotece Babel jest dostępny pod tym adresem: https://libraryofbabel.info/search.html

Przykładowo w galerii ("heksagonie") o nazwie:
```
01hfp23y0xaed3qf1a2fgh2lk0rroaurrbye5tp9mev9d77hpbmiqen0epirkdwr3k37rcc797qska2p5xas735vt5ksjnf3kv9ka2mh1l60jwn9jry6eol3b9pq5hqrutrukk5s5udik0esavfiy7tvjcy1g7a6bfcpf57l7bgtsebsb168bmyo3rxzscvy3jo6svtnbbrllw69pvve1wtcsb1644917o3vf5zyubo6xsoo7zwbcounzzm9ceh570gjh9ik5chfh1sbfb98hiercnzm2s30ffzjilcvyi60drfqj8d88x197xxevlzfioq4bvrthw940bkpjiuuserb3oa1z4k296d7fxqos697n4f8xdm9zgjlf1lhc16qgffoosldd883yih80gy0zxoklcs35snw53a65bbqenne247frlzcf5yw3s3e1x7t21fffsj053pt5ichh13s0ue6vnvd7hcsy7aoz3cq2jziv8qvm3e0kavqj2tc102nd7aq1u5h31rwqaxc0ogp4yr8n2kckmad35x6ga946l0ryzlfnglzmcdudltfq5levoaxattd6vvesyx2rv7i5d4z1udxj2achmbgxp4yt992033vpxtp42ld48lzz5r9q3gs5lvex5brv2605aqdwm1kz8xyedqmb3ar5z8evhvjsrabqybbdqkmnni4y58xxamkk9ll1x5uinizst0dioeio8ebctuwnemi1sq14d9s7ncj4qiadn3dzot3lwgu1kfk1whmhxy89y4zlt6nci4ui5sfv4u1a9z848q94yx7kymhkywka69eh5xb8p1phcexxwuwo71cah9vug0qaapu3yttq8bnvtu7rsfftqhdcoysvfg4v2uz8u80zs0h7vkbrzhnblm2gi0ijfnke7va96n8upngvrqj7vaoha01cldjfr0mcosrf5u2aoiz6zwcttvj6odg493ncs66kefp7odqlw3f2ca09k146e1uifd7sozf6vg5s3n2codl95xla82ahionnjz56wdbz546py20tqkkz2y8ftkfh1pah7mg4c478f450ng8su9e2cavp0tgjzli09t5zk7quzyqxrtt135vxma931cea2azssb962rt6o8r7n1j66cvl7e4vq6ilzecy7uuzigcx44h240m5av6r76ar7nhwnz0u7apkl9phxlw327h3hzzwwsu5hvi2li5talwag8td0gm2i36lpabus1ann50ix6pyvmyjfrp55hjk34e8nsbmvgfvbu4q8j7jb8zaxcl3uhouaupaw75so5perddgcgjjwkwa6dhi7kd3lbjvg3t5pf7wmc6565mtyu3sh9qbke6x74fj977ozo41xk102n1bd0tfxvz2mmbukvl2sikshp71180qu8cg9j3mw1vqy6iv2j92n3iiy8ly1xw96gxnvtlzuyzw278i8et16gkxcra1fygf5khk25wultau9ylachwd5i6gbkdgj8xwdkzifttymsz58fwgjm3jbc67cajoz6f4ezl0pjfnjpcz5n4xn771us2dpw5emdd0za9vqhlyzca16cbaykeenjiljobywkz6txafwbpns0vcp9b2ivxgp3qrj6orr6z6a4z8w9zee4beuo4vn6klg3y71oh55ajjeirlttc0cccdpbvxxys3nqkgj61hkz07ck6uctjuo1lyy9zbsxc9n7irygo74sbz41a9vz1vh0p2zkcn9nj5saf9v9p56me5hty7xjupy29tgqtah6lpe76v9jm5bivoxvvs129ochnkzkzgd5klkvp7464k1442qol5kqeq2mr3w6q4bo2m6tggm6qyub6v1mwc6ssvmezrt8i2ntqwfd8oqnpltcbtsyo6h532ginkhy0y67610k2k8lzkj9ne4jpsr5wv6n6epeh69di0909zz04q1wknf1g5pns95z52tyce4cuuf5zvtb8xu8ixoavaooezpp3ew2udqgq182bhcoyhd863hq1tvb1xbtae5sgd2f7yq7s56g4mzgoifip7cql3ziijj3fzlrn2rb94yi532ritu7a5040qof68ywnjt8ql5x5ivo9gu0kf9qt10x2d9m5dj8aanrwkjlt6ckwyn115jxdk9axpjivkj3cdanvwlweswiic4cts3s0y4jz25adhavmld828vf0ci7xuwmd5xmht22kavb7zv55mc1t0ljr8nwwkzoyskzmrc38cjk1eeo51e4iauint5h57f31p1rnoia8jafcgwlermsws4ia4a5fz1vuy2dkiazj5lfp5pd5u7wus4bvcevvhc2b94optawy4ewlvnnqiepby85msiu41m135trlaa3vx5g3r4elov2vrdhf1l9ik7kx975w9sgjzi3wels4qf23q2gvkqbpyemx2hqcs7lb03p3cejylbwq1ucrp7eosyep7svwf4at2ikg2cr5m894eox7nj9ky63cdm6lvstyzxj516fm4xcupel8dbdbwih33bvf3tju6om185rtqyh3ubp5a2qccegl7ny61jbo2gz2s4vvrymux0cqqsemg8yhssvvlrq35biq57zueiecokh4egch410d9mqf5bq0c19hge5fadmhwcvzakzjzv2whgzy4xdmwll920lww26swrmsu7pdy8l8e69cf17ojghi1554sfu2lot6q7dnb3a0rw7pdrfq8vwtt102f8l9diumofc9whobht8upwoyrmvensi63gwlym9w51begbz30anw3w7lqnxxtxx34n0qs99m2ynjvwumntrfvccc4nhb2nkptaajagumg8eqfi7d71ww5y0hq75v35fwuzopw86b6htjna7ydvvhks1svyrr3yhvn8macq0vguzeivpox814mgxtianth4v99t8vo87d6my4dbv73vrmqxdkroghs9zf801k142z9uekmedhafuvei5xkzuon2lkc7kg09j00hjhqfgp33uhqh6g7aeg23isyjyked85xiv4offcdorn7lb3z2mbw6dxn59h6cy2vnwf9i8deh6gfc3mmtdlk6043njkoig83u0lf33yeyfeiebovh9ysqbi1f3xeaw68s6lnfaix77eu7n49pllu4ci35np780eybhlquudp6h1edlyc3jgcdai26152gznlccadttphmuq3jrgizdqru24qjbaic4xr50cgjne0artuurc4hs7t
```
na trzeciej ścianie, na pierwszej półce, w książce numer 3 jest strona 35 składająca się z tekstu, który chciałem wyszukać oraz samych spacji.

Czy więc opowieść Jorge'a Borges'a można wciąż uznać w pełni za fantasy?

{{< img-nz "Babel: dziekuje" "babel.dziekuje.png" >}}

## Linki
- Tłumaczenie opowieści na angielski: https://jonathanbasile.info/libraryofbabel.html
- Tłumaczenie w wersji PDF'a ściągniete z wyżej wymienionej strony: [Biblioteka Babel.pdf](../../babel.pdf)
- Cyfrowe odtworzenie biblioteki Babel: https://libraryofbabel.info