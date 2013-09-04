# Sass for TextMate/Sublime Text 2

## What's this thingie?

This add-on adds syntax highlighting and tab/code completion for Sass and SCSS files. It features [Zen Coding](http://code.google.com/p/zen-coding/) shortcuts for many CSS properties, making you look like some kind of stylesheet wizard to everyone around you. You've got to like that.

## TextMate Installation

### With git

    mkdir -p ~/Library/Application\ Support/TextMate/Bundles/
    cd ~/Library/Application\ Support/TextMate/Bundles/
    git clone https://github.com/nathos/sass-textmate-bundle.git Sass.tmbundle
    osascript -e 'tell app "TextMate" to reload bundles'

### Without git
    mkdir -p ~/Library/Application\ Support/TextMate/Bundles
    cd ~/Library/Application\ Support/TextMate/Bundles
    mkdir sass-textmate-bundle.tmbundle && curl -L https://github.com/nathos/sass-textmate-bundle/tarball/master | tar xz --strip 1 -C sass-textmate-bundle.tmbundle
    osascript -e 'tell app "TextMate" to reload bundles'

## Sublime Text 2 Installation

### With Sublime Package Control

I recommend using the excellent [Sublime Package Control](http://wbond.net/sublime_packages/package_control) to install Sublime Text 2 packages.

Once you have Package Control installed, activate your Command Palette and choose ```Package Control: Install Package```.

Then, search for **"Sass"** and press Enter. In mere moments you'll be up and running with full syntax highlighting, tab completion and more. Huzzah!

### With Git (Windows)

From within Sublime Text go to:
```Preferences > Browse Packages...```

Right-click and select:
```Git Bash Here```

From the Git Bash: 
```git clone https://github.com/nathos/sass-textmate-bundle.git```

Restart Sublime Text.
    
### Putting HAML in its place

You may find that when you open files with the `.sass` extension, Sublime Text 2 initially interprets the syntax as HAML. To permanently fix this, open `Packages/Rails/Ruby Haml.tmLanguage` and delete the line `<string>sass</string>`.

Alternatively, you can open a sass file in Sublime Text (with either the .sass or .scss extension) and go to ```View > Syntax``` and select Sass. This will also ensure updated won't override this setting in future.

## About & Credit
This was originally a fork of <https://github.com/seaofclouds/sass-textmate-bundle>, and includes the best contributions of people [throughout the network](https://github.com/nathos/sass-textmate-bundle/network).

Features include imprpoved syntax highlighting, [Zen Coding](http://code.google.com/p/zen-coding/)-style property autocompletion, and more.