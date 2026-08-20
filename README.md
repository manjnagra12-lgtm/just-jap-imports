# Just Jap Imports

Just Jap Imports is a responsive static site used to showcase imported japanese cars through landing page, gallery and a contact page.

## Features

- Responsive layouts for desktop, tablet, and mobile screens

- Full page layout for larger screens
![Screenshot of the large-screen layout](image-2.png)

- Mobile page layout


![Screenshot of the mobile layout](image-3.png)

- CSS-only mobile navigation using a checkbox and label


![Screenshot of the mobile navigation](image-4.png)

- Hero banner using `images/banner.jpg`
![Screenshot of the banner and navigation bar](image-5.png)

- Featured vehicle cards with prices and contact links


![Screenshot of a vehicle card](image-6.png)

- Gallery page with six vehicle cards

- CSS-only image galleries for the Celica GT, Celica GTS, and Toyota Crown

- Previous and next image controls using native radio buttons and labels
![Screenshot of the gallery controls](image-4.png)

- Native HTML form validation for name, email, and message fields
![Screenshot of HTML validation](image-7.png)

- Bootstrap Icons for the navigation logo and footer social links


![Screenshot of the navigation logo](image-8.png)
![Screenshot of the footer social icons](image-9.png)

- Purple site theme with contrast-checked button backgrounds

- Accessible image alt text, gallery labels, and social link labels
![Screenshot of accessible image text](image-10.png)


## User Stories

- As a visitor, I want to see a clear hero banner so that I immediately understand what Just Jap Imports offers.
- As a potential customer, I want to view featured vehicles with prices and descriptions so that I can identify cars that interest me.
- As a vehicle shopper, I want to open the Gallery page so that I can compare more imported Japanese vehicles.
- As a vehicle shopper, I want to use the `<` and `>` controls on each image gallery so that I can view multiple images of a vehicle.
- As a potential customer, I want to open the About section so that I can learn about the dealership and its services.
- As an interested buyer, I want to use the Contact page so that I can ask about pricing, test drives, or vehicle assistance.
- As a contact-form user, I want the form to identify missing or invalid details so that I can submit complete contact information.
- As a mobile visitor, I want to open and close the navigation menu so that I can move between pages on a small screen.
- As a visitor using assistive technology, I want images and controls to have meaningful labels so that I can understand and operate the site.

## UX Principles Applied

The site was designed around the following user experience principles:

- **Clarity:** The navigation uses familiar labels such as Home, Gallery, About, and Contact. Each page has a clear heading and a focused purpose.
- **Visual hierarchy:** The home page introduces the business with a hero banner, then presents featured vehicles, company information, and a contact call to action in a logical order.
- **Consistency:** Buttons, navigation, image controls, colours, spacing, and card layouts use shared CSS styles across all pages.
- **User control:** Visitors can move through vehicle images using visible previous and next controls without relying on JavaScript or automatic movement.
- **Responsive design:** Flexible grids, mobile navigation, and responsive typography allow the site to work across desktop, tablet, and mobile screen sizes.
- **Feedback and error prevention:** Native form validation prevents incomplete or incorrectly formatted contact details from being submitted.
- **Accessibility:** Images include alternative text, gallery controls include labels, social links include accessible names, and colour contrast was checked for important text and buttons.
- **Recognition over recall:** Vehicle names, prices, descriptions, and clear calls to action are displayed directly on the page so visitors do not need to remember information between sections.

## Pages

- `index.html` - Home page with hero banner, featured vehicles, About section, and contact call to action
- `gallery.html` - Vehicle gallery with three interactive image galleries
- `contact.html` - Contact form and business information

## Basic Wireframe

```text
						 JUST JAP IMPORTS
 ------------------------------------------------------------------------
 | Logo                         Home | Gallery | About | Contact          |
 ------------------------------------------------------------------------

 HOME (`index.html`)
 ------------------------------------------------------------------------
 |                         HERO BANNER                                   |
 |                    Discover Exclusive Imports                         |
 |                         [Browse Gallery]                              |
 ------------------------------------------------------------------------
 |                         FEATURED VEHICLES                             |
 |               
 ------------------------------------------------------------------------
 |                         ABOUT THE BUSINESS                             |
 |                     
                            
 ------------------------------------------------------------------------
 |                    READY TO DRIVE HOME YOUR DREAM CAR?                 |
 |                            [Contact Us]                                |
 ------------------------------------------------------------------------
 | Copyright                                              Social icons    |
 ------------------------------------------------------------------------

 GALLERY (`gallery.html`)
 ------------------------------------------------------------------------
 |                         PAGE HEADER                                    |
 |                           Our Gallery                                  |
 ------------------------------------------------------------------------
 | [ gallery]            [ gallery]            [ gallery]      
 | [< image >]           [< image >]           [< image >]                 |
 | [price]               [price]               [price]                    |
 | [Get in touch]        [Get in touch]        [Learn More]               |
 |                                                                        |
 | [Additional vehicle cards...]                                           |
 ------------------------------------------------------------------------
 | Copyright                                              Social icons    |
 ------------------------------------------------------------------------

 CONTACT (`contact.html`)
 ------------------------------------------------------------------------
 |                         PAGE HEADER                                    |
 |                          Contact Us                                    |
 ------------------------------------------------------------------------
 | CONTACT FORM                         CONTACT INFORMATION               |
 | [Your Name]                          Phone                             |
 | [Your Email]                         Email                             |
 | [Your Message]                       Address                           |
 | [Send Message]                                                         |
 ------------------------------------------------------------------------
 | Copyright                                              Social icons    |
 ------------------------------------------------------------------------
```

## Project Structure

```text
just-jap-imports/
|-- index.html
|-- gallery.html
|-- contact.html
|-- styles.css
|-- images/
|   |-- banner.jpg
|   |-- celicagt*.jpg
|   |-- celicagts*.jpg
|   |-- crown*.jpg
|   |-- 1994toyotasupraa80.webp
|   |-- 2022supra.webp
|   `-- 1994supraa80.jpeg
`-- README.md
```

## Image Galleries

The gallery page uses CSS radio-button state changes rather than JavaScript:

- Velocity Sports uses the `celicagtb` image set.
- The sedan gallery uses the `celicagts` image set.
- The SUV gallery uses `crown.jpg` through `crown6.jpg`.

Each gallery has visible `<` and `>` controls. The checked radio input selects the visible image and the corresponding controls.

## Styling

All styling is contained in `styles.css`, organized into shared, home-page, gallery-page, contact-page, and responsive sections.

- Primary purple: `#667eea`
- Dark button purple: `#5568d3`
- Gradient purple: `#764ba2`
- White navigation text with purple hover state
- Dark navigation and footer backgrounds
- Responsive breakpoints at `768px` and `480px`

The darker button purple provides a white-text contrast ratio of approximately `4.88:1`.

Bootstrap Icons are loaded from jsDelivr CDN links in the HTML files. The project therefore needs an internet connection for the external icon resources when opened locally. Bootstrap CSS is also loaded on `index.html`.

## Form Validation

The contact form uses native HTML validation:

- Name is required and must contain at least two characters.
- Email is required and must use a valid email format.
- Message is required and must contain at least ten characters.

The form uses a `mailto:` action, so sending requires a configured email client. The current contact page also includes an inline confirmation handler on the submit button.

## Run Locally

1. Open the project folder in VS Code.
2. Open `index.html` in a browser, or use the Live Server extension.
3. Use the navigation links to visit the gallery and contact pages.

## GitHub

The project uses the following GitHub remote:

```text
https://github.com/manjnagra12-lgtm/just-jap-imports.git
```

To publish later changes:

```bash
git add .
git commit -m "Describe your changes"
git push
```

## Browser Support

The site is intended for current versions of Chrome, Edge, Firefox, and Safari, as well as modern mobile browsers with changes implimentled for view in mobile.




## Testing
-The code has been regularly debugged and checked in co pilot chat.
-The layout has been regularly checked in browsers to ensure key functionality stays with every build and push.
-Validation through W3 validator found errors in the HTML code :


![3 errors located](image-11.png)


- Errors have been fixed :


![no errors](image-12.png)


-Gallery Page errors found on [W3 validator ](https://validator.w3.org/nu/#textarea) these have not been removed due to wanting the site to have better fuctionality for screenreaders acessibility regarding main controls. 


![errors found](image-13.png) [W3 validator ](https://validator.w3.org/nu/#textarea) 



- Contact page errors found on [W3 validator ](https://validator.w3.org/nu/#textarea) i have not made changes to the code as i find that these are cosmetic and accessability issues and not code breaking issues. 



![errors found](image-14.png)


-CSS code checked via W3 validator :


![CSS review of code](image-15.png)


## Credits

Development was supported with Copilot, Chat GPT and Google research. The `images` folder contains a mix of self-taken and externally sourced images from google and pinterest used to showcase the vehicles. 

## Use of AI
-Code for rotating photos in gallery created using copilot chat to support more images in a tighter space while not sacrificing the page layout we desired.
-The use of AI allowed me to focus on key functionality bringing to life a more robust and interactive site and landing page, the code has gone through afew iterations and been cleaned up with AI support to help easily and effeciently section off code designed for each section, this also allowed for moving on with key aspects of the site. 
-AI used to help neeten up code and to section off Code areas.

![alt text](image-1.png)

-AI used to support CSS and flexbox positioning issues for site and key placements.


## License

Free to use and modify for personal or commercial projects.
