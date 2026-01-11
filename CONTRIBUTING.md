# Contributing to SciPy India Website

Thank you for your interest in contributing! This guide will help you get started to contribute to the SciPy India's website.

## Quick Start

### Setup

1. **Fork and clone the repository**

   ```bash
   git clone https://github.com/YOUR-USERNAME/scipy-india.github.io.git
   cd scipy-india.github.io
   ```

2. **Install pre-commit hooks** (optional but recommended)

   ```bash
   pip install pre-commit
   pre-commit install
   ```

### Running Locally

**Option 1**: Open `index.html` directly in your browser

**Option 2**: Use a local server (recommended)

```bash
# Python
python -m http.server 8000

# Node.js
npx http-server
```

Then visit `http://localhost:8000`

## Making Changes

1. **Create a branch**

   ```bash
   git checkout -b feature/your-feature-name
   ```

2. **Make your changes** and test locally

3. **Commit with clear messages**

   ```bash
   git commit -m "Add community call blog post"
   ```

4. **Push and create a Pull Request**

   ```bash
   git push origin your-branch-name
   ```

## Project Structure

```
scipy-india.github.io/
├── index.html              # Homepage
├── blogs.html              # Blog listing
├── coc.html                # Code of Conduct
├── contact.html            # Contact page
├── style.css               # All styles
├── navigation.js           # Navigation logic
├── events.js               # Event display
├── blogs.js                # Blog rendering
├── event_details.json      # Event data
├── blogs/                  # Blog content (Markdown)
└── assets/                 # Images and static files
```

## Common Tasks

### Adding a Blog Post

1. Create `blogs/your-post.md`
2. Write your content in Markdown
3. Update blog listing in `blogs.html` if needed

### Adding an Event

Edit `event_details.json`:

```json
{
  "title": "Event Name",
  "day": "Day 1",
  "date": "DD Month, YYYY",
  "time": "HH:MM AM/PM IST",
  "location": "Online or venue",
  "cfp_link": "URL",
  "rsvp_link": "URL",
  "livestream_link": "URL"
}
```

## Code Quality

Pre-commit hooks automatically run checks such as:

- Trailing whitespace
- End-of-file fixes (e.g., ensuring a final newline)
- Merge conflict marker detection
- YAML/JSON validation
- Markdown linting
- Code formatting (Prettier)

Run manually:

```bash
pre-commit run --all-files
```

## Community

- **Code of Conduct**: [Read here](https://scipy-india.github.io/coc.html)
- **Issues**: Bug reports and feature requests
- **Zulip**: [Chat](https://scipyindia.zulipchat.com/)

## License

Contributions are licensed under the BSD 3-Clause License.

---

**Thank you for contributing to SciPy India! 🎉**