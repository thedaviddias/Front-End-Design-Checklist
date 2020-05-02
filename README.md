![Front-End Design Checklist](/images/front-end-design-checklist-banner.jpg)
<h2 align="center">Checklista projektowania Frontend</h2>

<p align="center">
  <em> Checklista projektowania dla programistów Frontend to wyczerpująca lista elementów, które mogą pomóc programistom w analizie i zrozumieniu projektów internetowych oraz w zapewnieniu jakości ich rozwoju.</em>
</p>

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com) [![Join the chat at https://gitter.im/Front-End-Checklist/Front-End-Design-Checklist](https://badges.gitter.im/Front-End-Checklist/Front-End-Design-Checklist.svg)](https://gitter.im/Front-End-Checklist/Front-End-Design-Checklist) [![CC0](https://img.shields.io/badge/license-CC0-green.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

## Spis treści
* **[1. Wymagania projektowe](#1---wymagania-projektowe)**
	* [1.1 Grid system](#11---grid-system)
	* [1.2 Kolory](#12---kolory)
	* [1.3 Czcionki i teksty](#13---czcionki-i-teksty)
	* [1.4 Linki i nawigacja](#14---linki-i-nawigacja)
	* [1.5 Obrazy / Ikony](#15---obrazy--ikony)
	* [1.6 Formularze i przyciski](#16-formularze-i-przyciski)
	* [1.7 Responsywne projektowanie stron internetowych](#17---responsywne-projektowanie-stron-internetowych)
	* [1.8 Przewodnik po stylach i podejście do komponentów](#18---przewodnik-po-stylach-i-podejście-do-komponentów)
	* [1.9 Dostarczane pliki](#19---dostarczane-pliki)
* **[2. Analizy i etapy przygotowawcze](#2---analizy-i-etapy-przygotowawcze)**
	* [2.1 Analiza wersji papierowej](#21---analiza-wersji-papierowej)
	* [2.2 Faza przygotowawcza](#22---faza-przygotowawcza)
* **[3. Walidacja](#3---walidacja)**
* **[4. Faza rozwoju](#4---faza-rozwoju)**
* **[5. Przed produkcją](#5---przed-produkcją)**

---

> **Checklista projektowania dla programistów Frontend** to wyczerpująca lista elementów, które projektanci stron internetowych i programiści muszą wziąć pod uwagę, aby ułatwić sobie współpracę. Poniższe elementy stanowią połączenie znanych praktyk z nowymi elementami w oparciu o wieloletnie doświadczenie w analizowaniu projektów internetowych.

Jeśli szukasz listy wszystkich elementów, które musisz mieć/przetestować przed uruchomieniem witryny/strony HTML do produkcji, spójrz na → [Front-End Checklist](https://github.com/thedaviddias/Front-End-Checklist).


## Jak korzystać z Checklisty projektowania?

Kiedy przychodzi moment, w którym programiści odkrywają nowe projekty stron internetowych, zanim przekonwertują je na kod, może brakować niektórych ważnych elementów. Lista kontrolna projektowania Frontend to narzędzie dla programistów Frontend i projektantów stron internetowych, których celem jest pomoc im obu w płynnej pracy.

Możesz udostępnić tę listę kontrolną projektantom stron internetowych, aby zapewnić oszczędność czasu w czasie dostawy, lub możesz użyć jej do przejrzenia wszystkich elementów dostarczonych przez kreatywny zespół i upewnić się, że wszystko jest poprawne przed przystąpieniem do integracji kodu.


## Dlaczego powinieneś skorzystać z Checklisty projektowania?

* Upewnij się, że kreatywny zespół bierze pod uwagę wszystkie punkty
* Posiadanie dokumentu, na którym mogą polegać projektanci i programiści, aby zapewnić lepszą komunikację i spójność w interakcji.
* Ponieważ łatwo jest zapomnieć o niektórych ważnych elementach, gdy gonią cię krótkie terminy
* Unikanie odkrywania problemów, gdy kreatywny zespół już pracuje nad innym projektem.
* Aby pokazać komplementarną pracę między projektantem stron internetowych, a programistą Frontend

---

## 1. - Wymagania projektowe

Projektowanie strony internetowej lub aplikacji internetowej wymaga przestrzegania pewnych zasad i wzięcia pod uwagę, że projekt to nie tylko projekt graficzny, ale także projekt internetowy. Kolejne sekcje są kluczowe dla każdego projektu internetowego.

### 1.1 - Grid system

![Grid system](/images/grid-system.png)

* [ ] **Grid** jest wyraźnie określone w projekcie, a szczegóły siatki są zawarte w specyfikacji technicznej (szerokość, rynny, liczba kolumn…). Projektant stron internetowych może utrzymać siatkę w przezroczystej warstwie i używać jej we wszystkich swoich projektach.
	> ℹ️ [Guide Guide][6] to wtyczka do programu Photoshop, która może pomóc w łatwym budowaniu siatki.

	> ℹ️ W Sketch możesz używać zintegrowanego “[Make Grid Tool][7]” aby zaprojektować pożądaną siatkę.

* [ ] **Zapoznaj się z systemem siatki**, który będziesz używać w swoim projekcie. Przez większość czasu niektóre opcje (takie jak wyrównanie, przesunięcie, zagnieżdżanie…) są ignorowane przez programistę i zwykle są zastępowane przez ręczne wypełnianie lub marginesowane niepotrzebnie.
* [ ] Przed przystąpieniem do pracy nad każdym komponentem witryny możesz **budować wszystkie szablony** używane w creatives tylko z klasami siatki. Budowanie konstrukcji przede wszystkim ułatwi ci późniejszą pracę.

```html
<div class="container">
  <div class="row">
    <div class="col-sm">
      <!-- Najpierw opróżnij -->
    </div>
    <div class="col-sm">
      <!-- Najpierw opróżnij -->
    </div>
    <div class="col-sm">
      <!-- Najpierw opróżnij -->
    </div>
  </div>
</div>
```

⚠️ *Jeśli chcesz upewnić się, że siatka i szerokość urządzeń są przestrzegane, możesz wygenerować sobie szablon PSD i wysłać go do projektanta stron internetowych.*

__Dodatkowe materiały:__

* 🛠 [Bootstrap Grid System][8] (v4)
* 🛠 [Flexbox Grid][9]
* 📖 [Don't Overthink It Grids | CSS-Tricks][10]

**[⬆ powrót do góry](#spis-treści)**

### 1.2 - Kolory

![Colors](/images/colors.png)

* [ ] **Wszystkie kolory użyte w creatives są nazwane** ($gray-light, $gray-dark, $green) lub odpowiednio z ich użyciem
 ($body-background, $body-copy, $text-paragraph…). Można je wyeksportować w pliku [ACO][11] (jeśli korzystasz z Photoshopa lub na stronie symboli dla Sketch) i udostępniać programistom.

![Color Swatches](/images/color-swatches.jpg)

* [ ] Różny **stan kolorów** niektórych elementów (takich jak przyciski, odnośniki, wejścia...) są zdefiniowane i działają w kontekście jasnego lub ciemnego tła oraz jasnego lub ciemnego tekstu.

* [ ] Wszystkie lub najważniejsze/używane **kolory są dostępne** w projekcie, aby umożliwić płynną nawigację na stronie internetowej/aplikacji webowej.

__Dodatkowe materiały:__
* 🛠 [WCAG - Contrast Checker](https://contrastchecker.com/)
* 🛠 [Color Safe - accessible web color combinations](http://colorsafe.co/)
* 🛠 [Coolors.co - The super fast color schemes generator](https://coolors.co/)

**[⬆ powrót do góry](#spis-treści)**

### 1.3 - Czcionki i teksty

![Fonts](/images/fonts.png)

Czcionki są istotną częścią każdego projektu, nie należy ich wybierać bez rozeznania. Wybór niewłaściwej czcionki dla projektu może mieć skutki finansowe i prawne.

Zaleca się, aby poprosić klienta o zakup tych czcionek, aby uniknąć potencjalnych problemów w przyszłości i wziąć pod uwagę warunki użytkowania. Niektóre strony są ograniczone pod względem odsłon i nie mogą być hostowane ([Understanding Webfont Licensing Structures](https://aeolidia.com/understanding-webfont-licensing-structures/)).

* [ ] Dostarczono czcionki dla komputerów stacjonarnych (ogólnie TTF lub OTF) i stron internetowych, w formacie **WOFF, WOFF2 i TTF** (w pliku Zip lub dano dostęp do strony internetowej, na której zostały zakupione).
	> ℹ️ Format TTF dla desktopu nie jest taki sam jak format TTF dla webowych.

  __Materiały:__
	* 📖 [Using @font-face | CSS-Tricks](https://css-tricks.com/snippets/css/using-font-face/)
* [ ] [Fallback font](https://en.wikipedia.org/wiki/Fallback_font) zostały określone w dokumencie (najlepiej w Przewodniku po stylach) dla programisty Frontend.

  __Materiały:__
  * 📖 [CSS Basics: Fallback Font Stacks for More Robust Web Typography | CSS-Tricks](https://css-tricks.com/css-basics-fallback-font-stacks-robust-web-typography/)
  * [Create Your Own @font-face Kits » Font Squirrel](https://www.fontsquirrel.com/tools/webfont-generator)

* [ ] **Waga całkowita** wszystkich czcionek webfonts nie przekracza 1-2 Mb (wszystkie warianty zawierają: kursywę, pogrubienie itp.).

* [ ] W miarę możliwości **wszystkie teksty są dostarczane w odpowiednim języku** zamiast tekstów zastępczych w języku angielskim (Lorem Ipsum i podobne).

	> ℹ️ W przypadku wielojęzycznej strony internetowej zawsze zadaj sobie pytanie, jak projekt może zareagować, jeśli tekst jest dłuższy niż wcześniej zdefiniowany. Pamiętaj, że projektanci stron internetowych używają do tworzenia doskonałych projektów i nie zawsze myślą o możliwych problemach lub sytuacji ze zbyt dużą ilością tekstu.
	
__Dodatkowe materiały:__
* 📖 [Web Font Optimization  |  Web Fundamentals  |  Google Developers](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/webfont-optimization)
* [`font-display` for the Masses | CSS-Tricks](https://css-tricks.com/font-display-masses/)
* [Rhythm in Typography | improve legibility, readability, and visual hierarchy](https://betterwebtype.com/rhythm-in-web-typography)

**[⬆ powrót do góry](#spis-treści)**

### 1.4 - Linki i nawigacja

![Links and navigation](/images/links.png)

* [ ] Wszystkie **linki mają stan domyślny, najechanie kursorem, fokus, stan aktywny i odwiedzony** jasno określone (Przewodnik po stylu jest najlepszym dokumentem do ich określenia).
* [ ] Alternatywne widoki wszystkich stanów nawigacji (hover, aktywna/bieżąca strona).

### 1.5 - Obrazy / Ikony

![Images](/images/images.png)

* [ ] **Obraz favicon** z co najmniej 512px X 512px jest dostarczany w formacie PNG. Generowanie wszystkich innych Faviconów można łatwo zrobić za pomocą narzędzi online.

  __Materiały:__
  * [Favicon Generator for all platforms: iOS, Android, PC/Mac...](https://realfavicongenerator.net/)

* [ ] Wszystkie ikony dostarczone są w **formacie SVG**, każdy w tym samym kwadratowym wymiarze, w kolorze czarnym i w oddzielnym folderze.

  __Materiały:__
  * 🛠 [SVGOMG - SVGO's Missing GUI](https://jakearchibald.github.io/svgomg/)

* [ ] **Nazwa każdej ikony** rozpoczyna się od `icon-` i jest w całości pisana małymi literami (bez spacji i za pomocą myślników oddzielających każde słowo).

__Dodatkowe materiały:__
* 📖 [Essential Image Optimization](https://images.guide/)

**[⬆ powrót do góry](#spis-treści)**

### 1.6 Formularze i przyciski

![Forms](/images/forms.png)

* [ ] Wszystkie formularze posiadają tytuł, który można wykorzystać jako legendę
* [ ] Podano przykład **różnych stanów wszystkich pól wejściowych** (przynajmniej fokus i stan nieaktywny / wyłączony).
* [ ] **Wszystkie komunikaty o błędach** zostały dostarczone, tekst (ewentualnie w oddzielnym dokumencie) pozycja i kolor są wyraźnie widoczne w creatives i spójne. Niektóre komunikaty powinny się różnić w zależności od błędu.

  __Materiały:__
  * 📖 [Forms Need Validation – UX Collective](https://uxdesign.cc/forms-need-validation-2ecbccbacea1)
* [ ] Pola **indykatorów wymaganych/opcjonalnych** są dostarczone.
* [ ] **Główne i dodatkowe przyciski** są wyraźnie identyfikowalne i są stosowane zgodnie z powszechnymi praktykami.
  __Materiały:__
  * 📖 [Primary & Secondary Action Buttons – UX Planet](https://uxplanet.org/primary-secondary-action-buttons-c16df9b36150)
* [ ] Przykład **różnych stanów przycisku** podano (stan normalny, aktywowanie, skupienie, naciśnięcie i stan nieaktywny).
* [ ] Dostępne są przyciski z wbudowanymi **wskaźnikami ładowania**, które można zastosować do dowolnego przycisku.

__Dodatkowe materiały:__

* 📖 [Design Better Forms – UX Collective](https://uxdesign.cc/design-better-forms-96fadca0f49c)
* 📖 [Design Better Input Fields – UX Collective](https://uxdesign.cc/design-better-input-fields-3d02985a8e24)
* 📖 [Designing Perfect Text Field: Clarity, Accessibility and User Effort](https://uxplanet.org/designing-perfect-text-field-clarity-accessibility-and-user-effort-d03c1e26004b)
* 📖 [Button UX Design: Best Practices, Types and States – UX Planet](https://uxplanet.org/button-ux-design-best-practices-types-and-states-647cf4ae0fc6)
* 📖 [How To Design Better Buttons — Smashing Magazine](https://www.smashingmagazine.com/2016/11/a-quick-guide-for-designing-better-buttons/)
* 📖 [Buttons in Design Systems – EightShapes – Medium](https://medium.com/eightshapes-llc/buttons-in-design-systems-eac3acf7e23)

**[⬆ powrót do góry](#spis-treści)**

### 1.7 - Responsywne projektowanie stron internetowych

![Responsive](/images/responsive.png)

* [ ] **Wersja mobilna** projektu jest dostępna przed wersją komputerową lub w tym samym czasie.

	> Jeśli podejście “**mobile first**” nie było brane pod uwagę przez creative team, mogą wystąpić pewne nieprawidłowości i niespójności między wersją mobilną, a stacjonarną. Sprawdź i oznacz te problemy przed rozpoczęciem opracowywania projektu.
	* [ ] Należy również podać **wersję tabletu** projektu w niektórych przypadkach.

⚠️ *Pojęcie **pixel perfect** jest dziś w pewnym sensie przestarzałe. Dzisiaj nie można mieć projektu, który działałby tak samo w obliczu wielu rozmiarów ekranu.*

__Dodatkowe materiały:__

* 📖 [Official Google Webmaster Central Blog: Mobile-first Indexing](https://webmasters.googleblog.com/2016/11/mobile-first-indexing.html)

**[⬆ powrót do góry](#spis-treści)**

### 1.8 - Przewodnik po stylach i podejście do komponentów

![Styleguide](/images/styleguide.png)

* [ ] Wszystkie komponenty zaprojektowane na każdej stronie zostały utworzone za pomocą **component based approach**  (Atomic Design). Jeśli nie, mogą wystąpić problemy związane z wydajnością, utrzymaniem projektu...

  __Materiały:__
  * 📖 [Atomic design][16]
  * 📖 [6 Reasons for Component-Based UI Development](https://www.tandemseven.com/technology/6-reasons-component-based-ui-development/)

* [ ] Należy dostarczyć **Przewodnik po stylach** zawierający wszystkie elementy, komponenty, style i wymiary. Niektóre boilerplate'y, jak [UX Power Tools](https://www.uxpower.tools/) mogą pomóc zaoszczędzić czas i zachować spójność projektów.

⚠️ *W przypadku, gdy brakuje Przewodnika po stylu, dobrą praktyką jest zbudowanie sobie [living Style Guide](https://github.com/davidhund/styleguide-generators), aby ułatwić ci pracę. Na przykład niektóre CMS, takie jak Drupal, mają wtyczki, które pozwalają opracować aktualizowany przewodnik po stylach [Pattern Lab](https://drupal-pattern-lab.github.io/).*

__Dodatkowe materiały:__

* 📖 [Style Guides – Design + Sketch – Medium](https://medium.com/sketch-app-sources/tagged/style-guides)
* 📖 [The CodePen Design Patterns and Style Guide](https://codepen.io/guide)
* 📖 [Lonely Planet Travel Guides and Travel Information](http://rizzo.lonelyplanet.com/styleguide/design-elements/colours)
* 📖 [Styleguide](https://www.yelp.com/styleguide)

#### W przypadku istniejącego projektu:

Czasami creative team musi dodać nowe strony lub moduły do istniejącego projektu. Powinien mieć lub utworzyć listę wszystkich istniejących elementów i spróbować wykorzystać to, co już istnieje. Utworzenie Przewodnika stylu już może zaoszczędzić godziny i zapewnić spójność projektu.

**[⬆ powrót do góry](#spis-treści)**

### 1.9 - Dostarczane pliki

![Delivery files](/images/delivery-files.png)

* [ ] W przypadku wszystkich witryn projektant stron internetowych musi zapewnić co najmniej **2 PSD** (mobile, desktop i ewentualnie tablet) lub przynajmniej **1 Sketch file**, który musi zostać dostarczony z poniższym wymiarem (jeśli masz Photoshop CC 2015 i nowsze wersje, zalecam używanie obszarów roboczych).

	> ℹ️ Niektórzy projektanci stron internetowych mogą ostatecznie utworzyć wiele PSD odpowiadających poszczególnym zastosowanym komponentom i zaimportować je w jednym PSD jako “smart layer”. W takim przypadku będziesz mieć wiele plików PSD połączonych z jednym lub dwoma plikami. W przypadku Sketch, z uwagi że **biblioteki** istnieją od wersji 47, możliwe jest połączenie wielu plików za pomocą symboli ……..

* [ ] **Pliki graficzne są czyszczone** przed dostarczeniem do programistów (pusta i niepotrzebna warstwa musi zostać usunięta, aby uniknąć dużych plików).

* [ ] Strona błędu **404 error** (i ewentualnie błędu page 500 error) została zaprojektowana.
* [ ] Wszystkie **popins, popups i alert boxes** zostały zaprojektowane i można włączyć wrzucanie warstw kompozycji.

__Dodatkowe materiały:__

* 📖 [Photoshop Etiquette: A Guide to Discernible Web Design](http://photoshopetiquette.com/)

#### Szczegółowe zasady dla pliku PSD:

* [ ] **Layer compositions** są używane do wyświetlania każdej strony, jeśli w tym samym PSD zapewniono wiele widoków. To łatwy sposób na uniknięcie zamieszania i sprawdzenie, czy wszystkie elementy są poprawnie zorganizowane.

**[⬆ powrót do góry](#spis-treści)**

## 2. - Analizy i etapy przygotowawcze

![Analysis and phases](/images/phases.png)

Przed rozpoczęciem analizy i fazy przygotowawczej oraz po otrzymaniu creative files należy sprawdzić kilka ważnych elementów:

* __*Która wersja programu Photoshop, Sketch jest używana?*__
  Niektóre funkcje są specyficzne dla niektórych wersji Photoshopa lub Sketch. Ważne jest, aby jak najszybciej zgłosić każdą kwestię dotyczącą tego.
* __*Czy szerokość każdego PSD lub obszaru roboczego jest poprawna?*__
  W przypadku dodania miejsca po każdej stronie projektu, sprawdź dokładną szerokość strony internetowej.
* __*Czy creatives używają zbyt dużo “box-shadow”, “linear lub radial gradient”…?*__
  Nie zapomnij że .... Efekt, który może mieć wpływ na wydajność malowania przeglądarki.
* __*Czy zapewniono mapę witryny / menu nawigacyjne w celu zrozumienia architektury wszystkich stron i ich zależności?*__
* __*Czy strona musi mieć obrazy retina?*__

**[⬆ powrót do góry](#spis-treści)**

### 2.1 - Analiza wersji papierowej

![Paper Analysis](/images/analysis.png)

Zaleca się **drukowanie** niektórych (lub wszystkich) stron w formacie A3 (lub A4, jeśli nie masz tego formatu). Ze względu na wysokość strony. prawdopodobnie będziesz musiał wydrukować niektóre projekty na wielu stronach.

Nie mogę sobie wyobrazić lepszego sposobu na rozpoczęcie niż analizowanie kreacji na papierze ołówkiem (lub innymi kolorowymi ołówkami wybranymi w celu wyróżnienia różnego rodzaju informacji).

1. Zdefiniuj **strukturę stron**, nagłówki, sekcje, artykuły, główne, stopki, opisując je na co najmniej jednej wydrukowanej stronie.

2. Znajdź wszystkie **nagłówki**, które ustrukturyzowały stronę, upewnij się, że `H1` nie ma na logo i że przestrzegana jest logiczna kolejność. Przez większość czasu H1 strony głównej będzie ukryte za pomocą CSS, ale musi zachować swoje uzasadnione znaczenie. Tę analizę należy przeprowadzić przy pomocy specjalisty SEO, jeśli masz go w zespole.

3. Spróbuj znaleźć i zgrupować **podobne komponenty**, nadając im indywidualną nazwę dotyczącą ich funkcjonalności, a nie tylko kontekstu. Na przykład nazywanie systemu kart “

4. Większość creative elements można **wykonać za pomocą CSS**. Dzisiaj nie jest zalecane tworzenie żadnego elementu układu za pomocą obrazów. Każdy prosty element graficzny, taki jak przyciski lub obramowania, powinien być wykonywany w CSS, aby uniknąć problemów z wydajnością lub skalowalnością.

5. Znajdź jakiś **możliwy brak spójności**, w przypadku gdy zespół twórców nie zapewnił Przewodnika po stylach, twoim obowiązkiem jest upewnić się, że każdy element graficzny należy do możliwej kategorii (Przyciski, Typografia, Suwaki…). Pomoże ci to stworzyć własną architekturę CSS / Sass lub zidentyfikować potrzebny komponent ze zidentyfikowanego frameworka CSS.

⚠️ *Po fazie analizy papierowej możesz zaprosić zespół kreatywny do skorzystania z takiego narzędzia, jak [InVision](https://www.invisionapp.com/), w celu ułatwienia komunikacji i wymiany między zespołem kreatywnym a programistami. Możliwość komentowania bezpośrednio na stronach może być oszczędnością czasu i pozwala zachować historię zmian i decyzji.*

### 2.2 - Faza przygotowawcza

* [ ] Zgodnie ze specyfikacjami **potrzebne wtyczki zostały zdefiniowane** na wczesnym etapie. Posiadanie wstępnej listy możliwych wtyczek przed rozpoczęciem programowania może pomóc deweloperowi utrzymać koncentrację i nie spędzać zbyt wiele czasu na badaniach w fazie programowania. Oczywiście niektóre wtyczki mogą nie pasować idealnie i zostaną odpowiednio zmienione.

__Dodatkowe materiały:__

* 🛠 [Awesome JS][22]
* 🛠 [BestOfJS][23]


**[⬆ powrót do góry](#spis-treści)**

## 3. - Walidacja

Faza walidacji ma miejsce, gdy wszystko wydaje się być gotowe do zintegrowania. Ogólnie rzecz biorąc, klient sprawdza poprawność kreacji bez czekania na zgodę zespołu technicznego. Zgodnie z listą kontrolną projektu deweloperzy muszą zapewnić jakość dostarczenia przed rozpoczęciem kodowania.

## 4. - Faza rozwoju

* [ ] Wszystkie **media można wyciąć i zapisać** przed rozpoczęciem fazy rozwoju. Pomoże ci to uniknąć sytuacji, w których oprogramowanie twórcze i edytor kodu będą występować pomiędzy.

* [ ] **Folder obrazów ma przejrzystą architekturę**, w której rozmieszczono obrazy układu. Ważne jest, aby ogólnie zachować spójność między projektami. Pomocne może być zdefiniowanie struktury tego folderu i konwencji nazewnictwa.


  Możesz znaleźć przykład możliwej struktury z prefiksami używanymi do rozpoznawania każdego wyposażenia obrazu.

```bash
.
└── images
    ├── background
    ├── banners
    ├── icons
    └── layout
```

* [ ] **Stosowana jest konwencja nazewnictwa**, podobnie jak dodawanie prefiksów w celu rozróżnienia typów obrazów, wszystkie obrazy użyte w tle mogą być poprzedzone przez `bg-`, ikony przez `icon-`, hero banners przez `hero-` lub `banner-` i tak dalej.

## 5. - Przed produkcją

Przed uruchomieniem witryny sprawdź wszystkie strony za pomocą [Front-End Checklist](https://frontendchecklist.io)!

**[⬆ back to top](#table-of-contents)**

---

## Tłumaczenia

Checklista Frontendu dostępna jest również w innych językach. Dziękujemy wszystkim tłumaczom za ich wspaniałą pracę!

* 🇨🇳 chiński: [JohnsenZhou/Front-End-Design-Checklist](https://github.com/JohnsenZhou/Front-End-Design-Checklist)
* 🇪🇸 hiszpański: [eoasakura/Front-End-Design-Checklist](https://github.com/eoasakura/Front-End-Design-Checklist)
* 🇵🇱 polski: [mbiesiad/Front-End-Design-Checklist](https://github.com/mbiesiad/Front-End-Design-Checklist)

## Wsparcie

Jeśli masz jakieś pytania lub sugestie, nie wahaj się skorzystać z Gittera lub Twittera:

* [Give an UP on Product Hunt](https://www.producthunt.com/posts/front-end-design-checklist)
* [Chat on Gitter](https://gitter.im/Front-End-Checklist][28]/Front-End-Design-Checklist?utm_source=share-link&utm_medium=link&utm_campaign=share-link)
* [Facebook](https://www.facebook.com/frontenddesignchecklist/)
* [Twitter](https://twitter.com/thedaviddias)

## Autor

**[David Dias](https://github.com/thedaviddias)**

## Współtwórcy

Ten projekt istnieje dzięki wszystkim ludziom, którzy [współtworzą!](.github/CONTRIBUTING.md)

## Licencja

[![CC0](https://i.creativecommons.org/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

Wszystkie ikony są dostarczane przez [Icons8](https://icons8.com/)

**[⬆ powrót do góry](#spis-treści)**


[6]:	https://guideguide.me/
[7]:	https://www.sketchapp.com/docs/canvas/rulers-guides-grids/
[8]:	https://getbootstrap.com/docs/4.0/layout/grid/
[9]:	http://flexboxgrid.com/
[10]: 	https://css-tricks.com/dont-overthink-it-grids/
[11]:	https://www.lifewire.com/aco-file-2619477
[16]:	http://bradfrost.com/blog/post/atomic-web-design/
[22]:	https://js.libhunt.com/
[23]:	https://bestof.js.org/
[28]:	https://gitter.im/Front-End-Checklist/Front-End-Design-Checklist

___________________________________________________________________________

Stworzone przez @[thedaviddias](https://github.com/thedaviddias) polska wersja od @[mbiesiad](https://github.com/mbiesiad)
