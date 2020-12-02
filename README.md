# Tailwind Workshop With Small Boilerplate
>Small boilerplate with [TailwindCSS](https://tailwindcss.com/), [PostCSS](https://postcss.org/) and [StyleLine](https://stylelint.io/).

### VSCode 
This workshop uses VSCode since the Tailwind creators maintain a VSCode extension providing IntelliSense for Tailwind.

> However, Tailwind is supported in [WebStorm](https://www.jetbrains.com/webstorm/whatsnew/#support-for-tailwind-css) as of monday, and in [Rider](https://blog.jetbrains.com/webstorm/2020/11/webstorm-2020-3-eap-7/#tailwind_css_support), PhpStorm and PyCharm under the Early Access Program.

# Setup
- Get [VSCode](https://code.visualstudio.com/)

Consider the [Auto-Open Markdown Preview](https://marketplace.visualstudio.com/items?itemName=hnw.vscode-auto-open-markdown-preview) for reading the `README.md`-files in VSCode.
## VSCode Extensions

- [Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss)
- [Headwind](https://marketplace.visualstudio.com/items?itemName=heybourn.headwind)
- [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
- [Stylelint](https://marketplace.visualstudio.com/items?itemName=stylelint.vscode-stylelint) <- Addition from WS with minimal boilerplate

# Getting started
- `npm install` 🏃‍♂️
- `npm run build` 🏗️
- Right-click desired HTML-file, and click `Open with Live Server` 🚀
- Edit the HTML and enjoy live reload 😎

# What is this setup 🤔?
### IntelliSense
Provides autocomplete, linting, hover-preview and syntax-highlighting. The *awesomeness* lies in that it includes all the customizations in `tailwind.config.js` that form your design system.

### Headwind
Enforces consistent ordering of classes. Which reduces the cognitive load of dealing with multiple classnames.

### Live Server
Simple solution to launch a local development server with live reload.

### Stylelint
VSCode's default CSS validator disallows unknown at-rules, which includes a few Tailwind at-rules (`@tailwind`, `@responsive` etc.).   

There are [alternative solutions](https://stackoverflow.com/questions/47607602/how-to-add-a-tailwind-css-rule-to-css-checker/61333686#61333686) that configures VSCode, but I've opted for Stylelint because "[it is to style sheets what ESLint is for JavaScript](https://www.smashingmagazine.com/2016/05/stylelint-the-style-sheet-linter-weve-always-wanted/)".

Stylelint is configured in `stylelint.config.js` with a [recommended standard configuration](https://github.com/stylelint/stylelint-config-standard) that enforce common stylistic conventions found in reputable CSS styleguides, including: [The Idiomatic CSS Principles](https://github.com/necolas/idiomatic-css),
[Google's CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html#CSS_Formatting_Rules) and [Airbnb's Styleguide](https://github.com/airbnb/css#css). 

## Rebuild config