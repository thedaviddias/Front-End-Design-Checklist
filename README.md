![Front-End Design Checklist](/images/front-end-design-checklist-banner.jpg)
<h2 align="center">Checklista projektowania Frontend</h2>

<p align="center">
  <em> Checklista projektowania dla programistów Frontend to wyczerpująca lista elementów, które mogą pomóc programistom w analizie i zrozumieniu projektów internetowych oraz w zapewnieniu jakości ich rozwoju.</em>
</p>

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com) [![Join the chat at https://gitter.im/Front-End-Checklist/Front-End-Design-Checklist](https://badges.gitter.im/Front-End-Checklist/Front-End-Design-Checklist.svg)](https://gitter.im/Front-End-Checklist/Front-End-Design-Checklist) [![CC0](https://img.shields.io/badge/license-CC0-green.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

## Spis treści
* **[1. Wymagania projektowe](#1---wymagania-projektowe)**
	* [1.1 Grid system](#11---grid-system)
	* [1.2 Colors](#12---colors)
	* [1.3 Fonts and texts](#13---fonts-and-texts)
	* [1.4 Links and navigation](#14---links-and-navigation)
	* [1.5 Images / Icons](#15---images--icons)
	* [1.6 Forms and buttons](#16---forms-and-buttons)
	* [1.7 Responsive Web Design](#17---responsive-web-design)
	* [1.8 Style Guide and component approach](#18---style-guide-and-component-approach)
	* [1.9 Delivery files](#19---delivery-files)
* **[2. Analysis and pre-work phases](#2---analysis-and-pre-work-phases)**
	* [2.1 Paper analysis](#21---paper-analysis)
	* [2.2 Pre-development phase](#22---pre-development-phase)
* **[3. Validation](#3---validation)**
* **[4. Development phase](#4---development-phase)**
* **[5. Before production](#5---before-production)**

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

	> Jeśli “**mobile first**” thinking was not followed by the creative team, some irregularities and inconsistencies may appear between the mobile and the desktop version. Check and flag these issues before starting the development of the project.
* [ ] The **tablet version** of the design in certain cases should be provide too.

⚠️ *The **pixel perfect** notion is today in a certain way deprecated. Today, it’s impossible to have a design that worked the same facing the multitude of the screen sizes.*

__Additional Resources:__

* 📖 [Official Google Webmaster Central Blog: Mobile-first Indexing](https://webmasters.googleblog.com/2016/11/mobile-first-indexing.html)

**[⬆ powrót do góry](#spis-treści)**

### 1.8 - Style Guide and component approach

![Styleguide](/images/styleguide.png)

* [ ] All components designed on each page were created with the **component based approach**  (Atomic Design). If not, issues can occur in terms of performance, maintainability of the project...

  __Materiały:__
  * 📖 [Atomic design][16]
  * 📖 [6 Reasons for Component-Based UI Development](https://www.tandemseven.com/technology/6-reasons-component-based-ui-development/)

* [ ] A **Style Guide** needs to be provided listing all elements, components, styles, dimensions. Some boilerplates like [UX Power Tools](https://www.uxpower.tools/) can help saving time and keep consistency in the designs.

⚠️ *In the case where the Style Guide is missing, it's a good practice to build yourself a [living Style Guide](https://github.com/davidhund/styleguide-generators) to facilitate your work. Some CMS like Drupal, for example, have plugins that allow to develop a living Style Guide using [Pattern Lab](https://drupal-pattern-lab.github.io/).*

__Dodatkowe materiały:__

* 📖 [Style Guides – Design + Sketch – Medium](https://medium.com/sketch-app-sources/tagged/style-guides)
* 📖 [The CodePen Design Patterns and Style Guide](https://codepen.io/guide)
* 📖 [Lonely Planet Travel Guides and Travel Information](http://rizzo.lonelyplanet.com/styleguide/design-elements/colours)
* 📖 [Styleguide](https://www.yelp.com/styleguide)

#### In the case of an existing project:

Sometimes, the creative team needs to add new pages or modules in an existing project. They should have or create a list of all existing elements and try to use what is already there. Having a Style Guide already created can save hours and ensure consistency of the project.

**[⬆ powrót do góry](#spis-treści)**

### 1.9 - Delivery files

![Delivery files](/images/delivery-files.png)

* [ ] For all websites, the web designer needs to provide at least **2 PSD** (mobile, desktop and eventually tablet) or at least **1 Sketch file** which needs to be delivered with the dimension below (if you have Photoshop CC 2015 and above, I recommend using artboards).

	> ℹ️ Some web designers could eventually create multiple PSD corresponding to each components used and import them in a single PSD as “smart layer”. In that case, you’ll have multiple PSD linked to one or two files. In the case of Sketch, since the **libraries** exist since version 47, it is possible to link multiples files with symbols ……..

* [ ] The **creative files are cleaned** before delivering to developers (empty and unnecessary layer needs to be removed to avoid large files).

* [ ] The **404 error** (and eventually the page 500 error) page were designed.
* [ ] All **popins, popups and alert boxes** were designed and can be enable throw layers of compositions.

__Dodatkowe materiały:__

* 📖 [Photoshop Etiquette: A Guide to Discernible Web Design](http://photoshopetiquette.com/)

#### Specific rules for PSD file:

* [ ] **Layer compositions** are used to show each different pages, if multiple views are provided within the same PSD. It’s an easy way to avoid confusions and check that all elements are correctly organized.

**[⬆ powrót do góry](#spis-treści)**

## 2. - Analysis and pre-work phases

![Analysis and phases](/images/phases.png)

Before starting the analysis and the pre-work phases and after receiving the creative files, you need to check some important elements:

* __*Which version of Photoshop, Sketch is used?*__
  Some features are specific to some versions of Photoshop or Sketch. It is important to flag any issue regarding this as soon as possible.
* __*Is the width of each PSD or artboard correct?*__
  In case some space is added on each side of the design, check the exact width of the website.
* __*Are the creatives using too much “box-shadow”, “linear or radial gradient”…?*__
  Don’t forget the .... Effect which can have impacts on the browser painting performance.
* __*Is a sitemap / breadcrumb provided to understand the architecture of all pages and their dependencies?*__
* __*Does the website needs to have retina images?*__

**[⬆ powrót do góry](#spis-treści)**

### 2.1 - Paper analysis

![Paper Analysis](/images/analysis.png)

It is recommended **printing** some (or all) of the pages you have on an A3 format (or A4 if you don’t have this format). Because of the height of the page. you’ll probably need to print some designs on multiple pages.

I can’t imagine a better way to start than analysing creatives on a paper with a pencil (or different colourful pencils chosen to highlight different type of information).

1. Define the **structure of the pages**, the headers, the sections, the articles, main, footer outlining these on at least one printed page.

2. Find all the **headings** that structured a page, ensure the `H1` is not on the logo and that the logical order is followed. Most of the time, the H1 for the homepage will be hidden with CSS but needs to keep its legitimate meaning. That analysis should be done with the help of a SEO specialist in case you have one in your team.

3. Try to find and regroup **similar components** giving them an individual name regarding their functionality and not just their context. For example, naming a tab system “

4. Most of the creative elements can be **done using CSS**. Today, it is not recommended to create any layout element using images. Any simple graphical element like buttons or borders should be done in CSS to avoid performance or scalability issues.

5. Find some **possible lack of coherence**, in case a Styleguide was not provided by the creative team, it’s your responsibility to ensure that every graphic element belong to a possible category (Buttons, Typography, Sliders…). It’ll help you to create your own CSS / Sass architecture or to identify which component you’ll need from an identified CSS Framework.

⚠️ *After the paper analysis phase, you can invite the creative team to use a tool like [InVision](https://www.invisionapp.com/), to facilitate the communication and exchange between the creative team and the developers. The possibility to comment directly on pages can be a time-saver and allow to keep a history of modifications and decisions.*

### 2.2 - Pre-development phase

* [ ] According to the specifications, **plugins needed were defined** in an early stage. Having a pre-list of possible plugins before starting the development can help the developer to stay focus and not spend too much time in doing research during the development phase. Obviously, some plugins may not perfectly fit and will be changed accordingly.

__Additional Resources:__

* 🛠 [Awesome JS][22]
* 🛠 [BestOfJS][23]


**[⬆ powrót do góry](#spis-treści)**

## 3. - Validation

The validation phase is when everything seems to be ready to be integrated. The client, in general, validate the creatives without waiting for any approval from the technical team. As exposed in the Design Checklist, it is essential that developers ensure the quality of the delivery before starting to code.

## 4. - Development phase

* [ ] All **medias can be cut and saved** before starting the development phase. That can help you to avoid back and forth between your creative software and your code editor.

* [ ] **The image folder has a clear architecture** where you  arranged the layout's images. It is important to stay consistent between projects in general. Defining a structure for that folder and a naming convention can be helpful.


  You can find an example of a possible structure with prefixes used to recognise each image appurtenance.

```bash
.
└── images
    ├── background
    ├── banners
    ├── icons
    └── layout
```

* [ ] **A naming convention is used** like adding prefixes to differentiate types of images, all images used for background can be prefixed by `bg-`, icons by `icon-`, hero banners by `hero-` or `banner-` and so on.

## 5. - Przed produkcją

Przed uruchomieniem witryny sprawdź wszystkie strony za pomocą [Front-End Checklist](https://frontendchecklist.io)!

**[⬆ back to top](#table-of-contents)**

---

## Tłumaczenia

The Front-End Checklist is also available in other languages. Thanks for all translators and their awesome work!

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
