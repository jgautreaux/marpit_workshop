---
marp: true
author: Joan G.
theme: default
class: invert
backgroundImage: "linear-gradient(to right, #0f2027, #203a43, #2c5364)"
paginate: true
style: |
    footer {
        font-size: 20px
    }
    section::after {
        font-size: 20px
    }
    pre {
        background: linear-gradient(to top, #0f2027, #203a43, #2c5364)
    }
    .columns {
        display: grid;
        grid-template-columns: repeat(2, minmax(0, 1fr));
        gap: 1rem
    }
    .columns3 {
        display: grid;
        grid-template-columns: repeat(3, minmax(0, 1fr));
        gap: 1rem
    }

---

# Building slides as code with Marp

<!--- Do not add page number on this slide --->
<!---
_paginate: false
-->

````json
{
    "date": "12.04.2024",
    "topic": "random things about marp",
    "author": "Joan Gautreaux"
}
````

![bg right](img/pexels-daniel-putzer-633409.jpg)

---

<!--- Add footer starting from this slide --->
<!---
footer: "April 2024"
-->

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

---

# Paginate

```markdown
paginate: true
```

---

# Footer

```markdown
<!--- 
_footer: '![h:24](https://upload.wikimedia.org/wikipedia/commons/thumb/9/99/Arista-networks-logo.svg/220px-Arista-networks-logo.svg.png)'
--->
```

<!--- 
_footer: '![h:24](https://upload.wikimedia.org/wikipedia/commons/thumb/9/99/Arista-networks-logo.svg/220px-Arista-networks-logo.svg.png)'
--->

---

# 2 Columns format

<div class="columns">
<div>

- test
- test

</div>


<div>

```json
{
    "a": 1,
    "b": 2
}
```

</div>

</div>


---

# 3 Columns format

<div class="columns3">
<div>

- test
- test

</div>

<div>

Some text here

</div>


<div>

JSON Snippet

```json
{
    "c": 3,
    "d": 4
}
```

</div>

</div>

---

# Font Size

<style scoped>section {font-size: 14px} </style>

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque egestas velit at elit dapibus, non commodo mauris luctus. Etiam non blandit nisi. Donec vel massa vel turpis dignissim vehicula vitae eget turpis. Duis semper iaculis libero eget maximus. Duis iaculis eu nisl tincidunt ornare. Duis finibus sem sed neque vulputate, congue blandit arcu gravida. Quisque quis urna eu magna blandit tincidunt. Donec nec blandit massa. Ut et libero porttitor, condimentum massa sit amet, vulputate orci. Praesent vitae nulla velit. Donec consequat mi ligula, non condimentum tellus elementum id.

Vestibulum finibus eleifend odio, ac tristique massa interdum quis. Etiam viverra pretium erat, ac tincidunt nulla interdum sed. Pellentesque ultrices tristique ex at hendrerit. Vestibulum gravida porttitor tellus. Pellentesque lacus nunc, bibendum sed sollicitudin sed, cursus eget massa. Fusce ac mattis diam, sed lobortis lacus. Sed ac lacus a tellus facilisis egestas. Suspendisse sodales finibus eros ut sodales. Cras vehicula maximus imperdiet. Nullam tempor commodo egestas. Maecenas bibendum tincidunt aliquam. Ut fermentum libero nec dui tincidunt consequat.

Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Integer posuere mi tortor, faucibus iaculis libero pellentesque id. Ut nec lectus in sapien sagittis congue. Praesent tortor sem, ultrices vel sodales eu, lobortis nec enim. Fusce a nisi lorem. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Vivamus porttitor, odio at dapibus pharetra, quam nulla bibendum mauris, non varius lorem erat eu sem. Ut sit amet elit in massa gravida viverra. Nullam tempus eleifend neque, sed placerat erat tempor quis. Phasellus id efficitur neque. Morbi congue porttitor tortor placerat placerat. Vestibulum turpis massa, vehicula eu tempus vestibulum, efficitur eget nisl. Nam rutrum volutpat metus in bibendum. Aenean vehicula odio at feugiat eleifend. Sed in urna vestibulum mauris blandit malesuada vitae sed arcu. Nulla elementum mauris vitae mi tristique, ac varius ipsum pulvinar.

Quisque fermentum lorem nec sapien consequat, quis condimentum quam dapibus. Vivamus non interdum ante. Sed vestibulum vulputate dictum. Sed dictum vestibulum finibus. Praesent tincidunt euismod nulla, eget ullamcorper dolor consectetur id. Aenean non lorem mauris. Morbi lobortis mattis gravida. Pellentesque facilisis porttitor ultricies. Morbi iaculis varius lectus, eget aliquam elit iaculis vulputate. Nullam blandit tincidunt semper.

Vivamus vitae placerat felis. Nullam faucibus est imperdiet risus eleifend venenatis. Nunc cursus sem ac justo sollicitudin venenatis sit amet eu diam. Aliquam eget lorem ac metus auctor tempus et nec justo. Donec ullamcorper elit eget laoreet aliquet. Duis lacinia molestie nulla, ac venenatis ipsum tristique vitae. In at porta felis. Mauris tincidunt, justo nec malesuada volutpat, nisl enim sagittis enim, vel dignissim erat sem quis arcu.