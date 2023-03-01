# Topics Snippets

Snippets that only work on a Topic page

## [anchor-query-parameter](./anchor-query-parameter.html)

Standard URL anchors don't work on Blackbaud, because the page URLs are already built around an anchor (grr). But, this does allow you to link to a heading or some other anchored feature on the page by adding an `anchor` query parameter:

```
https://example.myschoolapp.com/path/to/page?anchor=foo#blackbaud-navigation-anchor
```

To use, create anchors as normal (`<a name="foo">Anchored text</a>`) and then insert the `anchor` query parameter into your page URl (as above).

## [back-button-rename](./back-button-rename.html)

Realistically, the back button does not actually take you back unless you are coming from the Topics page. This renames the back button so that it makes more sense. (Could be renamed to anything you like by editing the snippet.)

## [back-to-bulletin-board](./back-to-bulletin-board.html)

Relinks the Back button on a topic page to take the user back to the Bulletin Board, rather than back to the topics page. (Perhaps more sensible, if you have built out a welcome/home page on the Bulletin Board and you have many, many topics).

## [redirect](./redirect.html)

Redirect visitors to a Topic page to another arbitrary location. Useful if you have shared a link to a Topic but have moved it to a new page, or would rather users go to a Google Doc or some other page after the fact.

The trick is in the caption of the embed: name it with the URL you would like to redirect to:

```
{{redirect:https://github.com/groton-school}}
```
