# Blog template

Blog template for hosting on GitHub Pages.

Based on [Minimal Mistakes Jekyll theme](https://mmistakes.github.io/minimal-mistakes/).

Detailed documentation can be found [here](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/).

## Runnng locally

Make sure you go through the [Jekyll installation guide](https://jekyllrb.com/docs/installation/).

### Configuration

The `_config_local.yml` file contains the configuration for the local server.

The `_config.yml` file contains the configuration for the GitHub Pages server.

**Make sure to update both files** with your information.

### Install dependencies

```bash
bundle --gemfile Gemfile.local
bundle install --gemfile Gemfile.local
```

### Serving @localhost

```bash
# osx and linux
BUNDLE_GEMFILE=Gemfile.local bundle exec jekyll serve --config _config_local.yml

# or in windows command line
set BUNDLE_GEMFILE=Gemfile.local
bundle exec jekyll serve --config _config_local.yml
```

Go to `http://localhost:4000` in your browser.

## Serving on GitHub Pages

Rename the repository to `<username>.github.io` and enable GitHub Pages in the repository settings.

The repository must be public.

Push your changes to the `master` branch and GitHub will take care of the rest.
