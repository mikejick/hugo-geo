## Dependencies
- Hugo v0.14 or better
- LESS if you wish to compile the custom CSS

## Features
- Use `highlight = true` in the front matter to include [highlight js](https://highlightjs.org/) javascript and css files.
- In the front matter, use `index = true` on the first post in a tutorial series to make that content the "index" page for the rest of the series
- Include custom scripts and css on individual pages in front matter like so:
```toml
scripts = [
"//cdnjs.cloudflare.com/ajax/libs/highlight.js/8.8.0/languages/go.min.js",
]

css = [
"//cdn.leafletjs.com/leaflet/v0.7.7/leaflet.css"
]
```

## Site Config
These are my `config.toml` settings:

```toml
BaseURL = "https://base-url-here/"
relativeURLs = false
languageCode = "en-us"
title = "SiteTitle.Com"
disqusShortname = "*****"
paginate = 5

[taxonomies]
	tag = "tags"
	tutorial = "tutorials"

[params]
	# Include favicon
	favicon = "favicon.ico"
 	
	# Google Analytics
	analytics = "SHORT-CODE-HERE"

	# Email (optional)
	email = ""
	
	# Header Title for the main page
	header = "What I'm Thinking"
	
	# Sidebar profile picture
	profilepic = "img/smugmug.jpg"
	
	# Title/subtitle for the sidebar
	title = ""
	subtitle = ""
	
	# Social buttons for sidebar
	# Each of these are optional
	[[params.socialbuttons]]
	faicon = "github"
	url = "https://github.com/"
	[[params.socialbuttons]]
	faicon = "twitter"
	url = "https://twitter.com/"
	[[params.socialbuttons]]
	faicon = "linkedin"
	url = "https://linkedin.com"
	[[params.socialbuttons]]
	faicon = "google-plus"
	url = "https://plus.google.com/+YourID"

	# Nav links below the profile picture
	[[params.navlinks]]
	name = "About"
	url = "about/"
	
	[[params.navlinks]]
	name = "Blog"
	url = "posts/"
	
	[[params.navlinks]]
	name = "Tutorials"
	url = "tutorial/"
```
