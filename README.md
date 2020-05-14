<center>🚧 Work in progress 🚧</center>

# OLDP BEFR: Belgian French Theme for Open Legal Data
Unofficial fork from OLDP-DE, which can be found here: https://github.com/openlegaldata/oldp-de

Goal of this repo is to provide an up-to-date belgian template for OLDP.


## Getting Started

Installation over `pip` directly from Github:

```
pip install git+https://github.com/openjusticebe/oldp-de.git
```

Alternatively, you could `git clone` this repository and install it locally:

```
git clone https://github.com/openjusticebe/oldp-de.git
cd oldp-de
python setup.py install
```

Tell OLDP to use the OLDP-DE settings file and development configuration:

```
export DJANGO_SETTINGS_MODULE=oldp_fr.settings
export DJANGO_CONFIGURATION=DevFR  # For production use `ProdFR`
```

Start OLDP as always (from OLDP directory):

```
# Run from OLDP directory
python manage.py runserver
```

## How does it work?

By loading another settings file, we basically just tell Django to use assets (templates, images, ...) from the theme if then exist.
As a result, we can modify the layout etc. without touching the original OLDP code.
