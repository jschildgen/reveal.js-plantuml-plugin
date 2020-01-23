# reveal.js-plantuml-plugin

[PlantUML](https://plantuml.com/) transforms texts into UML diagrams (class, sequence, ...), ER diagrams, etc. This plugin adds an easy-to-use PlantUML support to the HTML presentation framework [reveal.js](https://github.com/hakimel/reveal.js)

## Setup

1. Add the file `lib/deflate.js` to the `lib` folder of reveal.js and add the following line to your presentation before reveal.js initialization:
```
<script src="lib/rawdeflate.js"></script>
```

2. Add the file `plugin/plantuml.js` to the `plugin` folder of reveal.js and include the following line in your dependencies list of the reveal.js initialization:

```
{ src: 'plugin/plantuml.js', async: true }
```

Your folder structure:
* lib/deflate.js
* plugin/plantuml.js
* your_presentation.html

## Usage

PlantUML images can be created in the slides with `<img uml="..."/>` 

```<img uml="Bob->Alice : hello"/>```

This will show the generated image.

![](http://www.plantuml.com/plantuml/img/SyfFqhLppCbCJbMmKiX8pSd91m00)

Important: Double-quote characters `"` must be replaced by `&quot;` 
 
## License

MIT licensed

Copyright (C) 2020 Johannes Schildgen
