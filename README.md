# Come-of-Age
A non profit organisation that is dedicated to teaching fundamental skills and requirements as they grow into adults. Learning how to Adult is not fully taught while in full time education, which is why this organisation provides valuable knowledge, to see today's generation is set up for success. They provide in person lectures and workshops relating to: Personal Finance, Job Searching and CV writing, House Keeping, and Raising a Family. 

This README is used to document the progress of the project and the usage of the website. Other developers of this project can refer to this document in order to better understand this project and its goals. Please make regular changes to this document when making further changes to the project.

## Project Goals

### Business Goals
* Increase the number of clients
* Expand the reach of the brand
* Establish a presence online
* Provide relevant and useful links to online resources

### User Goals
* Responsive Website so it can be used on all platforms
* A means of contacting the business 
* A place to book upcoming workshops 
* Infromation about the workshops and lectures 

## User Experience

### User Stories
1. As a student, I want a responsive website so I can view on my phone and computers at school.
2. As a school staff member, I need a simple form to contact the organisation so I can coordinate workshops and lectures for students.
3. As a student, I need a clear list of workshops so I can find the one i need easily.
4. As a student, I would like to sign up to a newsletter so i can find up-to-date information about future workshops and events.
5. As a potential client, I need to see clear images and layout so I can better understand the information given on the site.
6. As a teacher, I would like to see a number of links to social media and online resourses so i can see if booking  a workshop is good for my students.
7. as A student , I want to read testemonials from these workshops to see if joining one is right for me.
8. As a client, I need there to be a user friendly layout and navigation so I can quickly find the information I need about the services provided.

### Features on release

1. A simple navigation bar that colapses into a drop down on small screens
2. sign-up form for newsletter
3. responsive website for all devices
4. contact form for feedback and inquiries
5. footer with links to social media

### Design 

#### Colour Scheme

![image of colour scheme](/design%20docs/colour%20scheme.png) 

* Primary Text - #032b2d (charcoal)
* Secondary Text - #263a45 (Dark navy)
* Highlight Text - #f2f5f8 (off-white)
* Background - #b6e2ec (pale blue)
* Header and footer - #09747b (dark turquoise)
* contrast - #dc6413 (orange)

Chosen through [Colour Picker](https://imagecolorpicker.com/) using image generated through [Gemini](https://gemini.google.com/)
![Inspiration image Gemini Generated](/design%20docs/Inspiration%20image%20Generated%20through%20Gemini.jpg)
Using following prompt

"Realistic photograph of a bright, airy life skills workshop for late teenagers in a modern community centre. A friendly teacher in a turquoise shirt stands at the front, clearly visible and fully in frame, mid-demonstration and smiling. Around them, a group of engaged 17 to 19-year-olds sit at shared tables, taking notes, asking questions, and working on practical tasks such as a budgeting worksheet, a laptop with a CV template, and a simple cooking setup. Large windows flood the room with natural daylight, and the lighting is bright, even, and neutral. Casual, relaxed, and welcoming atmosphere, diverse group, shallow depth of field, 35mm lens, high resolution, photorealistic."

Assisted by [Claude](https://claude.ai/) 


#### Typography

![Image of Fonts from Google Fonts](/design%20docs/Fonts.png)

Chosen and linked from [Google fonts](https://fonts.google.com/share?selection.family=Overlock:ital,wght@0,400;0,700;0,900;1,400;1,700;1,900|Ranchers)

* Titles -  Ranchers - Bold and loud while still very readable.

* Secondary - Overlook - Has a hand-written look to it with rounded edges but is still sophisticated and readable. 


CSS code for fonts 

@import url('https://fonts.googleapis.com/css2?family=Overlock:ital,wght@0,400;0,700;0,900;1,400;1,700;1,900&family=Ranchers&display=swap');


#### Images

Stock images are taken from [iStockphoto](https://www.istockphoto.com/)

#### Wireframes

Created using [Whimsical](https://whimsical.com/slhcode/home-page-12XEufmVGuGHgjxTAYmH9c)

Home page
![Homepage](/design%20docs/wireframes/Home%20page%20wireframe%202.png)
Workshops
![Workshops](/design%20docs/wireframes/Workshops%20wireframe%202.png)
Lectures
![Lectures](/design%20docs/wireframes/Lectures%20wireframe%202.png)
ContactUs
![ContactUs](/design%20docs/wireframes/Contact%20us%20wireframe%202.png)
Booking Workshop
![BookWorkshop](/design%20docs/wireframes/Book%20your%20Workshop%20wireframe.png)
Booking Success
![BookingSuccess](/design%20docs/wireframes/booking%20Success%20wireframe%20.png)

## Technologies
### Site Build
* HTML - Using semantic design for accessiblity 
* CSS - Stylesheets 
* Javascript (using [Bootstrap 6.0](https://getbootstrap.com/)) - navigation, forms and responsive design
* VS Code - Text/code editor
* Chrome web tools - debugging


### Documentation

* Git/Github - Versioning, Project management, Deployment
* Whimsical - Wireframing 

### Assets

* Gemini - AI Image generation
* Claude - text generation for site and prompts for gemini
* Pixabay - Royalty Free Stock Images
* Image Color Picker - Colour scheme for site
* Google fonts - Fonts for site
* Fontawesome - Icons 
* Favicon.io - Favicons
* Pixlr - Free image format convertion

## Bugs

### 1. Main not covering the full width of view port
![bug 1](/documentation/bugs/bug%201.png)

This was caused by the width of "body" tag not being defined properly in style.css. After manuel testing of the "main" tag, the body tag was deemed to be the root cause.

### 2. Header not showing at the top under nav bar
![bug 2](/documentation/bugs/bug%202.png)

This was caused when applying "position: fixed" to the "nav" tag. "position: sticky" was tested and did not work. after consulting code institute lms learning platform, applying "margin-top: 65px" to "header" tag fixed this issue. 

### 3. scroll on various bits of text
![bug 3](/documentation/bugs/bug%203.png)

This affected is believed to be affected by the global styling used in all pages and in each section. It is possible that the global style for "overflow-y: hidden". this styling was removed and was not the cause. Using ai assistance in google web tools, "overflow: hidden !important" was added to any affected elements. this fixed this bug for now but needs further diagnois to find the root cause.

### 4. clipping of text in the footer
![bug 4](/documentation/bugs/bug%204.png)

This was found while testing responsiveness in web tools. this appears if the width of the view-port is 576px - 715px. this is caused by the padding applied to the "footer" elements. This can be fixed by using a media query for these elements to change the spacing between these width levels, also by altering padding or applying text-wrapping to ".footer-info". However, due to time constraints, and the fact that this range was deemed uncommon for modern device view-ports, this will be fixed in a future build.

### 5.Main body not filling remaining space of viewport
![bug 5](/documentation/bugs/bug%205.png)

Found while testing tablet presets in web tools. A fix for this was found on stackoverflow https://stackoverflow.com/questions/90178/make-a-div-fill-the-height-of-the-remaining-screen-space. 

### 6. nav dialog menu pinned to the right 
![bug 6](/documentation/bugs/bug%206.png)

This was found using the ipad mini preset in web tools. its cause by a bootstrap class "md:justify-content-end" in "dialog" not synced with the colapsing functionality of the bootstrap nav. Testing by changing this class to "sm:" and "lg" but was not fixed. Another possible fix for this could be a media query to added to this element to overwrite bootstrap, but due to time constraints, this must be added in a future build.
