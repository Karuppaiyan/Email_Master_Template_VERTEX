# Email_Master_Template_VERTEX

Responsive HTML email templates for Vertex Pharmaceuticals Incorporated, built for cross-client compatibility including Outlook Desktop (Word rendering engine).

## Setup

1. Clone the repo
```bash
git clone <repo-url>
cd Email_Master_Template_VERTEX
```

2. No build step required — these are static HTML files using table-based layouts and inline CSS (required for Outlook compatibility). Open any `.html` file directly in a browser to preview.

## Usage

1. Pick the template you need from the templates folder.
2. Edit content directly in the HTML — replace placeholder text, images, and links.
3. **Keep all styling inline** (`style="..."` attributes) — Outlook Desktop strips `<style>` blocks and external CSS, so avoid adding classes or `<style>` tags for anything critical to rendering.
4. Replace image `src` paths with hosted URLs (image assets must be publicly accessible — email clients don't render local/relative image paths).

## Testing before sending

- Test across Outlook (Desktop + Web), Gmail, Apple Mail, and mobile clients before a real send. Recommended tools:
  - [Litmus](https://litmus.com) or [Email on Acid](https://www.emailonacid.com) — paid, most thorough cross-client preview
  - Send a test to a personal Outlook.com and Gmail account as a free manual check

## Reference resources

- [Outlook Responsive Email guide](https://learn.microsoft.com) — official guidance on responsive design constraints in Outlook
- [Sendinblue free HTML templates](https://www.sendinblue.com) — free mobile-friendly templates for reference
- [Beefree](https://beefree.io) — drag-and-drop builder with Outlook-optimized export

## Notes

- Outlook Desktop uses Word's rendering engine — avoid CSS3 (flexbox, grid, background images via CSS) and stick to table layouts with inline styles.
- Keep total email width to 600–650px for consistent rendering across clients.
