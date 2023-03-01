# Shared Snippets

Snippets that can be used anywhere

## [checkboxes-stored-as-cookies](./checkboxes-stored-as-cookies.html)

Show a checkbox on a page that a student can check… that will stay checked for that student until they uncheck it (or switch browsers). Useful for self-maintained to do lists.

Note that you will need to repeat the `<label><input…` line once for each checkbox, give each checkbox a unique name, and then, at the bottom of the snippet, add a `trackWithCookie(...` line for each checkbox using those exact same names.

## [google-analytics](./google-analytics.html)

What it says on the tin. Track page views using Google analytics. You'll need to set up the Google Analytics yourself, and then get the measurement ID int the format `G-XXXXXXXXXX` from it to paste into the snippet.

## [hide-embed](./hide-embed.html)

Looks for a widget on the page with the same caption as the `caption` variable, and hides it. Useful in combination with practically every other snippet.

## [lightbox2](./lightbox2.html)

Use the Lightbox2 JavaScript library to make embedded images clickable to zoom in.

Directions on how to write the image HTML are on the [Lightbox website](https://lokeshdhakar.com/projects/lightbox2/#getting-started:~:text=INITIALIZE%20WITH%20HTML).

One useful trick is to create an already-expired topic in your course or group in which you put all the images you want to use in a Photos widget. This lets you host the images on Blackbaud (don't worry -- being expired won't make them inaccessible) and then you can copy the image URLs for your `<img>` tags in your HTML in other topics.

## [placeholders](./placeholders.html)

Replace a placeholder on your page with dynamically-generated values.

In the example in the snippet, I didn't want to have to remember to update the page with new dates every year, so I had the page look for everywhere I had put `<span class="school-year">{{year}}</span>` and replace it with the actual year in question (calculated based on the date the page is visited).

(It's looking for that `class="school-year"` value, not the `{{year}}`, which is just a visual reminder on the page that I have placeholders that will be replaced.)
