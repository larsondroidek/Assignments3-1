# Assignment 3.1 — Solution: Two-Page Website with Working Links

## Steps
1. Create a folder `two-page-website` and open it in VS Code.
2. Create `index.html` and `about.html` in the **same folder** (so `href="about.html"` works).
3. Paste the code below, replace "Your Name", and open with Live Server.
4. Click Home, About and the external link to test them.

## index.html
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Code Corner — Home</title>
  </head>

  <body>
    <!-- ===== Website name ===== -->
    <header>
      <h1>Code Corner</h1>

      <!-- ===== Navigation bar ===== -->
      <nav>
        <a href="index.html">Home</a> |
        <a href="about.html">About</a> |
        <!-- External link: opens in a new tab, secured with rel -->
        <a href="https://developer.mozilla.org" target="_blank" rel="noopener noreferrer">MDN Web Docs</a>
      </nav>
    </header>

    <hr />

    <main>
      <!-- ===== Introduction ===== -->
      <h2>Welcome!</h2>
      <p>
        Hello and welcome to <strong>Code Corner</strong>, a small website where
        I share what I learn while studying web development. Use the navigation
        bar above to visit the <a href="about.html">About</a> page, or explore
        the
        <a href="https://developer.mozilla.org" target="_blank" rel="noopener noreferrer">MDN Web Docs</a>
        to learn more about HTML.
      </p>
    </main>

    <hr />

    <footer>
      <p><small>&copy; 2026 Code Corner</small></p>
    </footer>
  </body>
</html>
```

## about.html
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Code Corner — About</title>
  </head>

  <body>
    <header>
      <h1>Code Corner</h1>

      <!-- Same navigation bar as the home page -->
      <nav>
        <a href="index.html">Home</a> |
        <a href="about.html">About</a> |
        <a href="https://developer.mozilla.org" target="_blank" rel="noopener noreferrer">MDN Web Docs</a>
      </nav>
    </header>

    <hr />

    <main>
      <h2>About This Website</h2>
      <p>
        Code Corner is a practice project built with <strong>HTML only</strong>.
        It has two pages connected with links, and an external link that opens
        in a new tab.
      </p>

      <h3>About the Author</h3>
      <p>
        My name is <strong>Your Name</strong> and I am learning web development.
      </p>

      <p><a href="index.html">&larr; Back to Home</a></p>
    </main>

    <hr />

    <footer>
      <p><small>&copy; 2026 Code Corner</small></p>
    </footer>
  </body>
</html>
```

## Requirements Checklist
| Requirement | Where it is met |
|-------------|-----------------|
| `index.html` and `about.html` | Two files in the same folder |
| Website name, introduction, nav bar on home page | `<h1>Code Corner</h1>`, "Welcome!" paragraph, `<nav>` |
| Home and About links | `<a href="index.html">`, `<a href="about.html">` |
| Pages connected with `<a href="">` | Nav on both pages + "Back to Home" link |
| External link | `https://developer.mozilla.org` |
| `target="_blank"` + `rel="noopener noreferrer"` | On every external link |

## Key Concepts
- **Relative link** (`href="about.html"`): points to a file in the same project.
- **External link** (`href="https://..."`): full URL to another website.
- **`target="_blank"`** opens the link in a new tab.
- **`rel="noopener noreferrer"`** stops the new page from accessing `window.opener` (security) and hides the referrer.

## Submission
- ✅ `index.html` and `about.html` (attached)
- 📸 Screenshot of the working website (home page with nav bar; optionally the About page too)
