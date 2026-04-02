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
├── submission.html      # Submission page
├── venue.html           # Venue page
└── contact.html         # Contact page template
```