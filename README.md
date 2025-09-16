# Claude Memory System Documentation

This repository contains the documentation for [claude-mem](https://github.com/thedotmack/claude-mem), built with [Mintlify](https://mintlify.com).

## 🚀 Development

### Prerequisites

- Node.js 18+
- Mintlify CLI (`npm i -g mint`)

### Local Development

```bash
# Install Mintlify CLI
npm i -g mint

# Start dev server
mint dev

# Or on a custom port
mint dev --port 3333
```

The documentation will be available at http://localhost:3000 (or your custom port).

## 📁 Structure

```
claude-mem-docs/
├── mint.json          # Mintlify configuration
├── introduction.mdx   # Landing page
├── quickstart.mdx     # Quick start guide
├── installation.mdx   # Installation guide
├── concepts/          # Core concepts
├── configuration/     # Configuration guides
├── cli/              # CLI reference
├── api-reference/    # API documentation
├── guides/           # Tutorials and guides
└── advanced/         # Advanced topics
```

## 🎨 Customization

Edit `mint.json` to:
- Update navigation structure
- Change colors and branding
- Configure analytics
- Add social links

## 📝 Writing Documentation

Mintlify uses MDX format with special components:

- `<Card>` - Feature cards
- `<CardGrid>` - Card layouts
- `<Tabs>` - Tabbed content
- `<Steps>` - Step-by-step guides
- `<AccordionGroup>` - Collapsible sections
- `<Note>`, `<Warning>`, `<Tip>` - Callouts

## 🚢 Deployment

The documentation can be deployed to:
- Mintlify hosting (recommended)
- GitHub Pages
- Netlify/Vercel
- Custom domain

### Deploy to Mintlify

```bash
mint deploy
```

## 📄 License

Documentation is licensed under MIT License.

## 🤝 Contributing

Contributions are welcome! Please:
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 🔗 Links

- [claude-mem Repository](https://github.com/thedotmack/claude-mem)
- [NPM Package](https://www.npmjs.com/package/claude-mem)
- [Live Documentation](https://docs.claude-mem.com) (coming soon)