# ICQMC 2026 - Jekyll Site

ICQMC website built with Jekyll.

## Setup

1. Install Ruby and Bundler if you haven't already
2. Install dependencies:
   ```bash
   bundle install
   ```

## Local Development

To run the site locally:

```bash
bundle exec jekyll serve
```

Then visit `http://localhost:4000` in your browser.

## Build for Production

To build the static site:

```bash
bundle exec jekyll build
```

The generated site will be in the `_site` directory.

## GitHub Pages Deployment

This site is ready to be deployed on GitHub Pages:

1. Push this directory to a GitHub repository
2. Go to Settings → Pages
3. Set Source to "Deploy from a branch"
4. Select the main/master branch
5. GitHub will automatically build and deploy the site

## Editing Content

### ✨ **All content is now managed through YAML data files!**

You can update conference information by editing YAML files in the `_data/` directory - **no HTML editing required**.

### Conference Information

Edit `_data/conference.yml`:

```yaml
name: "ICQMC"
short_name: "ICQMC 2026"
dates: "August 23-27, 2026"
venue: "Oriental Hotel, Jeju Island, Korea"
email: "icqmc2026@gmail.com"
about: "Conference description..."
```

### Important Dates

Edit `_data/dates.yml`:

```yaml
- name: "Minisymposium Proposals Deadline"
  date: "March 31, 2026"

- name: "Abstract Submission Deadline"
  subtitle: "(Minisymposium, Contributed Talks, and Posters)"  # Optional subtitle
  date: "May 31, 2026"
```

**To add a new date**: Simply add a new entry to the list.

### Committee Members

Edit `_data/committees.yml`:

```yaml
local_chairs:
  - name: "Minseok Choi"
    affiliation: "POSTECH"

local_organizing:
  - name: "Sehun Chun"
    affiliation: "Yonsei University"

scientific:
  - name: "Name"
    affiliation: "Institution"
```

**To add a member**: Add a new entry under the appropriate section.

### Registration Fees

Edit `_data/registration.yml`:

```yaml
categories:
  - name: "General participants"
    early_bird: "350 USD"
    early_deadline: "June 15"
    regular: "400 USD"
```

**To add a category**: Add a new entry to the categories list.

### Organizer Logos

Edit `_data/organizers.yml`:

```yaml
- name: "NIMS"
  logo: "logo_nims.png"
  alt: "NIMS Logo"
```

**Note**: Logo images should be placed in `assets/images/`.

## Directory Structure

```
.
├── _config.yml          # Site configuration
├── _data/               # 📝 Edit these YAML files to update content
│   ├── conference.yml   # Basic conference info
│   ├── dates.yml        # Important dates
│   ├── committees.yml   # Committee members
│   ├── registration.yml # Registration fees
│   └── organizers.yml   # Organizer logos
├── _layouts/            # Page templates
│   └── default.html
├── _includes/           # Reusable components
│   ├── navigation.html
│   └── footer.html
├── assets/              # Static files
│   ├── css/
│   │   └── style.css
│   └── images/
├── index.html           # Home page template
├── committees.html      # Committees page template
├── registration.html    # Registration page template
├── speakers.html        # Speakers page
├── minisymposiums.html  # Mini-symposiums page
├── submission.html      # Submission page
├── venue.html           # Venue page
└── contact.html         # Contact page template
```

## Conference Information

- **Dates:** August 23-27, 2026
- **Location:** Oriental Hotel, Jeju Island, Korea
- **Contact:** easiam2026@gmail.com
