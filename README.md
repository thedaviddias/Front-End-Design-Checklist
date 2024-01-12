![Front-End Design Checklist](/images/front-end-design-checklist-banner.jpg)
<h2 align="center">Front-End Design Checklist</h2>

<p align="center">
  <em> The Design Checklist for Front-End Developers is an exhaustive list of elements which can help developers to analyse and understand web designs and ensure the quality of their Front-End development.</em>
</p>

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com) [![Join the chat at https://gitter.im/Front-End-Checklist/Front-End-Design-Checklist](https://badges.gitter.im/Front-End-Checklist/Front-End-Design-Checklist.svg)](https://gitter.im/Front-End-Checklist/Front-End-Design-Checklist) [![CC0](https://img.shields.io/badge/license-CC0-green.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

## Table of Contents
* **[1. Design requirements](#1---design-requirements)**
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

> The **Design Checklist for Front-End Developers** is an exhaustive list of elements which Web Designers and Front-End Developers need to take into consideration to facilitate their collaboration. The following elements are a mix between known practices and new elements based on a long experience analysing web designs.

In case you are looking for a list of all elements you need to have/to test before launching your site/HTML page to production, take a look on the → [Front-End Checklist](https://github.com/thedaviddias/Front-End-Checklist).


## How to use the Design Checklist?

When comes the moment where developers discover new web designs, before converting them to code, some important elements may be missing. The Front-End Design Checklist is a tool for Front-End developers and Web Designers which aim to help both to work in a seamlessly way.

You can share that checklist to Web Designers to ensure time will be saved at the delivery time or you can use it to review all elements delivered by the creative team and ensure everything is correct before digging into the code integration.


## Why you need to use the Design Checklist?

* Ensure all points are taken into consideration by the Creative Team
* Having a document where Web Designers and Developers can rely to ensure a better communication and coherence in the way they interact.
* Because it's easy to forget some important elements when you are pushed by short timelines
* Avoid discovering issues after the creative team is already working on another project.
* To show the complementary work between a Web Designer and a Front-End Developer

---

## 1. - Design requirements

Designing a website or a webapp requires following some rules and taking into consideration that the project is not only a graphic project but a web project too. The next sections are crucial for any web project.

### 1.1 - Grid system

![Grid system](/images/grid-system.png)

* [ ] A **grid** is explicitly provided in the design, and the details of the grid are present in the technical specification (width, gutters, number of columns…). The Web Designer can keep the grid in a transparent layer and use it on all his project.
	> ℹ️ [GuideGuide][6] is a plugin for many design tools that can help you easily build your grid.

	> ℹ️ On Sketch, you can use the integrated “[Make Grid Tool][7]” to design your desired grid.

* [ ] **Be familiar with the grid system** you’ll use on your project. Most of the time, some options (like alignment, offsetting, nesting…) are ignored by the developer and tend to be replaced by manual padding or margin unnecessarily.
* [ ] Before working on each components of your website, you can **build every templates** used in the creatives only with the grid classes. Building the structure before everything else, will facilitate your work afterwards.

```html
<div class="container">
  <div class="row">
    <div class="col-sm">
      <!-- Let empty at first -->
    </div>
    <div class="col-sm">
      <!-- Let empty at first -->
    </div>
    <div class="col-sm">
      <!-- Let empty at first -->
    </div>
  </div>
</div>
```

⚠️ *If you want to ensure that the grid and the width of the devices are respected, you may want to generate yourself a PSD template and that you will send it to the Web Designer.*

__Additional Resources:__

* 🛠 [Bootstrap Grid System][8] (v4)
* 🛠 [Flexbox Grid][9]
* 📖 [Don't Overthink It Grids | CSS-Tricks][10]

**[⬆ back to top](#table-of-contents)**

### 1.2 - Colors

![Colors](/images/colors.png)

* [ ] **All colors used in the creatives are named** ($gray-light, $gray-dark, $green) or accordingly with their use ($body-background, $body-copy, $text-paragraph…). They can be exported in an [ACO file][11] (if use Photoshop or on a symbol page for Sketch) and shared with the developers.

![Color Swatches](/images/color-swatches.jpg)

* [ ] The different **color state** of some elements (like buttons, links, inputs...) are defined and worked in the context of a light or dark background and with a light or a dark text.

* [ ] All or the most important/used **colors are accessible** in the design to allow a fluid navigation on the website/webapp.

__Additional Resources:__
* 🛠 [WCAG - Contrast Checker](https://contrastchecker.com/)
* 🛠 [Color Safe - accessible web color combinations](http://colorsafe.co/)
* 🛠 [Coolors.co - The super fast color schemes generator](https://coolors.co/)

**[⬆ back to top](#table-of-contents)**

### 1.3 - Fonts and texts

![Fonts](/images/fonts.png)

Fonts are an essential part of every design, they shouldn’t be chosen without discernment. Choosing the wrong font for a project could have financial and legal impacts.

It is recommended to ask your client to buy these fonts to avoid possible future issues and take into consideration the condition of use. Some webfonts are limited in terms of pageviews and can’t be hosted ([Understanding Webfont Licensing Structures](https://aeolidia.com/understanding-webfont-licensing-structures/)).

* [ ] The fonts for desktop (TTF or OTF in general) and the webfonts, in **WOFF, WOFF2 and TTF format** were provided (in a Zip file or given access to the website where they were bought).
	> ℹ️ TTF format for desktop is not the same than TTF for Web.

  __Resources:__
	* 📖 [Using @font-face | CSS-Tricks](https://css-tricks.com/snippets/css/using-font-face/)
* [ ] [Fallback font](https://en.wikipedia.org/wiki/Fallback_font) stacks were specified in a document (ideally the Style Guide) to the Front-End Developer.

  __Resources:__
  * 📖 [CSS Basics: Fallback Font Stacks for More Robust Web Typography | CSS-Tricks](https://css-tricks.com/css-basics-fallback-font-stacks-robust-web-typography/)
  * [Create Your Own @font-face Kits » Font Squirrel](https://www.fontsquirrel.com/tools/webfont-generator)

* [ ] The **total weight** of the all webfonts don’t exceed 1-2 Mb (all variants included: italic, bold etc).

* [ ] As far as possible, **all texts are provided in the proper language** instead of dummy texts in English (Lorem Ipsum and affiliates).

	> ℹ️ In case of a multilingual website, always ask yourself how the design can react if the text is longer than it was previously define. Remember that Web Designers use to create perfect designs and don’t always think about possible issues or situation with too much text.

__Additional Resources:__
* 📖 [Web Font Optimization  |  Web Fundamentals  |  Google Developers](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/webfont-optimization)
* [`font-display` for the Masses | CSS-Tricks](https://css-tricks.com/font-display-masses/)
* [Rhythm in Typography | improve legibility, readability, and visual hierarchy](https://betterwebtype.com/rhythm-in-web-typography)

**[⬆ back to top](#table-of-contents)**

### 1.4 - Links and navigation

![Links and navigation](/images/links.png)

* [ ] All **links have a default, hover, focus, active and visited state** clearly defined (the Style Guide is the best document to specified these).
* [ ] Alternate views of all navigation states (hover, active/current page).

### 1.5 - Images / Icons

![Images](/images/images.png)

* [ ] A **favicon image** with at least 512px X 512px is provided in PNG format. The generation of all the others Favicons can be easily done with online tools.

  __Resources:__
  * [Favicon Generator for all platforms: iOS, Android, PC/Mac...](https://realfavicongenerator.net/)

* [ ] All icons are provided in **SVG format**, each in the same square dimension, in black and in a separated folder.

  __Resources:__
  * 🛠 [SVGOMG - SVGO's Missing GUI](https://jakearchibald.github.io/svgomg/)

* [ ] The **name of each icon** starts with `icon-` and is entirely in lowercase (without any space and using dashes to separate each word).

__Additional Resources:__
* 📖 [Essential Image Optimization](https://images.guide/)

**[⬆ back to top](#table-of-contents)**

### 1.6 Forms and buttons

![Forms](/images/forms.png)

* [ ] All forms possess a title that can be used as a legend
* [ ] An example of the **different states of all input fields** were provided (at least focus and inactive/disabled state).
* [ ] **All error messages** were provided, the text (eventually in a separated document) the position and the color are clearly identifiable in the creatives and consistent. Some messages should be different according to the error.
  __Resources:__
  * 📖 [Forms Need Validation – UX Collective](https://uxdesign.cc/forms-need-validation-2ecbccbacea1)
* [ ] **Indicators of required/optional** fields are provided.
* [ ] The **primary and secondary buttons** are clearly identifiable and are used following common practices.
  __Resources:__
  * 📖 [Primary & Secondary Action Buttons – UX Planet](https://uxplanet.org/primary-secondary-action-buttons-c16df9b36150)
* [ ] An example of the **different states of a button** were provided (Normal, hover, focused, pressed and inactive state).
* [ ] Buttons with built-in **loading indicators** are provided and can be applied to any button.

__Additional Resources:__

* 📖 [Design Better Forms – UX Collective](https://uxdesign.cc/design-better-forms-96fadca0f49c)
* 📖 [Design Better Input Fields – UX Collective](https://uxdesign.cc/design-better-input-fields-3d02985a8e24)
* 📖 [Designing Perfect Text Field: Clarity, Accessibility and User Effort](https://uxplanet.org/designing-perfect-text-field-clarity-accessibility-and-user-effort-d03c1e26004b)
* 📖 [Button UX Design: Best Practices, Types and States – UX Planet](https://uxplanet.org/button-ux-design-best-practices-types-and-states-647cf4ae0fc6)
* 📖 [How To Design Better Buttons — Smashing Magazine](https://www.smashingmagazine.com/2016/11/a-quick-guide-for-designing-better-buttons/)
* 📖 [Buttons in Design Systems – EightShapes – Medium](https://medium.com/eightshapes-llc/buttons-in-design-systems-eac3acf7e23)

**[⬆ back to top](#table-of-contents)**

### 1.7 - Responsive Web Design

![Responsive](/images/responsive.png)

* [ ] The **mobile version** of the design is provided before or at the same time of the desktop version.

	> If the “**mobile first**” thinking was not followed by the creative team, some irregularities and inconsistencies may appear between the mobile and the desktop version. Check and flag these issues before starting the development of the project.
* [ ] The **tablet version** of the design in certain cases should be provide too.

⚠️ *The **pixel perfect** notion is today in a certain way deprecated. Today, it’s impossible to have a design that worked the same facing the multitude of the screen sizes.*

__Additional Resources:__

* 📖 [Official Google Webmaster Central Blog: Mobile-first Indexing](https://webmasters.googleblog.com/2016/11/mobile-first-indexing.html)

**[⬆ back to top](#table-of-contents)**

### 1.8 - Style Guide and component approach

![Styleguide](/images/styleguide.png)

* [ ] All components designed on each page were created with the **component based approach**  (Atomic Design). If not, issues can occur in terms of performance, maintainability of the project...

  __Resources:__
  * 📖 [Atomic design][16]
  * 📖 [6 Reasons for Component-Based UI Development](https://www.tandemseven.com/technology/6-reasons-component-based-ui-development/)

* [ ] A **Style Guide** needs to be provided listing all elements, components, styles, dimensions. Some boilerplates like [UX Power Tools](https://www.uxpower.tools/) can help saving time and keep consistency in the designs.

⚠️ *In the case where the Style Guide is missing, it's a good practice to build yourself a [living Style Guide](https://github.com/davidhund/styleguide-generators) to facilitate your work. Some CMS like Drupal, for example, have plugins that allow to develop a living Style Guide using [Pattern Lab](https://drupal-pattern-lab.github.io/).*

__Additional Resources:__

* 📖 [Style Guides – Design + Sketch – Medium](https://medium.com/sketch-app-sources/tagged/style-guides)
* 📖 [The CodePen Design Patterns and Style Guide](https://codepen.io/guide)
* 📖 [Lonely Planet Travel Guides and Travel Information](http://rizzo.lonelyplanet.com/styleguide/design-elements/colours)
* 📖 [Styleguide](https://www.yelp.com/styleguide)

#### In the case of an existing project:

Sometimes, the creative team needs to add new pages or modules in an existing project. They should have or create a list of all existing elements and try to use what is already there. Having a Style Guide already created can save hours and ensure consistency of the project.

**[⬆ back to top](#table-of-contents)**

### 1.9 - Delivery files

![Delivery files](/images/delivery-files.png)

* [ ] For all websites, the web designer needs to provide at least **2 PSD** (mobile, desktop and eventually tablet) or at least **1 Sketch file** which needs to be delivered with the dimension below (if you have Photoshop CC 2015 and above, I recommend using artboards).

	> ℹ️ Some web designers could eventually create multiple PSD corresponding to each components used and import them in a single PSD as “smart layer”. In that case, you’ll have multiple PSD linked to one or two files. In the case of Sketch, since the **libraries** exist since version 47, it is possible to link multiples files with symbols ……..

* [ ] The **creative files are cleaned** before delivering to developers (empty and unnecessary layer needs to be removed to avoid large files).

* [ ] The **404 error** (and eventually the page 500 error) page were designed.
* [ ] All **popins, popups and alert boxes** were designed and can be enable throw layers of compositions.

__Additional Resources:__

* 📖 [Photoshop Etiquette: A Guide to Discernible Web Design](http://photoshopetiquette.com/)

#### Specific rules for PSD file:

* [ ] **Layer compositions** are used to show each different pages, if multiple views are provided within the same PSD. It’s an easy way to avoid confusions and check that all elements are correctly organized.

**[⬆ back to top](#table-of-contents)**

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

**[⬆ back to top](#table-of-contents)**

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


**[⬆ back to top](#table-of-contents)**

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

## 5. - Before production

Before launching your website, be sure to review all your pages using the [Front-End Checklist](https://frontendchecklist.io)!

**[⬆ back to top](#table-of-contents)**

---

## Translations

The Front-End Checklist is also available in other languages. Thanks for all translators and their awesome work!

* 🇨🇳 Chinese: [JohnsenZhou/Front-End-Design-Checklist](https://github.com/JohnsenZhou/Front-End-Design-Checklist)
* 🇪🇸 Spanish: [eoasakura/Front-End-Design-Checklist](https://github.com/eoasakura/Front-End-Design-Checklist)

## Support

If you have any question or suggestion, don't hesitate to use Gitter or Twitter:

* [Give an UP on Product Hunt](https://www.producthunt.com/posts/front-end-design-checklist)
* [Chat on Gitter](https://gitter.im/Front-End-Checklist][28]/Front-End-Design-Checklist?utm_source=share-link&utm_medium=link&utm_campaign=share-link)
* [Facebook](https://www.facebook.com/frontenddesignchecklist/)
* [Twitter](https://twitter.com/thedaviddias)

## Author

**[David Dias](https://github.com/thedaviddias)**

## Contributors

This project exists thanks to all the people who [contribute!](.github/CONTRIBUTING.md)

## License

[![CC0](https://i.creativecommons.org/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

All icons are provided by [Icons8](https://icons8.com/)

**[⬆ back to top](#table-of-contents)**


[6]:	https://guideguide.me/
[7]:	https://www.sketchapp.com/docs/canvas/rulers-guides-grids/
[8]:	https://getbootstrap.com/docs/4.0/layout/grid/
[9]:	http://flexboxgrid.com/
[10]: https://css-tricks.com/dont-overthink-it-grids/
[11]:	https://www.lifewire.com/aco-file-2619477
[16]:	http://bradfrost.com/blog/post/atomic-web-design/
[22]:	https://js.libhunt.com/
[23]:	https://bestof.js.org/
[28]:	https://gitter.im/Front-End-Checklist/Front-End-Design-Checklist
