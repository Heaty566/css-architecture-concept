# Scss-kit

## Concept
**SMACSS** which stands for Scalable and Modular Architecture for CSS is a set of guidelines to categorize your CSS rulesets to make the CSS codebase scalable and modular. It is not a technology or utility, it’s just a set of some golden rules or you can say guidelines to write your CSS.

1. Base — All the CSS rulesets which are used to give default styling to HTML elements in all occurrences of the page, fall under the Base rules. We don’t use classor id selectors to define these rulesets, rather we use element descendent selector, or a child selector, along with any pseudo-classes.

2. Layout — As per SMACSS principles, all the UI elements or components in a page can be categorized into two groups- major and minor UI Components. The major components are those which define the structure of the page and generally do not repeat itself in the page like headers, footers, sidebar, body, etc. These major components form the page Layout and hence, referred to as Layout rules.

3. Module (Component) — Modules are individually separated and distinct UI component. It sits inside the layout component as mentioned above as well as inside Modules itself. It is independent of other UI modules or layouts. Some very common examples are accordion , modal , button , carousal , etc.

4. State — State CSS Rulesets are basically to define Styles for a different state of a UI component. These basically overrides the default Styling of a UI module.

## How to build for production
When your project ready to deploy. using one of following config in your vscode json for faster loading css

 ```js
            "liveSassCompile.settings.formats":[
                // This is Default.
                {
                    "format": "expanded",
                    "extensionName": ".css",
                },
                // mini css allow browser can read your css faster
                {
                    "format": "compressed",
                    "extensionName": ".css",
                },
            ]
```

## Reference
 - [CSS Architecture with SASS, SMACSS, and BEM. by Bitupon Chetia]( https://itnext.io/css-architecture-with-sass-smacss-and-bem-cc618392c148 "Named link title") 