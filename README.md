# AI Project Context — `ai-context.yaml`

**A simple, human-readable file to give AI tools the right context for your project.**  
This repository shows an example `ai-context.yaml` for the _Awesome Web App_ project, but the idea works for **any** codebase.

---

## Why?

When developers use AI to write or review code, the AI often lacks important project knowledge:  
- coding style guides  
- terminology  
- architectural constraints  
- key files and their purpose  
- example inputs/outputs  

Instead of repeating all of that in every prompt, keep it **in one place**: `ai-context.yaml`.

---

## What is `ai-context.yaml`?

It’s a YAML file stored at your project’s root that contains:

- **Project info** – name, description, license, style guide
- **Profiles** – role-specific instructions for AI (e.g., code review, documentation)
- **Glossary** – project-specific terms with definitions
- **File references** – important files or directories
- **Examples** – sample inputs and expected outputs

---

## How to Use It

1. **Add it to your repo**  
   Copy `ai-context.yaml` to your project root and update the details.

2. **Choose a profile**  
   - General tasks → `default`
   - Code review → `code_review`
   - Documentation → `documentation`

3. **Tell the AI** to load and follow it  
   If your AI tool supports file reading, point it to `ai-context.yaml`.  
   If not, paste its contents or link to it and mention which profile to use.

**Example prompt**:
