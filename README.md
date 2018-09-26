# DecaStore technical road-map presentation

The presentation explains the choice for [Ruby on Rails](http://rubyonrails.org/) API as a back-end framework and [Ember JS](https://emberjs.com/) as a front-end framework.

### Installation

You will need Ruby `2.4.0` and `reveal-ck` gem.
Once Ruby installed, run `bundle install`.
All the slides are coded in [Markdown](https://guides.github.com/features/mastering-markdown/#what) language and are in `slides.md` file.

### Running

The presentation uses [Reveal-ck](http://jedcn.github.io/reveal-ck/).

- `reveal.js`  presentations are html.
- __Ruby__ is good at producing html.

- Navigate to your presentation project as `cd decastore-presentation` in your Terminal.
- Run the command `reveal-ck generate` . Your slides will be created in the `slides/` directory.
- You can run reveal-ck's built-in webserver with `reveal-ck serve`.
- View the slide deck generated from this single file `slides.md` by opening your browser to http://localhost:10000.
- You can also just open `slides/index.html` page in your preferred browser to see the result.

### PDF presentation

The generated PDF version is in `decastore-presentation.pdf` file.
You can regenerate it using [decktape](https://github.com/astefanutti/decktape) as follows:

- install decktape as described in the [doc](https://github.com/astefanutti/decktape/blob/master/README.adoc)
- open your terminal and start reveal-ck server: `reveal-ck serve`
- run the following decktape command from the terminal:
```
decktape generic --slides 1-60 --s 1366x768 http://localhost:10000 ~/Downloads/decastore-presentation.pdf
```
 The generated PDF file `decastore-presentation.pdf` will be saved to `~/Downloads/decastore-presentation.pdf`.

 You can use other available options, see **Decktape** documentation for more details.
