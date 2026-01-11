# Contributing to IRCC XFA Form Extractor

First off, thank you for considering contributing to IRCC XFA Form Extractor! 🎉

## Ways to Contribute

- 🐛 Report bugs
- 💡 Suggest new features
- 📝 Improve documentation
- 🔧 Submit pull requests

## Development Setup

1. **Fork and clone the repository**

```bash
git clone https://github.com/adelrzouga/ircc-xfa-extractor.git
cd ircc-xfa-extractor
```

2. **Create a virtual environment**

```bash
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install in development mode**

```bash
pip install -e ".[dev]"
```

4. **Create a new branch**

```bash
git checkout -b feature/your-feature-name
```

## Code Style

- Follow PEP 8 guidelines
- Use meaningful variable and function names
- Add docstrings to functions and classes
- Keep functions focused and modular

**Format code with Black:**

```bash
black ircc_xfa/
```

## Testing

Before submitting a pull request:

1. **Test with sample PDFs**

```bash
# Test basic extraction
ircc sample.pdf -v

# Test multiple files
ircc *.pdf --combined
```

2. **Verify installation**

```bash
pip install -e .
ircc --version
```

3. **Check for errors**

```bash
# Run with various PDF types
ircc valid_form.pdf
ircc empty_form.pdf
ircc non_xfa_form.pdf
```

## Submitting Changes

1. **Commit your changes**

```bash
git add .
git commit -m "Brief description of changes"
```

Use clear commit messages:
- ✨ `feat: Add support for IMM5645 forms`
- 🐛 `fix: Handle empty XFA datasets`
- 📝 `docs: Update installation instructions`
- 🔧 `refactor: Simplify field extraction logic`

2. **Push to your fork**

```bash
git push origin feature/your-feature-name
```

3. **Create a Pull Request**

- Go to the original repository on GitHub
- Click "New Pull Request"
- Select your branch
- Describe your changes clearly

## Pull Request Guidelines

### Good PR Description

```markdown
## Description
Adds support for extracting data from IMM5645 family information forms.

## Changes
- Added IMM5645 form template detection
- Updated extraction logic to handle new field types
- Added example output for IMM5645

## Testing
- Tested with 5 different IMM5645 PDFs
- Verified output format
- Checked edge cases (empty forms, partial completion)

## Checklist
- [x] Code follows project style
- [x] Documentation updated
- [x] Tested manually
- [x] No breaking changes
```

## Bug Reports

When reporting bugs, please include:

1. **Environment**
   - OS (macOS, Linux, Windows)
   - Python version
   - Package version (`ircc --version`)

2. **Steps to reproduce**
   ```bash
   ircc problematic_form.pdf -v
   ```

3. **Expected behavior**

4. **Actual behavior**

5. **Error messages** (if any)

6. **Sample PDF** (if possible, or describe the form type)

## Feature Requests

For feature requests, please describe:

1. **Use case**: What problem does this solve?
2. **Proposed solution**: How should it work?
3. **Alternatives**: What other approaches did you consider?
4. **Examples**: Show how you'd use this feature

## Code of Conduct

### Our Standards

- Be respectful and inclusive
- Welcome newcomers
- Focus on constructive feedback
- Assume good intentions

### Unacceptable Behavior

- Harassment or discrimination
- Trolling or insulting comments
- Personal attacks
- Publishing others' private information

## Questions?

- Open an issue for questions about contributing
- Check existing issues and PRs first
- Be patient - this is maintained by volunteers

## Recognition

Contributors will be recognized in:
- GitHub contributors page
- Release notes for significant contributions
- README acknowledgments section (coming soon)

---

Thank you for contributing! 🙏
