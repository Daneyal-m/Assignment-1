# Personal Portfolio Website — Mohammed Daneyal Mazher

**Author:** Mohammed Daneyal Mazher  
**Student ID:** 100973647  
**Email:** mohammeddaneyal.mazher@ontariotechu.net  
**Course:** INFR 3120U – Web and Script Programming  
**Date:** October 2026

A responsive, multi page personal portfolio website built using semantic HTML5 and CSS3. The project features adaptive media queries for desktop, tablet, and mobile displays, custom Google Fonts, linear gradient accents, integrated video and image media, and an accessible contact form.

## 1. Project Overview & File Structure

The project is structured into 4 HTML content pages and 3 device specific CSS stylesheets:

* **HTML Pages:**
  * `index.html`: The landing/home page presenting a welcome heading and a welcome gif.
  * `about.html`: The about me page intro para, a profile picture (`me.png`), and an embedded HTML5 video introduction (`intro.mp4`) with a poster frame (`intro2.png`).
  * `projects.html`: showcasing four projects (*Cosmic Carnage*, *Khidmaatt*, *Aus Adventures*, and *To-Do List*) using `.card` components and preview screenshots.
  * `contact.html`: A contact me page featuring a form that posts directly to my email address using `mailto:`.

* **CSS Stylesheets:**
  * `stylesheet.css`: Base and desktop layout styles.
  * `tablet.css`: Tablet media query styles targeting screen widths from `769px` to `1024px`.
  * `mobile.css`: Mobile media query styles targeting screen widths up to `768px`.

* **Assets:**
  * Images: `welcome.gif`, `me.png`, `CosmicCarnage.png`, `khidmaatt.png`, `AusAdventures.png`, `intro2.png`.
  * Video: `intro.mp4`.


## 2. Font Families

The website utilizes a dual-font strategy imported from Google Fonts alongside a standard web-safe fallback stack:

* **Header Title (`header h1`):**
  * `font-family: "Satisfy", cursive`.
  * Google Fonts preconnect links are included in the `<head>` of all pages (`https://fonts.googleapis.com` and `https://fonts.gstatic.com`) to optimize font delivery latency, importing both `Playfair Display` and `Satisfy`.

* **Body & General Content:**
  * `font-family: Arial, Helvetica, sans-serif`.


## 3. Color Palette & Scheme

The website uses a warm pastel and earth-toned palette from Adobe Color, designed for soft contrast and readability:
| Element | Color Name / Hex Value | Role & Usage |
|---|---|---|
| **Site Background** | `#F2D3D0` | Soft pastel background applied across the entire `body`. |
| **Header & Footer** | `#F7B4AE` | Accent peach-coral used for the top header banner and bottom footer container. |
| **Primary Text** | `brown` | text color applied globally to headings, paragraphs, and links. |
| **Card Fallback** | `#F2B999` | Warm peach background fallback for project cards. |
| **Contact Card Fallback** | `bisque` | Soft cream-peach fallback for the contact form container. |
| **Borders** | `#ccc` / `1px solid brown` | `#ccc` outlines project cards, video player, and form cards; `brown` outlines buttons. |
| **Button States** | `#F7B4AE` (Default) / `white` (Hover) | Primary button accent with high-contrast inverted white hover effect. |


## 4. Gradients Used in the Project


1. **Project Cards (`.card` in `stylesheet.css`, `tablet.css`, `mobile.css`):**
   * **Rule:** `background: -webkit-linear-gradient(top, #F2B999 0%, #F7B4AE 100%);`
   * **Type & Direction:** Top-to-bottom vertical linear gradient.
   * **Colors:** Blends from warm peach (`#F2B999`) at `0%` to soft coral-pink (`#F7B4AE`) at `100%`.
   * **Location:** Applied to all project display cards on the Projects page (`projects.html`).

2. **Contact Form Card (`#Contact .card` in `stylesheet.css`):**
   * **Rule:** `background: linear-gradient(135deg, bisque 0%, #F7B4AE 100%);`
   * **Type & Direction:** 135-degree diagonal linear gradient.
   * **Colors:** Flows smoothly from light cream `bisque` at `0%` in the upper-left to coral-pink `#F7B4AE` at `100%` in the lower-right.


## 5. Viewport Breakpoints & Responsive Dimensions

Responsive behavior is divided across three distinct stylesheets linked via HTML media queries:

* `<link rel="stylesheet" href="stylesheet.css">`
    The desktop dimensions use spacious 50px side margins, fluid 5% header padding, and capped element widths—like the 50% contact form and 600px video so the content takes 
    advantage of large computer screens while keeping lines of text and media from stretching too wide to read comfortably.
* `<link rel="stylesheet" href="mobile.css" media="(max-width: 768px)">`
    The mobile dimensions (768px and lower) reduce outer margins to a tight 16px to 20px and push cards, images, and inputs to a full 100% width so everything stacks naturally down the screen, preventing awkward horizontal scrolling while keeping buttons and 16px form text easy and comfortable to tap with thumbs.
* `<link rel="stylesheet" href="tablet.css" media="(min-width: 769px) and (max-width: 1024px)">`
    The tablet dimensions scale (between 769px and 1024px) the spacing down to 32px side margins, 3.5% header padding, and a 75% contact form to balance the layout on medium sized displays, giving content plenty of breathing room without wasting screen space or crowding touch navigation.


## 6. References

 **Course Lectures & Materials:**
   * Munieb, S. A. (2026). *INFR 3120U: Web and Script Programming — Course Lecture Slides and Instructional Materials*. Faculty of Business and Information Technology, Ontario Tech University.

 **Google Fonts:**
  * Google. (n.d.). *Google Fonts*. Retrieved October 9, 2026, from https://fonts.google.com/

 **Adobe Color:**
  * Adobe Inc. (n.d.). *Adobe Color: Color wheel & color palette generator*. Retrieved October 9, 2026, from https://color.adobe.com/create