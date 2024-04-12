---
marp: true
author: Joan G.
theme: default
class: invert
backgroundImage: "linear-gradient(to right, #0f2027, #203a43, #2c5364)"

---

# Building slides as code with Marp

![bg opacity:.7](img/pexels-daniel-putzer-633409.jpg)

---

# Use Cases for Marp

- Repeatable way to build slides
- Integrate slide with some repository
- Sharing ``code examples`` with in a nice way

---

# How to change Theme

Nice and dark 🌔

```markdown
---
marp: true
theme: default
class: invert
```

---

# To get Free Pictures

![bg right](img/pexels-andrea-piacquadio-3758104.jpg)

Use:
- [Pexels](https://www.pexels.com)
- [Unsplash](https://unsplash.com)

How to work with images:
- [image syntax](https://marpit.marp.app/image-syntax)

Say thanks! - add a reference to the author or collection.

---

![bg blur:2px](img/pexels-andrea-piacquadio-3758104.jpg)
![bg opacity:.7](img/pexels-andrea-piacquadio-3758104.jpg)
![bg sepia](img/pexels-andrea-piacquadio-3758104.jpg)

---

# More Marp Themes

- [Dracula](https://draculatheme.com/marp)
- [Beam](https://rnd195.github.io/marp-community-themes/theme/beam.html)
- [Marpstyle](https://github.com/cunhapaulo/marpstyle)

---

# Using Community Themes

- Add CSS from some community repos
- Add VScode settings

````json
{
    "markdownlint.config": {
        "default":true,
        // allow multiple H1s for Marp
        "MD025":false,
        "MD032": false
    },
    "markdown.marp.themes": [
        "./themes/dracula.css"
    ]
}
````

- Update theme: e.g. `theme: dracula`
- Update the workflow

---

# Using Gradient Background

```yaml
backgroundImage: "linear-gradient(to right, #0f2027, #203a43, #2c5364)"
```

Where to find gradients and colors:

- [Uigradients](https://uigradients.com)
- [HappyHues](https://happyhues.co)

---

# How to Use Animated Images

- This looks amazing on a starting page

```markdown
![bg right fit](https://github.com/srl-labs/containerlab/raw/main/docs/images/containerlab_export_white_ink.svg?sanitize=true)
```

![bg right fit](https://github.com/srl-labs/containerlab/raw/main/docs/images/containerlab_export_white_ink.svg?sanitize=true)

---

# Using Lists

```markdown
- item1
- item2
```

- item1
- item2

---

# Animated Lists

- Some item
  - sub item

* This will be hidden at first

```markdown
- Some item
  - sub item

* This will be hidden at first
```
