# phd_thesis
PhD thesis in LateX

__Author__: Michal Dyzma

__Title:__ Modelowanie oscylacji stężeń jonów wapniowych w komórkach eukariotycznych z uwzględnieniem obszarów bezpośredniego kontaktu pomiędzy mitochondriami a~retikulum endoplazmatycznym.

__Abstract:__

Przedmiotem pracy jest analiza wpływu obszarów bliskiego kontaktu pomiędzy retikulum endoplazmatycznym (ER) a mitochondriami na homeostazę wapniową w komórce. Obszary te odkryto już w latach 70-tych, jednak dopiero niedawno zostały intensywnie zbadane. Ponieważ znajdują się one na granicy mitochondria-retikulum, określa się je jako ,,mitochondria-associated ER membrane complexes'', a w literaturze naukowej stosowana jest w stosunku do nich skrótowa nazwa MAM. Badania za pomocą mikroskopii elektronowej, FRET i metod genetycznych pozwoliły na dokładne określenie struktury fizycznej oraz zidentyfikowanie komponent tworzących MAM. Odległość między błonami odgraniczającymi w powyższym kompleksie waha się od 10 - 25 nm tworząc fizyczne połączenia przypominające synapsy, umożliwiające szybsze przekazywanie jonów wapnia z ER do mitochondriów i odwrotnie. Interfejs mitochondrialno-retikularny stabilizowany jest przez szereg protein, które w większości powiązane są z głównymi elementami przewodzącymi sygnał wapniowy w tych kompartmentach, tj. receptorem IP$_3$R, pompą wapniową SERCA oraz kanałem VDAC. Szacuje się, że w 80\% przepływu jonów wapniowych pomiędzy mitochondrium a retikulum, odbywający się pośrednio przez cytozol, zachodzi poprzez obszary typu MAM. W Polsce badania nad strukturami MAM prowadzone są w Instytucie Biologii Doświadczalnej im. Nenckiego PAN przez Prof. Mariusza Więckowskiego z Pracowni Bioenergetyki i Błon Biologicznych.


Ze względu na wspomniana powyżej bezpośrednią bliskość retikulum endoplazmatycznego i mitochondriów, kompleksy MAM spełniają niezwykle ważną rolę w homeostazie i dynamice wapnia w komórce. Ułatwiony przepływ wapnia pomiędzy powyższymi kompartmentami komórkowymi może wpływać istotnie np. na oscylacje stężenia wolnych jonów wapnia w poszczególnych częściach komórki. Oscylacje takie są niezbędne do prawidłowego funkcjonowania komórki. Odpowiedzialne są m.in. za szereg istotnych procesów fizjologicznych takich jak kontrola cyklu komórkowego, skurcz mięśni szkieletowych, wzmocnienie synaptyczne. Stabilne oscylacje wapniowe stanowią istotny czynnik będący częścią sieci sygnałowej, który sprawdza czy komórka jest w dobrej kondycji i utrzymujący ją przy życiu. Cykliczne wahanie poziomu wapnia w~mitochondriach (stabilny cykl graniczny) powoduje aktywację dehydrogenaz poprzez allosteryczne związanie jonów Ca$^{2+}$ i wzrost produkcji ATP. Zatem z  jednej strony lokalne w czasie i przestrzeni zmiany stężenia wolnego wapnia cytozolicznego są jednym ze sposobów przenoszenia informacji w komórce i inicjacji szeregu ścieżek sygnałowych będących odpowiedzią na zmieniające się warunki zewnętrzne, z drugiej zaś zbyt wysokie stężenie wolnych jonów wapnia w cytozolu jest bardzo szkodliwe i może doprowadzić do śmierci komórki. (Wiadomo np., że wapń jest jednym z kilku czynników zapoczątkowujących apoptopzę – kontrolowaną śmierć komórki). W istocie, badanie wpływu kompleksów MAM na dynamikę wapnia w komórce należałoby przeprowadzić na gruncie modelu przestrzennego opisywanego układem równań różniczkowych cząstkowych przy uwzględnieniu informacji dotyczących  rozmieszczenia i rozmiarów zbiorników retikularnych i mitochondrialnych w komórce. Zadanie takie jest jednak bardzo skomplikowane, zarówno z teoretycznego, jak i numerycznego punktu widzenia. Co więcej, dla tego typu układów, ze skomplikowaną geometrią i olbrzymia ilością podobszarów i nieliniowymi przepływami miedzy nimi, bardzo rzadko daje się znaleźć  (numerycznie) rozwiązanie opisujące oscylacje w czasie (i przestrzeni). W swoich rozważaniach zdecydowałem się zatem na pozostaniu w ramach tzw. modeli całokomórkowych (,,whole cell models''), które abstrahują od przestrzennego rozkładu retikulum i mitochondriów wewnątrz komórki i analizują jedynie zależność od czasu stężenia wolnego wapnia uśrednionych przestrzennie po odpowiedniej składowej kompartmentalnej (cytozolicznej, retikularnej i mitochondrialnej) przy założeniu dostatecznie szybkiej dyfuzji wapnia. W tym podejściu opis zmienności czasowej wapnia dany jest układem nieliniowych równań różniczkowych zwyczajnych. Ponieważ dokonujemy przestrzennego uśrednienia stężenia, uwzględnienia istnienia kompleksów MAM dokonujemy poprzez wprowadzenie dodatkowego bezpośredniego przepływu wapnia pomiędzy retikulum a mitochondriami. (W modelach całokomórkowych nie biorących pod uwagę  istnienia obszarów MAM, przepływ pomiędzy tymi kompartymentami ,,odbywa się'' pośrednio przez cytozol.).

Punktem wyjścia do budowy nowego modelu był model zaproponowanym przez Marhla i współpracowników z roku 2001. Jest to jeden z nielicznych modeli, który uwzględnia aktywny wpływ mitochondriów na dynamikę sygnału wapniowego w komórce i nie traktował ich jedynie jak ,,olbrzymich'' cząsteczek buforujących (tzn. przyłączających jony wapnia). W ,,nowym'' modelu uwzględniono również właściwości białka transportującego wapń do wnętrza mitochondrium – uniportera mitochondrialnego -  który w warunkach ekspozycji na submilimolowe stężenie wapnia aktywuje tzw. szybki mechanizm pobierania jonów wapniowych RaM (ang. \textit{\textbf{ra}pid uptake \textbf{m}ode}). Doświadczenia przeprowadzone przez Guntera i współpracowników oraz Vinogradova sugerują, że w tych warunkach mitochondria pobierają wapń znacznie wydajniej. Przepływ do mitochondriom składa się zatem z dwóch części. Pierwsza z nich uwzględnia wspomniany powyżej szybki mod RaMowy, druga opisuje prace uniportera mitochondrialnego w trybie standardowym.

Zaproponowany  układ równań różniczkowych zwyczajnych przy dowolnych nieujemnych dodatnich danych początkowych posiada globalne w czasie rozwiązanie różniczkowalne o nieujemnych składowych. Ilościowa analiza układu układu mogła być jednak przeprowadzona tylko za pomocą symulacji numerycznych, w oparciu o procedury platformy MATLAB oraz  programu MATCONT. 
Dla szerokiego zestawu parametrów charakteryzujących przepływy miedzykompartmentowe, rozwiązania układu maja charakter oscylacyjny. W ramach przedstawionego powyżej  modelu zbadano  wpływ parametru kMAM  regulującego przepływ w kompleksach MAM na okres oscylacji, istnienie rozwiązań chaotycznych oraz  baseny przyciągania rozwiązania okresowego (cyklu granicznego). Wyznaczono zestawy parametrów, dla których istnieją różne typy oscylacji wapniowych: regularne, seryjne („bursting”) i chaotyczne. Okazało się, że wprowadzenie dodatkowego przepływu w kompleksach MAM sprawia, że  system zachowuje się jak układ bistabilny, w którym współwystępują dwa atraktory: stabilny cykl graniczny oraz stabilny punkt stacjonarny. Dla dostatecznie dużych wartości kMAM, większość trajektorii układu znajduje się w basenie przyciągania wspomnianego stabilnego punktu stacjonarnego.  Takie zachowanie się rozpatrywanego układu równań, może mieć ciekawą interpretację biologiczną. Stabilny punkt stacjonarny układu charakteryzuje się wysokim poziomem wapnia w mitochondriach. Jeśli zatem trajektoria układu znalazła się w basenie przyciągania tego punktu, może to oznaczać, że komórka weszła na ścieżkę apoptotyczną. Akumulacja wapnia w mitochondriach i pęcznienie mitochondriów występuje bowiem w początkowej fazie apotozy."
