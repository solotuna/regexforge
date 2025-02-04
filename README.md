# Regex Forge Community Patterns

This repository contains a collection of community-contributed regex patterns for [Regex Forge](https://apps.apple.com/us/app/regex-forge/id6737852994), a macOS regex editor designed to make working with regular expressions easier.

## Structure 

Each regex pattern is stored as a YAML file inside the patterns/ folder and follows this structure:

```yaml
version: 1
name: Email
description: This pattern matches common email formats.
pattern: >
  ^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$
text: |
  Valid emails:
  test@example.com
  user.name+tag@domain.co.uk

  Invalid emails:
  invalid-email
  user@domain
author: john_doe
```

## Using the Patterns

Regex Forge automatically loads and displays these patterns inside the app, allowing users to explore, test, and use them in their projects.

## Contributing

Want to add a new pattern? Follow these steps:

- Create a new YAML file inside the patterns/ directory.
- Use the format shown above, ensuring your pattern includes:
  - version: Format version (always 1 for now).
  - name: A short, descriptive name for your pattern.
  - description: A brief explanation of what the pattern does.
  - pattern: The regular expression itself.
  - text: Example input data showcasing valid and invalid matches.
  - author: Your name or GitHub handle (optional).
- Submit a pull request, and after review, your pattern will be added!

## Licence

This repository is open-source and follows the MIT License.

