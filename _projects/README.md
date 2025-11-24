# Project Template Guide

When creating a new project, create a file in `_projects/` folder with the name `your-project-name.md`

## Minimal Template

```markdown
---
layout: default
title: "Your Project Title"
description: "One-line description of your project"
github: "https://github.com/username/repo"
paper: "https://arxiv.org/abs/xxxx.xxxxx"
blog: "/blog/YYYY/MM/DD/post-title"
---

# {{ page.title }}

## Overview

Write your project description here.

## Key Features

- Feature 1
- Feature 2
- Feature 3

## Technical Details

Add technical details, code snippets, architecture diagrams, etc.

### Architecture

Describe your model/system architecture here.

### Implementation

```python
# Sample code snippet
def example_function():
    return "This is a placeholder"
```

## Results

Present your results, metrics, or visualizations.

## Front Matter Fields

- **title** (required): The project name
- **description** (required): Short description shown on projects list page
- **github** (optional): Link to GitHub repository
- **paper** (optional): Link to paper (arxiv, conference, journal)
- **blog** (optional): Relative link to your blog post about this project

## Notes

- Links are optional - only include the ones that exist
- The blog link should be relative (e.g., `/blog/2025/11/24/post-title`)
- GitHub and paper links should be full URLs
- Projects will appear on the main projects page automatically

```
## Links

{% if page.github %}
- **GitHub Repository:** [{{ page.github }}]({{ page.github }})
{% endif %}

{% if page.paper %}
- **Paper:** [Read the paper]({{ page.paper }})
{% endif %}

{% if page.blog %}
- **Blog Post:** [Read more about this project]({{ page.blog | relative_url }})
{% endif %}

## Citation

If you use this work, please cite:

```bibtex
@article{yourname2025,
  title={Your Paper Title},
  author={Your Name},
  journal={Conference/Journal},
  year={2025}
}
```

---

*Last updated: {{ page.date | default: "2025-11-24" | date: "%B %Y" }}*


