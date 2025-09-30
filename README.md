# AWS Budgets Workshop

A comprehensive hands-on workshop for learning AWS cost management using AWS Budgets service.

## 🎯 Overview

This workshop teaches you how to effectively manage and monitor AWS costs using **AWS Budgets**. You'll learn to create different types of budgets, set up alerts, and implement cost control strategies for your AWS environment.

## 📚 What You'll Learn

- Understanding AWS Budgets service and its capabilities
- Creating and configuring different budget types
- Setting up cost alerts and notifications
- Implementing automated budget actions
- Best practices for cost management

## 🏗️ Workshop Structure

### Prerequisites
- AWS Account with billing access
- Basic understanding of AWS services
- IAM permissions for AWS Budgets and CloudWatch

### Workshop Modules

1. **[Create Template](content/0-Createtemplate/)** - Initial setup and preparation
2. **[Cost Budgets](content/1-Cost-Budgets/)** - Track AWS spending with cost-based budgets
3. **[Usage Budget](content/2-Usage-Budget/)** - Monitor service usage with usage-based budgets
4. **[Reservation Budget](content/3-Reservation-Budget/)** - Track Reserved Instance utilization
5. **[Savings Plans Budget](content/4-Saving-Plans-Budget/)** - Monitor Savings Plans coverage
6. **[Clean Up](content/5-clean-up/)** - Remove workshop resources

## 🚀 Getting Started

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/AWS-First-Cloud-Journey/000007-AWSBudget.git
   cd 000007-AWSBudget
   ```

2. **Install Hugo** (if not already installed)
   ```bash
   # macOS
   brew install hugo
   
   # Ubuntu/Debian
   sudo apt-get install hugo
   
   # Windows
   choco install hugo
   ```

3. **Run the development server**
   ```bash
   hugo server -D
   ```

4. **Access the workshop**
   Open your browser to `http://localhost:1313`

### Build for Production

```bash
hugo --minify
```

The generated site will be in the `public/` directory.

## 🌐 Languages

This workshop is available in multiple languages:

- **English** (`/en/`) - Primary language
- **Vietnamese** (`/vi/`) - Tiếng Việt

## 📋 Budget Types Covered

### 1. Cost Budget
- Track AWS spending against monetary thresholds
- Set up alerts for actual and forecasted costs
- Configure multiple alert levels (50%, 80%, 90%, 100%)

### 2. Usage Budget
- Monitor specific service usage (EC2 hours, data transfer, etc.)
- Set usage-based thresholds and alerts
- Track resource consumption patterns

### 3. Reservation Budget
- Monitor Reserved Instance utilization and coverage
- Track RI efficiency and cost savings
- Optimize reservation strategies

### 4. Savings Plans Budget
- Monitor Savings Plans utilization and coverage
- Track commitment efficiency
- Optimize savings strategies

## 🔧 Technical Stack

- **Static Site Generator**: Hugo
- **Theme**: Hugo Learn Theme
- **Languages**: Markdown, HTML, CSS, JavaScript
- **Deployment**: GitHub Pages compatible

## 📁 Project Structure

```
000007-AWSBudget/
├── content/                 # Workshop content
│   ├── 0-Createtemplate/   # Setup module
│   ├── 1-Cost-Budgets/     # Cost budget module
│   ├── 2-Usage-Budget/     # Usage budget module
│   ├── 3-Reservation-Budget/ # RI budget module
│   ├── 4-Saving-Plans-Budget/ # Savings Plans module
│   └── 5-clean-up/         # Cleanup module
├── static/                 # Static assets
│   ├── images/            # Workshop images
│   └── css/               # Custom styles
├── layouts/               # Hugo layout templates
├── themes/                # Hugo theme
├── public/                # Generated site (build output)
├── config.toml           # Hugo configuration
└── README.md             # This file
```

## 🎨 Customization

### Theme Configuration
The workshop uses the Hugo Learn theme with custom styling:
- Theme variant: `workshop`
- Custom CSS: `static/css/theme-workshop.css`
- Custom logo: `layouts/partials/logo.html`

### Adding Content
1. Create new markdown files in the appropriate `content/` directory
2. Follow the existing frontmatter structure
3. Use Hugo shortcodes for enhanced formatting

## 🔒 Security Best Practices

- Use IAM roles with least privilege principles
- Enable MFA for accounts with budget management permissions
- Regularly review and audit budget configurations
- Implement proper access controls for billing information

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Content Guidelines
- Follow the existing content structure
- Include both English and Vietnamese translations
- Add relevant screenshots and examples
- Test all procedures before submitting

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/AWS-First-Cloud-Journey/000007-AWSBudget/issues)
- **Discussions**: [GitHub Discussions](https://github.com/AWS-First-Cloud-Journey/000007-AWSBudget/discussions)
- **AWS Study Group**: [Facebook Group](https://www.facebook.com/groups/awsstudygroupfcj)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🏷️ Tags

`aws` `budgets` `cost-management` `workshop` `hugo` `cloud` `finops` `cost-optimization`

---

**AWS First Cloud Journey** - Empowering cloud learning through hands-on workshops.
