# Unicusine Restaurant Page

A restaurant website built with vanilla JavaScript modules and Webpack. Instead of navigating between separate HTML documents, the Home, Menu, and Contact views are created in JavaScript and rendered into a shared content container.

[View the live site](https://mohamedmosilhy.github.io/Restaurant-Page/) · [View the source](https://github.com/mohamedmosilhy/Restaurant-Page)

![Unicusine restaurant home page](./screenshots/home.png)

## Views

### Home

Introduces Unicusine with a headline and a full-width food photograph.

### Menu

Displays six menu cards with photography, dish names, prices, and Book Now controls:

- Berry Smoothie
- Bibimbap Bowl
- Grilled Steak
- Lemon Cheesecake
- Kimchi Stir Fry
- Spicy Chicken

### Contact

Presents the restaurant address, telephone number, and email with dedicated local icons.

## Implementation highlights

- Persistent navigation shared across all views
- DOM-generated page content
- Separate modules for Home, Menu, and Contact
- ES module imports for CSS and image assets
- Webpack asset handling and HTML template generation
- Responsive layouts and locally stored food photography

The phone, booking, and contact controls are presentation elements; they do not currently create reservations or send messages.

## Built with

- HTML5
- CSS3
- JavaScript ES modules
- Webpack
- HtmlWebpackPlugin
- webpack-dev-server

## Getting started

### Prerequisites

- Node.js
- npm

### Installation

```bash
git clone https://github.com/mohamedmosilhy/Restaurant-Page.git
cd Restaurant-Page
npm install
npm run dev
```

The development server opens the site and reloads changes from `src/`.

### Available scripts

| Command | Purpose |
| --- | --- |
| `npm run dev` | Start Webpack Dev Server |
| `npm run build` | Create a production bundle in `dist/` |
| `npm run deploy` | Push the built `dist/` subtree to the `gh-pages` branch |

## Project structure

```text
Restaurant-Page/
├── src/
│   ├── assets/             # Food and contact imagery
│   ├── css/styles.css
│   ├── html/template.html
│   └── js/
│       ├── index.js        # Navigation and view switching
│       ├── initial_page.js
│       ├── menu_page.js
│       └── contact_page.js
├── webpack.config.js
├── package.json
├── LICENSE
└── README.md
```

## License

See [LICENSE](./LICENSE) for the repository's license terms.
