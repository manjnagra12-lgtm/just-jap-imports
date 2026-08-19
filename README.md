# Just Jap Imports

A responsive static website for showcasing imported Japanese cars, including featured vehicles, a gallery, and a contact page.

## Features

- Responsive layout for desktop, tablet, and mobile screens
- Sticky navigation with mobile menu toggle
- Hero banner using `images/banner.jpg`
- Featured vehicle cards with vehicle images and pricing
- Gallery page with additional vehicle listings
- Contact page with enquiry form and business details
- Bootstrap Icons for navigation and social media links
- Smooth scrolling and hover transitions
- Accessible labels and tooltips for social media icons

## Pages

- `index.html` - Home page with hero banner, featured vehicles, and About section
- `gallery.html` - Full vehicle gallery
- `contact.html` - Contact form and contact information

## Project Structure

```text
just-jap-imports/
|-- index.html
|-- gallery.html
|-- contact.html
|-- styles.css
|-- images/
|   |-- banner.jpg
|   |-- celicagt.jpg
|   `-- 2022supra.webp
`-- README.md
```

## Vehicle Images

The default featured vehicle image is `images/celicagt.jpg`. The SUV card uses `images/2022supra.webp` through the targeted `.car-image.suv::before` rule in `styles.css`.

To add or change a vehicle image, update the relevant CSS selector and image path. Keep the image path relative to `styles.css`.

## Styling

All styling is contained in `styles.css`. The current visual system includes:

- Purple primary color: `#667eea`
- Purple gradient color: `#764ba2`
- White navigation text with purple hover state
- Dark navigation and footer backgrounds
- Responsive breakpoints at `768px` and `480px`

Bootstrap 5 and Bootstrap Icons are loaded from jsDelivr CDN links in the HTML files, so an internet connection is needed for those external resources when opening the pages locally.

## Run Locally

1. Open the project folder in VS Code.
2. Open `index.html` in a browser, or use the Live Server extension.
3. Use the navigation links to visit the gallery and contact pages.

The contact form currently uses a `mailto:` action and requires a configured email client to send messages.

## GitHub

This project is tracked on the `main` branch and uses the following remote repository:

```text
https://github.com/manjnagra12-lgtm/just-jap-imports.git
```

To commit and publish later changes:

```bash
git add .
git commit -m "Describe your changes"
git push
```

## Browser Support

The site is intended for current versions of Chrome, Edge, Firefox, and Safari, as well as modern mobile browsers.

## Support Recieved
I have utilised copilot for support with coding and google for support in building site fuctionalities along with other aspects of design and content i.e images housed in images folder both self taken and also found online to showcase on site. 

## License

Free to use and modify for personal or commercial projects.
