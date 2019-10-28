# Introduction

An editor plans to A/B test an article for mobile devices. He needs your help to transform the article design and functionality based on feedback from stakeholders.

# Test Parameters

1.  Modify `css/variation.css` to achieve the **Design** requirements provided below.
2.  Modify `js/variation.js` to achieve the **Functionality** requirements provided below.
    - Javascript solutions should use raw javascript.
    - The use of any javascript libraries, especially `jQuery`, is NOT allowed.
3.  You can modify the mark-up of `index.html`
4.  You can use the Internet to search for a posible solutions.
5.  You may tackle any of the **Design** and **Functionality** requirements below in any order.

# Design Requirements

1.  set the default font for the entire article to be: `"Helvetica Neue", Helvetica, Arial, sans-serif`
2.  set the default font for all headings to be: `Georgia, "Times New Roman", Times, serif`
3.  change the default color of all links to: `#2093d2`
4.  change the default hover color of all links to: `#be2d00`
5.  except for the first in the list, add a top margin of `1em` for all list items
6.  center the figure title "*Average Contingency Fee*"
7.  except for the subtitle, change the top margin for all `h2` tags to: `2em`
8.  the `aside` containing the `blockquote` should not have a border
9.  the `aside` containing the `blockquote` should use the full width of the article
10.  change all `strong` tags in list items to render their text as uppercased
11. When the browser is less than or equal to 480px, reduce the height of the `header` by `20px`
12. When the browser is less than or equal to 480px, reduce the space between the `header` and the title by `20px`
13. When the browser is less than or equal to 480px, hide the "*Average Contingency Fee*" `aside` container
14. When the browser is less than or equal to 480px, the "*How Much Did Readers Receive?*" `figcaption` should have a background color of `#e6e6e6` and should look like `images/example.png`

# Functionality Requirements

1.  Modify the `footer` year to have the following functionality:
    - When loading the page, update the `footer` year to *match the current year*.
2.  Modify the `header` logo to have the following functionality:
    - When clicking the logo, it should toggle between:
        - The page not rendering all the CSS to achieve the design requirements above
        - The page rendering all the CSS to achieve the design requirements above
3.  Given the following *query string*: `?aop=Wrongful%20Termination&views=mobile&views=tablet&views=desktop&variation=1&domain=local&source=test`
    - Convert into *JSON format* using the `query parameter` as the `object property` and the `query value` as the `object property value`.
    - store the *JSON value* as a *global variable*
    - store the value of `variation` as a *session cookie*
    - the value of the `variation` cookie should match the value of the *query parameter*
    - if the `variation` parameter is missing from the *query*, use the value of the cookie to populate the `JSON`
