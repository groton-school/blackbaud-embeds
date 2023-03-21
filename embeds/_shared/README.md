# Shared Snippets

Snippets that can be used anywhere -- just paste the contents of a file into an embed widget in Blackbaud (some of them may require updating some specific information).

For snippets that work on Bulletin Board pages specifically, [click here](../bulletin-board#bulletin-board-snippets).

For snippets that work on Topics pages specifically, [click here](../topics#topics-snippets).

## [google-analytics](./google-analytics.html)

[Click here to get the `google-analytics` embed snippet](./google-analytics.html)

What it says on the tin. Track page views using Google analytics. You'll need to set up the Google Analytics yourself, and then get the measurement ID int the format `G-XXXXXXXXXX` from it to paste into the snippet.

## hide-by-date

[Click here to get the `hide-by-date` embed snippet](./hide-by-date.html)

Hide HTML elements based on an annual date -- e.g. "before May 1" or "after November 12". Embed the script and then write HTML anywhere on the age that includes the `data-hide-until` or `data-hide-after` attributes in the element to be hidden. The date format can be anything that Javascript can parse, and is always assumed to be in the current year.

```html
<div data-hide-until="mar 14" data-hide-after="3/14">
  I only appear on &pi; day!
</div>
```

Faculty visitors to the page will see a note about when the element is visible.

## hide-embed

[Click here to get the `hide-embed` snippet](./hide-embed.html)

Looks for a widget on the page with the same caption as the `caption` variable, and hides it. Useful in combination with practically every other snippet.

## lightbox2

[Click here to get the `lightbox2` snippet](./lightbox2.html)

Use the Lightbox2 JavaScript library to make embedded images clickable to zoom in.

Directions on how to write the image HTML are on the [Lightbox website](https://lokeshdhakar.com/projects/lightbox2/#getting-started:~:text=INITIALIZE%20WITH%20HTML).

One useful trick is to create an already-expired topic in your course or group in which you put all the images you want to use in a Photos widget. This lets you host the images on Blackbaud (don't worry -- being expired won't make them inaccessible) and then you can copy the image URLs for your `<img>` tags in your HTML in other topics.

## placeholders

[Click here to get the `placeholders` snippet](./placeholders.html)

Replace a placeholder on your page with dynamically-generated values.

In the example in the snippet, I didn't want to have to remember to update the page with new dates every year, so I had the page look for everywhere I had put `<span class="school-year">{{year}}</span>` and replace it with the actual year in question (calculated based on the date the page is visited).

(It's looking for that `class="school-year"` value, not the `{{year}}`, which is just a visual reminder on the page that I have placeholders that will be replaced.)

## remember-checkboxes

[Click here to get the `remember-checkboxes` snippet](./remember-checkboxes.html)

Show a checkbox on a page that a student can check… that will stay checked for that student until they uncheck it (or switch browsers). Useful for self-maintained to do lists.

Note that you will need to include the `data-stored` attribute and a unique (to the page) `name` attribute for each checkbox:

```html
<label>
  <input type="checkbox" name="unique" data-stored />
  Click me! I'm unique. And I'll remember you!
</label>
```
