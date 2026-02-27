# Blueprint for "세븐챠트" Homepage

## Overview
This blueprint outlines the creation of a homepage named "세븐챠트" (Seven Chart), designed to be similar in aesthetic and functionality to linkroom.org. The primary goal is to provide a clean, minimalist, and highly readable directory of links/resources, organized into categories.

## Detailed Outline of Project
*   **Title:** "세븐챠트"
*   **Design Philosophy:** Minimalist, content-focused, high-contrast for readability, with a clean layout.
*   **Core Structure:**
    *   `index.html`: Main HTML file for the page structure.
    *   `style.css`: CSS file for all styling.
    *   `main.js`: JavaScript file for any interactivity (initially minimal).
*   **Key Design Elements (inspired by linkroom.org analysis):**
    *   Clear header with site title and navigation menu.
    *   Main content area structured with categories and lists of links.
    *   Simple, readable typography (sans-serif).
    *   High-contrast color scheme (e.g., dark background with light text).
    *   Responsive design.
    *   Distinct footer.
    *   Advertisement banners at the top.
    *   A central, horizontally arranged "배고광코칸" feature.
    *   Top-right horizontal menu for general navigation (Login, etc.).
    *   Top-left horizontal menu for "게시판 기능" (Announcements, Free Board, Telegram Inquiry).

## Implemented Features (Completed)

1.  **Project Setup:**
    *   Created `index.html`, `style.css`, and `main.js`.
    *   Added basic HTML5 boilerplate to `index.html`.
    *   Linked `style.css` and `main.js` in `index.html`.
    *   Set the page title to "세븐챠트".
2.  **Initial HTML Structure:**
    *   Implemented a `<header>` with the site title.
    *   Added a `<main>` element to hold content.
    *   Included a `<footer>`.
    *   **Content:** Added several placeholder category sections within the `<main-content>` area, each with a heading and a list of placeholder links, simulating the directory structure of linkroom.org.
3.  **Basic CSS Styling:**
    *   Applied a dark background and light text color scheme.
    *   Set a base sans-serif font family.
    *   Styled the header and footer for a clean appearance.
    *   **Main Content Styling:** Implemented CSS Grid for laying out categories in the main content area.
    *   Styled individual category blocks with background, padding, and subtle shadow/hover effects.
    *   Styled category headings.
    *   Styled the lists of links, removing default list styles.
    *   Styled individual links with specific colors and hover effects for a high-contrast and minimalist aesthetic.
    *   Ensured basic responsiveness for the overall layout.
4.  **Advertisement Banners:**
    *   Added a `<section class="ad-banners">` immediately after the `<header>` in `index.html`, containing three `div` elements for placeholder banners.
    *   Styled the `.ad-banners` container using Flexbox to arrange banners horizontally with a gap.
    *   Styled individual `.ad-banner-item` elements with distinct background, height, borders, and centered text.
    *   Implemented responsiveness for the ad banners, causing them to stack vertically on smaller screens.
5.  **Top Right Navigation Menu (General Navigation):**
    *   Initially had "공지사항", "자유게시판", "텔레문의", and "로그인".
    *   Now contains only "로그인" in `<nav class="main-nav">` within the `<header .container>`.
    *   Styled the navigation menu to display horizontally using flexbox, with appropriate spacing and hover effects, integrating seamlessly with the existing dark theme.
    *   **Alignment:** Modified the header's CSS to use flexbox, aligning the `<h1>` title to the left and the `.main-nav` to the right within the header, while ensuring proper vertical alignment and responsiveness.
    *   **Box Styling:** The `.main-nav a` style gives it a distinct background, increased padding, and a border to create a "box" appearance, and refined hover styles for these new box-like elements.
6.  **"배고광코칸" Feature:**
    *   Added a new `<section class="feature-input-section">` element within the `<main-content>` container in `index.html`, before the existing categories, with a placeholder input and button.
    *   Styled the `.feature-input-section` to provide vertical spacing and a distinct background.
    *   Styled its internal `input-container` to be a horizontal flex container and centered its contents.
    *   Styled the input field and button to match the dark theme, including appropriate padding, borders, background, text color, and hover effects.
    *   Implemented responsiveness for this section, allowing the input and button to stack vertically on smaller screens.
7.  **Top Left "게시판 기능" Menu:**
    *   Introduced a new `div` wrapper (`<div class="header-left-group">`) within `.header .container`.
    *   Moved the `<h1>세븐챠트</h1>` inside this `header-left-group`.
    *   Added a new `<nav class="board-nav">` with "공지사항", "자유게시판", and "텔레문의" links *within* this `header-left-group`.
    *   Adjusted the `.header .container` to manage `header-left-group` and `main-nav`.
    *   Styled `header-left-group` to arrange its contents (h1 and board-nav).
    *   Styled `board-nav` (including its links) to match the "square box" style and integrate with the left side, ensuring responsiveness.

## Next Steps / Future Enhancements

*   Implement search functionality.
*   Add actual links and dynamic content loading.
*   Refine color scheme and typography based on user feedback.
*   Implement Web Components for more complex, reusable UI elements if needed.
