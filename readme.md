
# CSS3 Please snippets for SnipMate

This is a collection of CSS snippets for the [SnipMate VIM
plugin](http://www.vim.org/scripts/script.php?script_id=2540), based on
the wonderful [css3please](http://css3please.com) website.

I'm using css3-please nearly every day, this is an essential part of my
CSS authoring workflow. As a lazy-developer, everytime I go there to
copy and paste some awesome CSS rules I feel like I could stay in the
comfort of my VIM session. and simply start typing something like
`transition<TAB>`.

And then I would have the according snippet from css3-please
automatically, copy-pasted into my buffer, with appropriate placeholder.
That would make me a happy developer.

## Installation

Put the `css` directory in your `~/.vim/snippets` directory and you're done.

For the snippets to work, the filetype needs to be `css`.

## Snippets

```sh
├── 3dtransforms.snippet
├── animation.snippet
├── bgsize.snippet
├── boxshadow.snippet
├── columns.snippet
├── font.snippet
├── gradient.snippet
├── opacity.snippet
├── rgba.snippet
├── rotate.snippet
├── round.snippet
├── scale.snippet
├── tabsize.snippet
├── textshadow.snippet
└── transition.snippet
```

## Example

Typing the `transition` trigger word followed by a `<tab>`

```css
transition<tab>
```

will expand the following CSS snippet:

```css
  -webkit-transition: all 0.3s ease-out;
     -moz-transition: all 0.3s ease-out;
      -ms-transition: all 0.3s ease-out;
       -o-transition: all 0.3s ease-out;
          transition: all 0.3s ease-out;
```

To go to the next item placeholder, simply `<tab>` over to it; if there is
repeated code, such as the "all" variable in this example, you can simply
start typing once it's highlighted and all the matches specified in the
snippet will be updated.

#### todo

* rotate

rotate snippet ommits filter for ie6-ie9. Requires conversion from deg
to appropriate matrix (=/)

    filter: progid:DXImageTransform.Microsoft.Matrix(
           M11=0.9914448613738104, M12=-0.13052619222005157,M21=0.13052619222005157, M22=0.9914448613738104, sizingMethod='auto expand');

* same goes for the scale snippet

* same goes for the rgba snippet

