# The Beavers Trust Website

Welcome to the codebase for **The Beavers Trust**, the official supporters' society for Hampton & Richmond Borough FC. This site serves as a hub for fans, providing news, updates, travel guides, and information about the Trust's activities.

## Overview

The Beavers Trust website is built using the [Hugo](https://gohugo.io/) static site generator and the [Congo theme](https://github.com/jpanther/congo). It is designed to be lightweight, responsive, and easy to maintain. The site includes:

- **News and Updates**: Regular posts about Trust activities, match previews, and club updates.
- **Fan Guides**: Detailed travel and matchday guides for away games.
- **Membership Information**: Details on how to join the Trust and member benefits.
- **Fundraising Initiatives**: Information on how fans can support the Trust and the club.
- **Contact Information**: Ways to get in touch with the Trust board.

## Features

- **Responsive Design**: Optimized for desktop and mobile devices.
- **Markdown Content**: All posts and pages are written in Markdown for simplicity.
- **Custom CSS**: Tailored styles using the `hampton.css` scheme.
- **Google Maps Integration**: Embedded maps for stadium locations and travel guides.
- **Dynamic Menus**: Configurable navigation menus via TOML files.

## File Structure

- **`/content`**: Contains all the Markdown files for pages and posts.
  - `/posts`: Blog posts, fan guides, and updates.
  - `/about`: Information about the Trust.
  - `/contact`: Contact details for the Trust.
- **`/config`**: Configuration files for Hugo.
  - `_default`: Default settings for the site, including menus, parameters, and theme options.
- **`/assets/css/schemes`**: Custom CSS for the site's color scheme.
- **`/archetypes`**: Templates for creating new content.
- **`/static`**: Static assets like images and PDFs.

## Setup Instructions

### Prerequisites

- [Hugo](https://gohugo.io/) (v0.118.2 or later)
- Git
- A text editor (e.g., VS Code)

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/JasonWStewart/beavers-trust.git
   cd beavers-trust
   ```

2. Install Hugo:
   Follow the [Hugo installation guide](https://gohugo.io/getting-started/installing/) for your operating system.

3. Run the development server:
   ```bash
   hugo server
   ```
   The site will be available at `http://localhost:1313`.

### Deployment

The site is configured for deployment to a static hosting platform. Update the `baseURL` in `/config/_default/config.toml` to match your production URL. Then, build the site:

```bash
hugo
```

The generated static files will be in the `/public` directory.

## Configuration

### Menus

Menus are defined in `/config/_default/menus.en.toml`. You can add, remove, or reorder menu items by editing this file.

### Theme

The site uses the Congo theme, imported via the Hugo module system. Customizations are applied in `/assets/css/schemes/hampton.css`.

### Parameters

Site-wide settings are configured in `/config/_default/params.toml`. Key options include:

- `colorScheme`: Defines the color scheme (set to `hampton`).
- `enableSearch`: Enables or disables the search functionality.
- `showTableOfContents`: Toggles the table of contents for articles.

## Content Creation

To create a new post, use the following command:

```bash
hugo new posts/<post-name>.md
```

Edit the generated Markdown file in `/content/posts` and add your content.

## Contribution Guidelines

1. Fork the repository and create a new branch for your changes.
2. Follow the existing code style and structure.
3. Submit a pull request with a clear description of your changes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact

For questions or feedback, please contact the Trust at [info@thebeaverstrust.com](mailto:info@thebeaverstrust.com).

---

**Up the Beavers!**
