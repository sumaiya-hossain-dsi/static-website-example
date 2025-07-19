# Static Website Example Documentation

## Overview
This repository contains a responsive static website built using the "Dimension" template by HTML5 UP. It's designed to be used with Cloud Academy labs and serves as an example of a modern, responsive static website implementation.

## Project Structure

```
static-website-example/
├── assets/               # All website assets
│   ├── css/              # Compiled CSS files
│   ├── fonts/            # Font Awesome font files
│   ├── js/               # JavaScript files
│   └── sass/             # SASS source files
├── error/                # Error page (404)
├── images/               # Website images
├── sections/             # Modular content sections
│   ├── about/            # About section content
│   ├── contact/          # Contact section content
│   ├── elements/         # Elements section content
│   ├── intro/            # Intro section content
│   └── work/             # Work section content
└── index.html            # Main HTML file
```

## Template Information
- **Name**: Dimension by HTML5 UP
- **Designer**: @ajlkn
- **Website**: [html5up.net](https://html5up.net)
- **License**: [Creative Commons Attribution 3.0 License](https://html5up.net/license)

## Features
- Fully responsive design that works on all devices
- Modern, clean single-page layout
- Animated transitions between sections
- Modal-based navigation
- Contact form
- Social media icons
- Cross-browser compatibility (including IE9 support)
- Modular section content organization

## Technical Implementation

### HTML Structure
The website is built as a single-page application with multiple sections that are shown/hidden using JavaScript. The main sections include:
- Header with navigation
- Intro section
- Work section
- About section
- Contact section
- Elements section (hidden by default)

Each section's content is stored in its own directory under the `sections/` folder, making the codebase more modular and maintainable.

### Content Loading
The website uses AJAX to dynamically load section content from the `sections/` directory:
- Each section is stored in its own subdirectory with an `index.html` file
- The main JavaScript loads these sections on page initialization
- This modular approach makes it easier to maintain and update individual sections

### CSS/SASS Architecture
The styling is implemented using SASS with a well-organized structure:
- **Base**: Core styling for page elements and typography
- **Components**: Reusable UI components (buttons, forms, tables, etc.)
- **Layout**: Page-specific layouts (header, footer, main content)
- **Libs**: Utility functions, variables, and mixins

The SASS files are compiled into several CSS files:
- `main.css`: Main stylesheet
- `ie9.css`: IE9-specific styles
- `noscript.css`: Styles for users with JavaScript disabled

### JavaScript Functionality
The website uses several JavaScript libraries:
- **jQuery**: DOM manipulation
- **Skel**: Responsive framework
- **Util.js**: Utility functions

The main JavaScript file (`main.js`) handles:
- Page loading animations
- Section transitions
- Modal behavior
- Form handling
- Responsive adjustments
- Dynamic section content loading

### Responsive Design
The website uses media queries to adapt to different screen sizes:
- xlarge: max-width 1680px
- large: max-width 1280px
- medium: max-width 980px
- small: max-width 736px
- xsmall: max-width 480px
- xxsmall: max-width 360px

## Usage
This template can be customized by:
1. Modifying the content in the section files under `sections/` directory
2. Updating images in the `images/` directory
3. Customizing styles in the `assets/sass/` directory (requires SASS compilation)
4. Extending functionality in `assets/js/main.js`

### Adding a New Section
To add a new section:
1. Create a new directory under `sections/` (e.g., `sections/newpage/`)
2. Create an `index.html` file with the section content
3. Add the section name to the sections array in the main `index.html` file
4. Add a navigation link in the header

## Error Handling
The site includes a custom 404 error page located in the `error/` directory, which maintains the same design language as the main site.

## License
This project is licensed under the [Creative Commons Attribution 3.0 License](https://creativecommons.org/licenses/by/3.0/), which allows for:
- Personal and commercial use
- Modifications and adaptations
- Distribution

The license requires attribution to the original creator (HTML5 UP).

## Cloud Academy Integration
This repository is designed to be used with Cloud Academy labs, providing a practical example of a static website deployment. Students can use this codebase to learn about:
- Static website hosting
- Front-end web development
- Responsive design principles
- Modern web technologies
- Modular content organization 