Structure
---------

Structure is the only obligatory file to have in Gutenberg.  
Structure is a file called `structure` in `book` folder with any extension.

Structure is hooked up first and should be a barebone of your README.
For example, this repo README's structure looks like this:

```md
{{structure}}
```

As you see, `books/introduction.md` can be loaded just using Mustache's
{{mustache_introduction}} variable. So treat `structure.md` like you’d treat
a bookcover for your book pages (I won't ever call it `bookcover`, I swear).

This one includes all built-in Gutenberg mixins and sets your repo to 'sword'
and user to 'somu'. Those two variables are very important in Gutenberg. After
setting them, you can easily generate a header, for example, using built-in
{{mustache_header}} variable, so in that case you'd receive something like this
for your {{mustache_header}}:

    Sword
    =====

After you've setup books folder, start creating pages inside it. They will be
automatically hooked and put into a variable with the same name: you can use
them in your `structure.md`.

To understand how to write all this template things, just look into this repo's
book folder. I love eating my own dog food. In fact, I cook it for myself.
Barkety bark.