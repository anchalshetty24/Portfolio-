# Anchal Shetty — Portfolio Website

A responsive personal portfolio built for the YR NOVATECH internship.
It presents my skills, projects, education, and contact details as a software developer.

**Live site:**  https://anchalshetty24.github.io/Portfolio-/   
**Repository:**  https://github.com/anchalshetty24/Portfolio-

## Sections

- **Navbar:** sticky, highlights the section you're viewing, and collapses into a menu on phones
- **Hero:** name, role, availability for internships, and links to Projects and Contact
- **About:** who I am and what I'm looking for
- **Skills:** programming, tools, and working-style skills as tags
- **Projects gallery:** a featured project (Shakthi, a women's safety app presented at Project Expo 2026,task-manager) and a card layout for adding more
- **Education:** BCA, XII, and X
- **Contact:** email, LinkedIn, phone, and a form with validation

## Tech

- HTML, CSS, and vanilla JavaScript in a single `index.html` (no frameworks or build step)
- Google Fonts: Fraunces, Inter, and IBM Plex Mono

## My approach

1. **Start with content.** I wrote the sections from my real background first, then designed around them.
2. **Keep the design simple.** A calm palette (paper, ink, and teal with one coral accent), a serif for headings, and lots of whitespace so the content stands out.
3. **Mobile first.** The layout uses flexible grids (`auto-fit`), `clamp()` for text sizes, and one breakpoint for the navbar menu and contact layout.
4. **Accessible by default.** Semantic HTML, visible keyboard focus, labelled form fields, error messages announced to screen readers, and reduced-motion support.
5. **Validate forms on the client.** The contact form checks each field when you leave it and again on submit:
   - Name: at least 2 characters
   - Email: must look like a valid address
   - Message: at least 10 characters

   Errors appear under the field and the first invalid field gets focus.

## How the contact form sends messages

The site is static, so there's no server to receive form data. After validation passes, the form opens the visitor's email app with the message filled in (`mailto:`). To receive messages directly instead, connect the form to a service like Formspree or Netlify Forms.

## Run locally

Open `index.html` in a browser. No setup needed.

## Deploy on GitHub Pages

1. Create a new public repository on GitHub, for example `portfolio`.
2. Upload `index.html` and `README.md` to it.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select the `main` branch and the `/ (root)` folder, then save.
5. After a minute or two, your site is live at `https://<your-username>.github.io/portfolio/`.

## Adding a new project

In `index.html`, find the `<div class="gallery">` block, copy an existing `project-card`, and change the title, description, and tags. Remove the `planned` class once the project is done.
