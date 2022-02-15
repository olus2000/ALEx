# Awesome Library of Extensions
ALEx is meant to be a publicly avaliable repository of extensions for the
[Quackery](https://github.com/GordonCharlton/Quackery) programming language
created by [Gordon Charlton](https://github.com/GordonCharlton).
At the time of its creation the language doesn't have a significant community
that I know of, but I hope someone interested in Quackery finds this repo useful.

All extensions are described in detail inside their files.

## Usage guide
There are a couple of ways to use ALEx depending on how much you are comfortable
with downloading and how many extensions you need. For **ALEx-loader config guide**
check `ALEx-loader.qky`.

### Clone the repository
If you are going to be using almost every extension provided in the repository
you can just clone it with git. Then you can copy the `ALEx-loader.qky`
into the Quackery directory and configure it properly.
You will then be able to load any extension in the folder.

The added convenience is that any updates can be performed by pulling
the repository and copying the `ALEx-loader.qky` if it was updated.

### Download extensions and use ALEx-loader
If you wish to use a substantial amount of extensions provided here
but don't want to clone the whole repo you can download any extensions you need
by hand into a dedicated folder. You then can download `ALEx-loader.qky`
and configure it properly.

Be careful to make sure that you have met all
dependencies, including `filepath` for `ALEx-loader.qky`.

### Download only extensions
If you only wish to use a couple of extensions you can just download them
and add to your `extensions.qky`. They are just Quackery files after all,
you don't need any fancy loaders to use them.

You may need to comment out lines at the start of extensions that depend on
other extensions. Make sure to load them in the correct order so all dependencies
are met.

## Assumptions about the system
Some extensions may require `filepath` support which, if not provided by the system,
can be loaded from `filepath.qky`. `ALEx-loader.qky` requires either `filepath`
system support or `filepath.qky` to be loaded beforehand.

Some extensions may depend on other extensions.

## Contents
* `ALEx-loader.qky`

  Includes a word for loading the extension and a configurable path for the
  extension folder.

  Author: [Aleksander "olus2000" Sabak](https://github.com/olus2000)

* `template.qky`

  Template for your own extension. Feel free to submit pull requests with your work.

  Author: [Aleksander "olus2000" Sabak](https://github.com/olus2000)

* `bigrat.qky`

  Big rational number operations.

  Author: [Gordon Charlton](https://github.com/GordonCharlton)

* `binary-search.qky`

  Rightmost binary search.

  Author: [Gordon Charlton](https://github.com/GordonCharlton)

* `brainfuck.qky`

  brainfuck interpreter.

  Author: [Gordon Charlton](https://github.com/GordonCharlton)

* `filepath.qky`

  Support for relative and scoped paths. Obsolete with current versions of Quackery.

  Author: [Aleksander "olus2000" Sabak](https://github.com/olus2000)

* `higher-order.qky`

  Higher order functions. `fold`, `foldr`, `map`, `filter`

  Author: [Gordon Charlton](https://github.com/GordonCharlton)

* `literal.qky`

  A word for proceduraly generating values at build-time.

  Author: [Aleksander "olus2000" Sabak](https://github.com/olus2000)

* `lookup-table.qky`

  Lookup table/association table/dictionary implementation.

  Author: [Aleksander "olus2000" Sabak](https://github.com/olus2000)

* `merge-sort.qky`

  Replaces the default sorting words with a more efficient algorithm.

  Author: [Gordon Charlton](https://github.com/GordonCharlton)

* `priority-queue.qky`

  Priority queue implementation.

  Author: [Gordon Charlton](https://github.com/GordonCharlton)

* `sundry.qky`

   Some words that were considered for Quackery core words.

   * `#` `footnotes` – more ways of making comments.
   * `[peek]` `[poke]` – like `peek` and `poke` but can dive into nested nests.
   * `switch` `case` `otherwise` – a switch statement.

  Author: [Gordon Charlton](https://github.com/GordonCharlton)

* `types.qky`

  A simple object system for easy polimorphism.
  
  Depends on: `lookup-table.qky`

  Author: [Aleksander "olus2000" Sabak](https://github.com/olus2000)
