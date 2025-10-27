# Reccaller Contexts Store

Official context repository for [Reccaller AI](https://reccaller.ai) - version-controlled context configurations for better AI-assisted development.

## 🌐 Access

Base URL: **https://contexts.reccaller.ai**

## 📚 Available Contexts

Browse all available contexts:
```bash
curl https://contexts.reccaller.ai/index.json
```

### Current Contexts

- **Default** - Base context configuration
  - `https://contexts.reccaller.ai/contexts/default.json`

- **TypeScript React** - For React/TypeScript projects
  - `https://contexts.reccaller.ai/contexts/typescript-react.json`

- **Python** - For Python development
  - `https://contexts.reccaller.ai/contexts/python.json`

## 🚀 Usage

### Via CLI (coming soon)
```bash
# List available contexts
reccaller contexts list

# Download a specific context
reccaller contexts get typescript-react
```

### Direct Download
```bash
# Get a specific context
curl https://contexts.reccaller.ai/contexts/typescript-react.json

# Get the index
curl https://contexts.reccaller.ai/index.json
```

## 📦 Structure
```
contexts/
├── default.json          # Base context
├── typescript-react.json # TypeScript React context
├── python.json          # Python context
└── ...                  # More contexts

starter-pack/            # Coming soon
└── ...                  # Starter pack files

index.json              # Context directory
CNAME                   # GitHub Pages domain
```

## 🎯 Context Format

Each context is a JSON file with the following structure:
```json
{
  "version": "1.0.0",
  "id": "unique-id",
  "name": "Human Readable Name",
  "description": "What this context is for",
  "updated": "2025-10-27",
  "patterns": ["*.ts", "*.tsx"],
  "rules": [
    "Rule 1",
    "Rule 2"
  ],
  "preferences": {
    "key": "value"
  }
}
```

## 🤝 Contributing

Want to add your own context? 

1. Fork this repo
2. Add your context JSON file to `contexts/`
3. Update `index.json`
4. Submit a pull request

## 📝 Version Control

All contexts are version controlled via Git. Each update creates a commit for tracking changes.

## 🔗 Links

- **Main Site**: https://reccaller.ai
- **Main Repository**: https://github.com/reccaller-ai/reccall
- **Issues**: https://github.com/reccaller-ai/contexts/issues

## 📄 License

MIT License - see main repository for details.
