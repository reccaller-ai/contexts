# Reccaller Contexts Store

Official context repository for [Reccaller AI](https://reccaller.ai) - version-controlled context configurations and recipes for better AI-assisted development.

## 🌐 Access

Base URL: **https://contexts.reccaller.ai**

## 📚 Repository Structure

This repository now supports both **contexts** (for AI-assisted development environments) and **recipes** (for RecCall shortcuts and automation).

### Structure
```
contexts/
├── manifest.json       # Recipe manifest with shortcuts and metadata
├── contexts/           # Context configurations
│   ├── default.json
│   ├── python.json
│   └── typescript-react.json
├── git/               # Git-related recipes
│   ├── sync-main.json
│   ├── create-feature-branch.json
│   └── cleanup-branches.json
├── development/       # Development recipes
├── deployment/        # Deployment recipes
├── debugging/         # Debugging recipes
├── code-review/       # Code review recipes
├── testing/          # Testing recipes
├── database/         # Database recipes
├── security/         # Security recipes
├── devops/           # DevOps recipes
├── frontend/         # Frontend recipes
├── backend/          # Backend recipes
├── project-management/ # Project management recipes
└── additional/       # Additional utilities
```

## 🚀 Usage

### RecCall Recipes

Browse available recipes via the manifest:
```bash
curl https://contexts.reccaller.ai/manifest.json
```

### Contexts

Browse all available contexts:
```bash
curl https://contexts.reccaller.ai/index.json
```

### Direct Download
```bash
# Get a specific context
curl https://contexts.reccaller.ai/contexts/typescript-react.json

# Get a specific recipe
curl https://contexts.reccaller.ai/git/sync-main.json

# Get the manifest
curl https://contexts.reccaller.ai/manifest.json
```

## 🎯 Recipe Format

Each recipe is a JSON file with the following structure:
```json
{
  "shortcut": "sync-main",
  "context": "Switch to main branch and pull latest changes...",
  "category": "git",
  "description": "Sync main branch with latest remote changes"
}
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
