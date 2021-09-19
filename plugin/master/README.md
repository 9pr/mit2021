# Reveal.js Master Plugin

Headers, Footers and conditional Page-Numbering for Reveal.js


## Initialization

```javascript
Reveal.initialize({
    master: {
        header: {
            size:  '60%',
            left:  'Great Presentation',
            right: '<img src="image.png" height="100px" />',
        },

        footer: {
            size:   '60%',
            left:   'John Doe',
            center: 'Fancy Something',
            right:  '#{slideNumber} / #{slideCount}'
        }
    },

    controls: false,
    dependencies: [
        /* [...] */
        { src: 'master.js', async: true }
    ]
});
```

## Usage

```html
    <div class="reveal">
        <div class="slides">
            <section header="false" footer="false" count="false">
            	Title Slide
            </section>
            <section>
                Slide with header and footer.
            </section>
            <section footer="false" count="false">
                Uncounted slide with header only.
            </section>
            <section>
                Another slide with header and footer.
            </section>
            <section header="false">
                Counted slide without header.
            </section>
            <section header="false" footer="false" count="false">
                Questions?
            </section>
        </div>
    </div>
```

## License

   Copyright 2016 Peter Heisig

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
