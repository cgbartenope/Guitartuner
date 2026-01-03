# Contributing to Guitar Tuner Directory

First off, thank you for considering contributing to Guitar Tuner Directory! It's people like you that make this project better for everyone.

## Code of Conduct

By participating in this project, you are expected to uphold our Code of Conduct:
- Be respectful and inclusive
- Welcome newcomers
- Focus on what's best for the community
- Show empathy towards others

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check existing issues to avoid duplicates. When creating a bug report, include:

- **Clear title and description**
- **Steps to reproduce** the behavior
- **Expected behavior** vs actual behavior
- **Screenshots** if applicable
- **Browser and OS** information

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion, include:

- **Clear title and description**
- **Detailed explanation** of the proposed feature
- **Why this enhancement would be useful** to most users
- **Possible implementation** ideas (optional)

### Adding New Content

#### Adding New Online Tuners

1. Verify the tuner is free and works properly
2. Add a new card in the "Online Guitar Tuners" section
3. Include:
   - Accurate description
   - Key features (4-5 bullet points)
   - Working link with `target="_blank"` and `rel="noopener"`
   - Appropriate badge (free/premium)

#### Adding New Product Listings

1. Verify product information and pricing
2. Add to the "Tuners for Sale" section
3. Include:
   - Product name and manufacturer
   - Accurate description
   - Technical specifications
   - Current approximate price
   - Badge indicating category (budget/premium/best seller)

#### Adding New Educational Resources

1. Verify the resource is high-quality and free (or clearly marked if paid)
2. Add to the "Learning Resources" section
3. Include:
   - Resource title and source
   - Skill level indicator
   - Brief description
   - Key topics covered
   - Working link

### Pull Request Process

1. **Fork the repository** and create your branch from `main`
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. **Make your changes**
   - Follow the existing code style
   - Keep changes focused and atomic
   - Test on multiple browsers if making CSS/JS changes

3. **Test your changes**
   - Open `index.html` in multiple browsers
   - Check responsive design on mobile/tablet
   - Verify all links work
   - Check for console errors

4. **Commit your changes**
   ```bash
   git commit -m "Add: description of your changes"
   ```
   Use conventional commit messages:
   - `Add:` for new features
   - `Fix:` for bug fixes
   - `Update:` for updates to existing features
   - `Remove:` for removing features
   - `Docs:` for documentation changes

5. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```

6. **Submit a Pull Request**
   - Provide a clear title and description
   - Reference any related issues
   - Include screenshots for visual changes

### Code Style Guidelines

#### HTML
- Use semantic HTML5 elements
- Maintain proper indentation (2 spaces)
- Include alt text for images
- Use meaningful class names

#### CSS
- Follow existing naming conventions
- Use CSS custom properties for colors
- Keep selectors specific but not overly complex
- Comment major sections
- Mobile-first approach for media queries

#### JavaScript
- Use modern ES6+ syntax
- Keep functions small and focused
- Add comments for complex logic
- Avoid inline event handlers

### Content Guidelines

- **Accuracy**: All information must be accurate and up-to-date
- **Quality**: Only include high-quality resources
- **Neutrality**: Avoid promotional language
- **Attribution**: Properly attribute sources
- **Links**: All external links must be verified working

### Adding SEO Improvements

If suggesting SEO improvements:
- Provide data or reasoning
- Don't sacrifice user experience for SEO
- Follow current best practices
- Test changes if possible

## Development Setup

1. Clone your fork
   ```bash
   git clone https://github.com/YOUR-USERNAME/guitar-tuner-directory.git
   ```

2. Navigate to the directory
   ```bash
   cd guitar-tuner-directory
   ```

3. Open in your preferred editor
   ```bash
   code .  # VS Code
   # or your preferred editor
   ```

4. Open `index.html` in a browser
   - Use live server if available
   - Or simply open the file directly

## Testing Checklist

Before submitting a PR, ensure:

- [ ] Tested in Chrome/Edge
- [ ] Tested in Firefox
- [ ] Tested in Safari (if possible)
- [ ] Tested on mobile viewport
- [ ] Tested on tablet viewport
- [ ] All links work correctly
- [ ] No console errors
- [ ] Smooth animations/transitions
- [ ] Proper contrast/accessibility
- [ ] Valid HTML (W3C validator)
- [ ] Valid CSS

## Questions?

Feel free to:
- Open an issue with the `question` label
- Reach out to maintainers
- Check existing issues/PRs for similar questions

## Recognition

Contributors will be recognized in:
- GitHub contributors page
- README.md acknowledgments section

Thank you for contributing! 🎸
