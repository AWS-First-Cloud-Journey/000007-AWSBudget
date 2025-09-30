# Contributing to AWS Budgets Workshop

Thank you for your interest in contributing to the AWS Budgets Workshop! This document provides guidelines and information for contributors.

## 🤝 How to Contribute

### Reporting Issues

Before creating an issue, please:
1. Check existing issues to avoid duplicates
2. Use the appropriate issue template
3. Provide clear, detailed information
4. Include screenshots when relevant

### Suggesting Enhancements

We welcome suggestions for improvements:
- New workshop modules or exercises
- Better explanations or examples
- Additional language translations
- UI/UX improvements

### Contributing Code

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Make your changes**
4. **Test thoroughly**
5. **Commit with clear messages**
   ```bash
   git commit -m "Add: Clear description of changes"
   ```
6. **Push to your fork**
7. **Create a Pull Request**

## 📝 Content Guidelines

### Writing Style
- Use clear, concise language
- Write for beginners to intermediate users
- Include practical examples
- Maintain consistent terminology

### Structure
- Follow the existing content structure
- Use proper markdown formatting
- Include appropriate frontmatter
- Add navigation elements

### Screenshots
- Use high-resolution images (1920x1080 minimum)
- Highlight relevant UI elements
- Keep images current with AWS console updates
- Optimize file sizes

### Code Examples
- Test all code before submitting
- Include error handling where appropriate
- Add comments for complex sections
- Follow AWS best practices

## 🌐 Translation Guidelines

### Adding New Languages
1. Create language-specific content directories
2. Update `config.toml` with new language settings
3. Translate all content files
4. Test the site with the new language

### Translation Standards
- Maintain technical accuracy
- Preserve formatting and structure
- Keep code examples in English
- Translate UI elements and descriptions

## 🔧 Technical Requirements

### Development Environment
- Hugo (latest version)
- Git
- Text editor with markdown support
- Web browser for testing

### Testing
Before submitting:
- Test locally with `hugo server`
- Verify all links work
- Check responsive design
- Validate HTML output

### Build Process
```bash
# Install dependencies
hugo mod get

# Run development server
hugo server -D

# Build for production
hugo --minify
```

## 📋 Pull Request Process

### Before Submitting
- [ ] Code follows project conventions
- [ ] All tests pass locally
- [ ] Documentation is updated
- [ ] Screenshots are current
- [ ] Translations are complete (if applicable)

### PR Description Template
```markdown
## Description
Brief description of changes

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Documentation update
- [ ] Translation update

## Testing
- [ ] Tested locally
- [ ] All links verified
- [ ] Screenshots updated
- [ ] Cross-browser tested

## Screenshots
Include before/after screenshots if UI changes
```

### Review Process
1. Automated checks must pass
2. At least one maintainer review required
3. Address feedback promptly
4. Maintain clean commit history

## 🎯 Priority Areas

We especially welcome contributions in:
- **Screenshots**: Keeping AWS console images current
- **Translations**: Adding new languages or improving existing ones
- **Examples**: Real-world scenarios and use cases
- **Testing**: Improving test coverage and automation

## 📞 Getting Help

### Communication Channels
- **GitHub Issues**: Bug reports and feature requests
- **GitHub Discussions**: General questions and ideas
- **Facebook Group**: [AWS Study Group](https://www.facebook.com/groups/awsstudygroupfcj)

### Maintainer Contact
- Create an issue for technical questions
- Use discussions for general inquiries
- Tag maintainers in urgent matters

## 🏆 Recognition

Contributors will be recognized:
- Listed in repository contributors
- Mentioned in release notes
- Featured in community highlights
- Added to acknowledgments section

## 📜 Code of Conduct

### Our Standards
- Be respectful and inclusive
- Focus on constructive feedback
- Help others learn and grow
- Maintain professional communication

### Unacceptable Behavior
- Harassment or discrimination
- Spam or off-topic content
- Sharing sensitive information
- Disruptive behavior

### Enforcement
Violations may result in:
1. Warning
2. Temporary suspension
3. Permanent ban

Report issues to maintainers via private message.

## 📚 Resources

### AWS Documentation
- [AWS Budgets User Guide](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/budgets-managing-costs.html)
- [AWS Cost Management](https://aws.amazon.com/aws-cost-management/)

### Hugo Documentation
- [Hugo Quick Start](https://gohugo.io/getting-started/quick-start/)
- [Hugo Learn Theme](https://learn.netlify.app/en/)

### Markdown Resources
- [Markdown Guide](https://www.markdownguide.org/)
- [GitHub Flavored Markdown](https://github.github.com/gfm/)

## 🚀 Getting Started

1. **Read the README** - Understand the project structure
2. **Set up locally** - Follow installation instructions
3. **Pick an issue** - Start with "good first issue" labels
4. **Ask questions** - Don't hesitate to seek help
5. **Start small** - Begin with minor improvements

Thank you for contributing to the AWS Budgets Workshop! Your efforts help the community learn AWS cost management effectively.
