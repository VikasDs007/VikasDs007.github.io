# Contributing Guidelines

Thank you for your interest in contributing! This is an **open-source project** and we welcome improvements from the community.

---

## 🤝 Ways to Contribute

### 1. **Report Bugs**
Found an issue? Let us know!
- Open an **Issue** on GitHub
- Describe the problem clearly
- Include screenshots if possible
- Specify your browser/OS

### 2. **Suggest Features**
Have an improvement idea?
- Open an **Issue** with the label `enhancement`
- Explain the feature and why it would help
- Provide examples if relevant

### 3. **Improve Code**
Want to contribute code?
- Fork the repository
- Create a feature branch
- Make improvements
- Submit a Pull Request

### 4. **Improve Documentation**
Help make setup easier for others
- Update SETUP.md with clearer instructions
- Add troubleshooting guides
- Improve README.md
- Fix typos

### 5. **Add Examples**
Show how to customize the portfolio
- Add case studies of customizations
- Create video tutorials
- Document design changes
- Share tips & tricks

---

## 🚀 Quick Contribution Process

### Step 1: Fork the Repository

```bash
# Go to https://github.com/VikasDs007/VikasDs007.github.io
# Click "Fork" button
```

### Step 2: Clone Your Fork

```bash
git clone https://github.com/YOUR-USERNAME/VikasDs007.github.io.git
cd VikasDs007.github.io
```

### Step 3: Create a Feature Branch

```bash
git checkout -b feature/your-improvement-name
# Example: feature/add-dark-mode-toggle
```

### Step 4: Make Your Changes

Edit files and test locally:

```bash
python3 -m http.server 8080 --bind 127.0.0.1
# Visit http://localhost:8080 to test
```

### Step 5: Commit Your Changes

```bash
git add .
git commit -m "Concise description of changes"
# Example: "Fix mobile button touch targets"
```

### Step 6: Push to Your Fork

```bash
git push origin feature/your-improvement-name
```

### Step 7: Create a Pull Request

1. Go to the original repository
2. Click **"Compare & pull request"**
3. Describe your changes
4. Submit!

---

## 📋 Pull Request Guidelines

### Before Submitting

- [ ] Code is tested locally
- [ ] No breaking changes
- [ ] Follows existing code style
- [ ] Comments explain complex logic
- [ ] Documentation is updated
- [ ] No console errors

### Describe Your PR

```markdown
## Description
Brief explanation of what this PR does.

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Documentation improvement
- [ ] Performance improvement

## Testing
How did you test this?
- [ ] Tested locally on desktop
- [ ] Tested on mobile
- [ ] No breaking changes

## Related Issues
Fixes #123 (if applicable)
```

### Good PR Examples

✅ **"Fix: improve mobile button accessibility - increase touch targets to 48px"**

✅ **"Feature: add dark/light theme toggle with local storage persistence"**

✅ **"Docs: clarify GitHub Pages setup process with screenshots"**

❌ **"Update"** (too vague)

❌ **"Fixed stuff"** (unclear what changed)

---

## 💡 Ideas for Contributions

### Code Improvements
- [ ] Add dark/light theme toggle
- [ ] Optimize image loading (lazy loading)
- [ ] Add keyboard navigation
- [ ] Improve form validation
- [ ] Add more animation options
- [ ] Performance optimizations

### Documentation
- [ ] Add video setup tutorial
- [ ] Create customization examples
- [ ] Add troubleshooting guide expansion
- [ ] Translate SETUP.md to other languages
- [ ] Add FAQ section

### Features
- [ ] Multiple portfolio color schemes
- [ ] Blog/article section template
- [ ] Timeline for work experience
- [ ] Interactive skill level indicators
- [ ] Project filtering/categories
- [ ] Dark mode theme

### Design
- [ ] Create alternative color palettes
- [ ] Design mobile-first layouts
- [ ] Create new hero section options
- [ ] Design responsive gallery templates

---

## 🎨 Code Style Guidelines

### HTML
```html
<!-- Use semantic HTML -->
<section id="projects">
    <h2>Projects</h2>
    <!-- Content -->
</section>

<!-- Use meaningful class names -->
<div class="project-card"> <!-- Good -->
<div class="pc"> <!-- Bad -->
```

### CSS
```css
/* Use Tailwind utility classes when possible */
<div class="flex gap-4 md:gap-8 p-4 md:p-6">

/* Use meaningful variable names */
.project-btn-primary { /* Good */
.pb { /* Bad */

/* Add comments for complex rules */
/* Mobile touch target accessibility */
.btn { min-height: 48px; }
```

### JavaScript
```javascript
// Use descriptive function names
function initMobileMenu() { /* Good */ }
function im() { /* Bad */ }

// Add comments for non-obvious logic
// Fade in project cards on scroll
animateProjectCards();

// Use const/let, not var
const portfolio = document.querySelector('#portfolio');
```

---

## 📝 Commit Message Best Practices

**Format:** `type: brief description`

```bash
# Good commit messages
git commit -m "fix: resolve mobile button click issue"
git commit -m "docs: improve SETUP.md clarity"
git commit -m "feature: add resume download button"
git commit -m "style: improve spacing on hero section"

# Bad commit messages
git commit -m "Update"
git commit -m "Fixed bug"
git commit -m "WIP"
```

**Types:**
- `feat:` New feature
- `fix:` Bug fix
- `docs:` Documentation
- `style:` Formatting/styling
- `refactor:` Code restructuring
- `perf:` Performance improvement
- `test:` Adding tests

---

## ✅ Checklist Before Submitting PR

- [ ] Tested on desktop
- [ ] Tested on mobile
- [ ] No console errors
- [ ] No broken links
- [ ] Documentation updated
- [ ] Follows code style
- [ ] Commit messages are clear
- [ ] No unnecessary files added

---

## 🙋 Questions?

- **Questions about setup?** → Check [SETUP.md](SETUP.md)
- **Need customization help?** → See [CUSTOMIZATION_CHECKLIST.md](CUSTOMIZATION_CHECKLIST.md)
- **Have an issue?** → Open a GitHub Issue
- **Want to discuss?** → Start a GitHub Discussion

---

## 🎉 Thank You!

Contributors make this project better for everyone. Your time and effort are greatly appreciated!

### Recognition

All contributors are recognized in the [Contributors](#contributors) section of README.md.

---

## License

By contributing, you agree that your contributions will be licensed under the [MIT License](LICENSE.md).

---

Happy coding! 🚀
