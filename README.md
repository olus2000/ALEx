# Awesome Library of Extensions
ALEx is meant to be a publicly avaliable repository of extensions for the [Quackery](https://github.com/GordonCharlton/Quackery) programming language created by [Gordon Charlton](https://github.com/GordonCharlton). At the time of its creation the language doesn't have a significant community that I know of, but I hope someone interested in Quackery finds this repo useful.

All extensions are described inside their files.

## Usage guide
There are a couple of ways to use ALEx depending on how much you are comfortable with downloading and how many extensions you need.

### Clone the repository
If you are going to be using almost every extension provided in the repository you can just clone it with git. They should be cloned into a folder 'ALEx' in the directory you are running Quackery from. Then you can copy the `ALEx-loader.qky` into the Quackery directory and add it to your `extensions.qky`. It will handle loading extensions from the 'ALEx' folder, just uncomment relevant lines in yout `ALEx-loader.qky`.

The added convenience is that any updates can be performed by pulling the repository and copying the `ALEx-loader.qky`.

### Download extensions and use ALEx-loader
If you wish to use a substantial amount of extensions provided here but don't want to clone the whole repo you can make the 'ALEx' folder yourself and download any extensions you need by hand. You then can download `ALEx-loader.qky`, uncomment relevant lines and add it to your `extensions.qky`. It will handle loading extensions from the 'ALEx' folder. Be careful to make sure that either your system supports `file.path` or you downloaded the `filepath.qky` extension.

### Download only extensions
If you only wish to use a couple of extensions you can just download them and add to your `extensions.qky`. They are just Quackery files after all, you don't need any fancy loaders to use them.

## Assumptions about the system
Some extensions may require the system with the [protect breaks bailed](https://github.com/GordonCharlton/Quackery/issues/3) issue resolved.

Some extensions may require `file.path` support which, if not provided by the system, can be loaded from `filepath.qky`. `ALEx-loader.qky` requires either `file.path` system support or `filepath.qky` among the extensions in the 'ALEx' folder.

## Contents
* `ALEx-loader.qky`

  Used to load extensions. Should be copied up a directory. Assumes the folder with ALEx extensions is called 'ALEx'.

  Author: [Aleksander "olus2000" Sabak](https://github.com/olus2000)

* `bigrat.qky`

  Big rational number operations.

  Author: [Gordon Charlton](https://github.com/GordonCharlton)

* `brainfuck.qky`

  brainfuck interpreter.

  Author: [Gordon Charlton](https://github.com/GordonCharlton)

* `filepath.qky`

  Support for relative and scoped paths.

  Author: [Aleksander "olus2000" Sabak](https://github.com/olus2000)

* `lookup-table.qky`

  Lookup table/association table/dictionary implementation.

  Author: [Aleksander "olus2000" Sabak](https://github.com/olus2000)

* `merge-sort.qky`

  Replaces the default sorting words with a more efficient algorithm.

  Author: [Gordon Charlton](https://github.com/GordonCharlton)
  
* `sundry.qky`

   Some words that were considered for Quackery core words but omitted for the sake of brevity.

   * `#` `footnotes` – more ways of making comments.
   * `[peek]` `[poke]` – like `peek` and `poke` but can dive into nested nests.
   * `switch` `case` `otherwise` – a switch statement.
   * `map` `filter` `reduce` – combinators.

  Author: [Gordon Charlton](https://github.com/GordonCharlton)


* `template.qky`

  Template for your own extension. Feel free to submit pull requests with your work.

  Author: [Aleksander "olus2000" Sabak](https://github.com/olus2000)
