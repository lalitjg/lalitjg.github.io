---
layout: default
title: "Example Blog Post"
date: 2025-11-24
excerpt: "This is a sample blog post showing the structure for future posts."
---

# {{ page.title }}

*Published on {{ page.date | date: "%B %-d, %Y" }}*

This is a sample blog post. When you create new blog posts, follow this structure:

## File Naming Convention

Files in `_posts/` must follow the format: `YYYY-MM-DD-title-of-post.md`

For example:
- `2025-11-24-my-first-post.md`
- `2025-12-01-learning-about-transformers.md`

## Front Matter

Each post needs YAML front matter at the top:

```yaml
---
layout: default
title: "Your Post Title"
date: YYYY-MM-DD
excerpt: "A short description that appears on the blog listing page."
---
```

## Writing Your Post

After the front matter, write your content in Markdown. You can use:

- **Bold** and *italic* text
- Lists (like this one)
- Code blocks
- Headers
- Links and images
- Math equations (using KaTeX)

### Code Example

```python
def hello_world():
    print("Hello from my blog!")
```

### Math Example

Inline math: $E = mc^2$

Block math:

$$
\frac{\partial u}{\partial t} = \alpha \nabla^2 u
$$

## That's It!

Just create a new `.md` file in the `_posts/` folder with the proper date format, and it will automatically appear on your blog page.

You can delete this example post once you're ready to write your own!
