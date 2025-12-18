# Odin Recipes

A simple HTML site for practicing basic elements like headings, links, and images. The homepage is `index.html`; individual recipes live in the `recipes/` folder.

## Project Structure

```
odin-recipes/
├─ index.html
├─ README.md
└─ recipes/
	 ├─ injera.html
	 ├─ lasagna.html
	 └─ vegetable.html
```

## Getting Started

- Double‑click `index.html` to open it in your browser, or run in PowerShell:

```powershell
Start-Process .\index.html
```

## Navigation

- Each recipe page includes a “back home” link that returns to the homepage:

```html
<a href="../index.html">back home</a>
```

## Adding a New Recipe

1. Create a new file in `recipes/`, for example `pizza.html`.
2. Use this minimal HTML template:

```html
<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="UTF-8" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0" />
		<title>Pizza Recipe</title>
	</head>
	<body>
		<a href="../index.html">back home</a>
		<h1>Pizza Recipe</h1>
		<h2>Ingredients</h2>
		<ul>
			<li>...</li>
		</ul>
		<h2>Steps</h2>
		<ol>
			<li>...</li>
		</ol>
	</body>
	</html>
```

3. Link your new recipe from `index.html` using a relative link, e.g.:

```html
<ul>
	<li><a href="recipes/pizza.html">Pizza</a></li>
	<!-- add more links here -->
	</ul>
```

## Notes

- Use relative paths (e.g., `recipes/name.html`, `../index.html`).
- Keep file names simple (lowercase, hyphens if needed).
- No build tools required—just open the HTML files in a browser.

## Credits

Inspired by The Odin Project’s “Odin Recipes” assignment.
