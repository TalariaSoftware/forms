# Forms

Tools to make goverments more responsive, effective, and efficient by making it easier for constituents to fill out forms.

## Why

For most government services, in order to receive them, a person is required to submit a request that includes all of the information the government agency needs to fulfill the request. Agencies have a standardized document for each type of request, a form.

In the long ago time, the only way to submit a form was to visit the agency in question, get a paper copy of the form, make marks on it with a typewriter and/or a ballpoint pen, and then return it to the agency. This is less than optimal; it is slow, error-prone, and onerous. As such it makes it difficult for people, especially marginalized people, to request and recieve government services.

The information age has improved the situation somewhat. Some agencies offer webforms or even native apps for people to make requests. But for the most part, paper forms still rule, though they are usually downloadable as PDF files and sometimes even fillable PDFs. The process is still slow and difficult, especially for people with low bandwidth, small screens, slow devices, accessibiility needs, and/or language barriers.

The goal of this project is to give governments a tool they can use to make it easier for the public to submit forms. 

## Roadmap

### Proof of concept

A user can go to the page for a form, fill out an HTML form, and recieve a completed PDF with their info.

### MVP

A user can start with a fillable PDF file, and create a page with an HTML form that can be filled out to recieve a completed PDF.

### Later Improvements

- Field input types (string, text, date, boolean, number, etc.)
- Customize HTML form layout
- Non-fillable PDF files
- Duplicated data (i.e. typing your social security number once puts it on every page)
- Derived data (i.e. enter 1 dependent spouse and 2 dependent children, and get 3 dependents total automatically)
- Form submission (email, file storage, webhook, etc.)
- Related / suggested forms

## Requirements

Law and policy create a long list of largely-immutable requirements for government technology.

### Static pages

Forms MUST be delopyable as static pages.

It is possible for governments to spin up servers and run code on them but security requirements make the process complicated, onerous, and slow. In order for Flow to be usable it needs to be able to be deployed as static pages with no server-side processing required. 

### Local data

User data MUST never leave the user's local machine.

All user data is "Restricted information." It would cause tangible detremental effects if it were made available to the public or any unauthorized persons. As a result, extreme care would need to be taken regarding any user data that leaves the user's device. Thus, in order for Flow to be usable it cannot transmit any user data away from the user's device.

### Accessibility

Forms MUST be accessible to people with disabilities.

All government services must be accessible to people with disabilities. In many jurisdictions this requirement is codified into law, for example Section 508 of the Rehabilitaion Act.

#### Resources
[Create Accessible Digital Products](https://section508.gov/create)
[Guide to Accessible Web Design & Development](https://www.section508.gov/content/guide-accessible-web-design-development)
[18F Accessibility Guide](https://accessibility.18f.gov)
[Accessibility for Teams](https://accessibility.digital.gov)
[US Web Design System](https://designsystem.digital.gov)

### Translations

Forms MUST be available in multiple languages.

Government services must be accessible to people in the language they speak. In many jurisdictions this requirement is codified into law. For example, New York City has ten official languages and must provide access in each of those ten languages.
