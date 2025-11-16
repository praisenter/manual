# Presenting
> Presenting is how you show content on a screen, projector, TV, etc. and manage that content over the duration of a service.
{: .p-man-page-intro}

All presentation control is handled from the Present tab on the left navigation.  It's the first place you will see after selecting a workspace.  From here, you can control everything around presentation, displays, queues, and more.  To review, each display you have configured is given it's own _display controller_ to control the content being presented to that display.  The below screenshot represents ONE display controller.  We'll go through each element of the display controller and explain it's function and call out any features.

![presentation display controller]({{ page.relpath }}assets/img/present-display-controller.png){: .rounded .img-fluid}

## Slide preview[#](#slide-preview)
Each _display controller_ has a slide preview.  It's the rectangle at the top of the controller that shows the slide before you present it.  The slide preview will be updated based on the actions you take on the display controller.  You must have a preview before you can show anything.

![presentation slide preview]({{ page.relpath }}assets/img/present-slide-preview.png){: .rounded .img-fluid}

## Show / hide[#](#show--hide)
Under the slide preview, there are two large buttons: `Show` and `Hide`.  These are your main controls for sending and clearing content from the attached display.  As mentioned above, you must have a slide preview before you can send content.

When you use the `Show` button, Praisenter will take the slide you have prepared in the preview, use it's transition, and show it on the display.  There are some interesting details in this one button that you should keep in mind:

- If a slide is currently displayed, it will be transitioned away using the transition of the new slide.
- If a slide is currently displayed, and that slide and the new slide are the same, Praisenter will attempt to transition the placeholder content of the slide only.  The background and other static content like pictures and videos will NOT transition.  This is the default, but it can be changed in the settings.
- If a slide is currently being transitioned in and you click the show button again, Praisenter will stop the current transition, and start a new transition with the new slide.  This is the default, but it can be changed in the settings as well.

The standard process of showing content on a display is to select the tab for the content to display: `Bibles`, `Song Lyrics`, `Slides`, or `Notifications` (more on these later), use the controls in the tab to _preview_ a slide, then click the `Show` button.

When you use the `Hide` button, Praisenter will use the transition on the currently displayed slide to transition it out.  Clicking `Hide` when nothing is displayed will have no effect.

## Preview Transition[#](#preview-transition)
The `Preview Transition` option allows you to see the transition of the slide before showing the slide on the display.  If the slide doesn't have a transition set, then it shows the preview as if this option was disabled.  This can be useful when you aren't sure how the slides will perform or you aren't sure if you configured the placeholders correctly.

## Auto-show[#](#auto-show)
The `auto-show` toggle is used to automatically show the slides on the display.  This can be a very useful feature when you are following along in the reading of a Bible verse or song lyrics.  For example, if you want to show the next Bible verse, you need to use the `>>` button, then click the `Show` button.  When you have auto-show enabled, you only need to click the `>>` button.

> **NOTE**: This feature can be a little tricky to get used to so be careful when enabling it.  The recommendation is to try it off hours to get a feel for the way it works.

## Add to queue[#](#add-to-queue)
The `Add to Queue` button will be talked about more in the [Queue Management](#queue-management) section, but put simply, it's a way to save what you have previewed for display later.  The idea is to prepare for a service where you may present Bible verses, song lyrics, and maybe a few other things and call those things up quickly as needed.  For example, you can search in the `Song Lyrics` tab for the songs being performed, click on a section to preview it, then click `Add to Queue` to _save it_ for later.

## Presenting Bible verses[#](#presenting-bible-verses)
Presenting Bible verses is performed using the `Bible` tab in the _display controller_.  

![presenting bibles tab]({{ page.relpath }}assets/img/present-bible-verses-tab.png){: .rounded .img-fluid}

Presenting Bible verses requires you to select a slide template first (remember a slide template is just a slide with [_placeholders_]({{ page.relpath }}index.html#placeholder-component)).

![presenting bibles select template]({{ page.relpath }}assets/img/present-bible-verses-template.png){: .rounded .img-fluid}

Once you selected a template, you should see the preview box show the first verse of the selected Bible.  Praisenter allows you to select a primary and secondary Bible.  The primary Bible is used for searching and navigation and the secondary Bible is used to show two versions/translations at one time (provided you've created a slide with the correct placeholders).

![presenting bibles select bibles]({{ page.relpath }}assets/img/present-bible-verses-bibles.png){: .rounded .img-fluid}

Once you've chosen the primary Bible you can then use the book, chapter, verse inputs, and the `Find` button to navigate to a verse directly.  The `<<` and `>>` buttons can be used to navigate to the previous or next verse respectively.  You can also use the `Search` button to search the primary Bible.  The numbers showing under the `<<` and `>>` buttons are the number of chapters in the currently selected book and the number of verses in the selected chapter (respectively).

> **NOTE**: Searching will be discussed later in the manual.

> **NOTE**: Another trick is if you hold down the <kbd>Ctrl</kbd> or <kbd>Command</kbd> key while using the `>>` button, Praisenter will append the verses to the slide instead of just going to the next one.

![presenting bibles navigation]({{ page.relpath }}assets/img/present-bible-verses-nav.png){: .rounded .img-fluid}

Lastly, as you navigate through the primary Bible, the `Previous verse` and `Next verse` are shown based on the current verse you have selected in the book, chapter, and verse fields.

![presenting bibles previous and next verses]({{ page.relpath }}assets/img/present-bible-verses-prev-next.png){: .rounded .img-fluid}

## Presenting song lyrics[#](#presenting-song-lyrics)
Presenting song lyrics is performed on the `Song Lyrics` tab in the _display controller_.

![presenting song lyrics tab]({{ page.relpath }}assets/img/present-song-lyrics-tab.png){: .rounded .img-fluid}

Presenting song lyrics requires you to select a slide template first (remember, a slide template is just a slide with [_placeholders_]({{ page.relpath }}index.html#placeholder-component)).

![presenting song lyrics template]({{ page.relpath }}assets/img/present-song-lyrics-template.png){: .rounded .img-fluid}

After selecting the template, you need to find the song you want to present. You do that by using the search.  In the example below, I've searched for a song with the word "song" in it.

> **NOTE**: Searching will be discussed later in the manual.

![presenting song lyrics find]({{ page.relpath }}assets/img/present-song-lyrics-find.png){: .rounded .img-fluid}

Once you've found the song, the primary lyrics will be automatically selected.  You can optionally select a secondary set of lyrics too.  In the example below, it selected the "My Special Song" lyrics.

> **NOTE**: Remember that a _song lyrics_ item in Praisenter contains multiple sets of _song lyrics_ all in the same document.  This allows you to show the lyrics side-by-side on a slide.

![presenting song lyrics lyric selection]({{ page.relpath }}assets/img/present-song-lyrics-lyrics.png){: .rounded .img-fluid}

Since the primary lyrics are auto-selected, the sections that make up the lyrics are show below as buttons.  For example, in the screenshot below, our sample song only has one section called `Verse 1`.  If the song had many sections, you would see a button for each one.  When you click a section, the slide preview will update with the content from that section.

![presenting song lyrics verses]({{ page.relpath }}assets/img/present-song-lyrics-verses.png){: .rounded .img-fluid}

Finally, at the bottom are the song comments.  Comments that are particularly useful are things like section order or notes for the person who is presenting the song.

![presenting song lyrics notes]({{ page.relpath }}assets/img/present-song-lyrics-notes.png){: .rounded .img-fluid}

## Presenting slides[#](#presenting-slides)
Presenting slides is performed on the `Slides` tab in the _display controller_.

> **NOTE**: Only slides without [_placeholders_]({{ page.relpath }}index.html#placeholder-component) will be shown here.

![presenting slides tab]({{ page.relpath }}assets/img/present-slides-tab.png){: .rounded .img-fluid}

On the `Slides` tab, you'll see all the slides available to be presented.

![presenting slide list]({{ page.relpath }}assets/img/present-slides-list.png){: .rounded .img-fluid}

If you have a lot of slides, you can use the search feature to search by name or tag to find the slide you are looking for.

![presenting slide search]({{ page.relpath }}assets/img/present-slides-search.png){: .rounded .img-fluid}

To preview a slide, just click on it!

## Presenting notifications[#](#presenting-notifications)
Notifications are intended to be quick alerts that are overlayed on top of whatever is currently on a display.  These alerts could be things like a reminder or something to get someones attention.  

![presenting notifications tab]({{ page.relpath }}assets/img/present-notifications-tab.png){: .rounded .img-fluid}

Next, select the notification slide template to use.

> **NOTE**: The template chosen should have a [_placeholder_]({{ page.relpath }}index.html#placeholder-component) component configured with `Type` = `Text` and `Variant` = `Primary`.

![presenting notifications template]({{ page.relpath }}assets/img/present-notifications-template.png){: .rounded .img-fluid}

Next, enter in the text you would like to have appear on the notification.

![presenting notification text]({{ page.relpath }}assets/img/present-notifications-text.png){: .rounded .img-fluid}

Because notifications are overlayed on top of anything that is currently displaying, the default `Show` and `Hide` controls are _not_ used.  Instead, you use the controls under the notification text field.

![presenting notification controls]({{ page.relpath }}assets/img/present-notifications-controls.png){: .rounded .img-fluid}

## Queue Management[#](#queue-management)
Whenever the [Slide preview](#slide-preview) is showing, you have the ability to _save_ that content to the Queue using the `Add to Queue` button.  Each _disply controller_ has a queue allowing you prepare content for each display independently.  A common scenario is to have song lyrics queued for one display and sermon notes queued for another.  

> **NOTE**: See the [Add to queue](#add-to-queue) section of the manual for more details.

![presenting queue example]({{ page.relpath }}assets/img/present-queue-ex.png){: .rounded .img-fluid}

You can add as many slides as you need to the queue, but having too many could make it difficult to swap between them.  One way to avoid too many slides in the queue is to only add the _first_.  For example, let's imagine you need to present the Bible verses Matthew 1:1-10.  Instead of adding one slide to the queue for each verse, only add a slide for the first verse.  Now, when you click on that slide in the in queue, the _display controller_ will switch to the `Bibles` tab, set the Bible, book, chapter, and verse.  Now if you need to show the other 9 verses, you just use the `>>` and `Show` buttons!  This applies to song lyrics too, just add a slide for one of the sections in the song and Praisenter will switch the _display controller_ to the `Song Lyrics` tab, set the selected song, and show all the section buttons for you to switch between them.

> **NOTE**: The queue for each display controller will be saved on close of the application.  Praisenter doesn't have an option to save queues (or slide shows) for reuse at this time.

> **NOTE**: Praisenter does not have an option to auto-play the queue.  To advance the queue, you must click on the slide and show it manually.

As you are adding slides to the queue, you may find you added them in the wrong order.  To re-order them, click and drag the slide to the correct position.  In the example below, I'm moving slide 3 above slide 2.

![presenting queue reorder]({{ page.relpath }}assets/img/present-queue-reorder.png){: .rounded .img-fluid}

![presenting queue reorder result]({{ page.relpath }}assets/img/present-queue-reorder-result.png){: .rounded .img-fluid}

You can remove slides from the queue by using the <kbd>Delete</kbd> key, the context menu `Delete` option, or the `Remove Selected` and `Remove All` buttons.

If you want to duplicate a slide, you can use the copy and paste [hotkeys]({{ page.relpath }}index.html#hotkeys), the context menu `Copy` and `Paste` options, or hold down the <kbd>Ctrl</kbd> or <kbd>Command</kbd> key while dragging a slide.  What's really cool is that you can copy, paste and move slides _between_ display controllers.

![presenting queue move between controllers]({{ page.relpath }}assets/img/present-queue-move-controller.png){: .rounded .img-fluid}

![presenting queue move between controllers result]({{ page.relpath }}assets/img/present-queue-move-controller-result.png){: .rounded .img-fluid}

## Bible searching[#](#bible-searching)
Praisenter provides a flexible bible searching feature to help find verses on the fly.  Click the `Search` button to bring up the search tool.  The seach tool combines the searching and filtering options, a results view, and a detail view when you click on an item in the results view.  The searching and filtering options are at the top, the results view on the left, and the detail view on the right.  

![presenting bible searching]({{ page.relpath }}assets/img/present-bible-verses-search.png){: .rounded .img-fluid}

When you perform a search, the results will be shown up to 100 matches.  If your search has more than 100 matches you'll see `Found 100+ matching results` in the bottom left corner.  You'll need to refine your search to reduce the number of matches.  When the results display, the words or phrases that matched the search will be highlighted.  In the example above, we searched for "grace" and each verse that matches has the word "grace" underlined and in blue.  The last result (the one that is currently selected) doesn't show the matched word because it's further in the verse.  When you click on the result in the list, the right pane will show the whole chapter and scroll you to the verse that matched.  The item with the blue line on the right is the verse that you clicked on.  It will also show the matched terms.

Within the search results you have the `Score`, `Reference`, and the `Text`.  The `Score` represents a _relevancy_ score.  The score is used to show results that might be most relevant to your search.  In the above example, John 1:16 has the highest relevance because it contains the search team twice AND those matched terms are very close to each other.

When you find the verse you are looking for you can either double click the row in the results or click the verse reference link on the left.  The copy icon next to the reference on the left will copy the verse reference and text.

> **NOTE**: You can append multiple verses from the search by holding down the <kbd>Ctrl</kbd> or <kbd>Command</kbd> key when double clicking a result or clicking a reference on the left.

The search tool allows you to search a single Bible at a time and, optionally, limit that search to single a Book.  You can also change how the search works using the `Search type` and `Match type` options.  The default search is to match the `Phrase` `Exact`ly.  Here's a list of the other options and their use:

Search Types:

- `Phrase` - Match on all the words _and_ the order the words were given.
- `All words` - Match on all the words but order doesn't matter.
- `Any words` - Match on any word.

Match Types:

- `Exact` - Match the phrase, all words, or any words exactly as provided.
- `Fuzzy` - Match the phrase, all words, or any words closely and score them based on how close they are to the provided search.

`Fuzzy` matching is a great way to try to find something that you don't remember exactly how it was phrased or spelled.  Praisenter will use the `Score` to order them based on their closeness to the original search.  In the example below, we searched on `then peter said repent` using a `Fuzzy` `Phrase` search.  It was able to find the verse I was looking for even though I left out two words.

> **NOTE**: To find what you are looking for quickly, try using `Exact` `All words` before using `Fuzzy`.  most often you'll know some key words and that will be a more effective search.  Use the `Fuzzy` search when exact searching fails.

> **NOTE**: To improve the results of `Fuzzy` searching, you should use uncommon words and longer words.  Using short or common words will cause the search to rank results higher than because of their frequency in the text.  A great example of this is the example below.  See how it highlighted the word `then`?  Well, `then` is very close to my search term `them`.

![presenting bible searching fuzzy search]({{ page.relpath }}assets/img/present-bible-verses-search-fuzzy.png){: .rounded .img-fluid}

## Song searching[#](#song-searching)
Song searching is nearly the same as Bible searching so this section will only call out any differences in behavior.  Please see the section above for basic searching features.

Song searching works a little differently to Bible searching due to the types of content that you can search.  In addition to being able to search the song lyrics, Praisenter will also search the song _name_, lyrics _titles_, and _keywords_.  When your search matches one of these items, the `Section` column will display `Metadata` to indicate that a match was detected outside of the song lyrics.

When you find what you are looking for, the behavior of selecting that item will depend on the search result type.  For example, in the screenshot below, if I double click on the first result, Praisenter will set the Song and Lyrics options and will list the sections on the display controller, but it will not update the slide preview.  This is because the match was the song title, not a section.  However, if the last result is double clicked, Praisenter will set the Song and Lyrics options, list the sections, _AND_ update the slide preview with the content of that section.  If you click the section name on the left, regardless of the result type, Praisenter will update the slide preview.

> **NOTE**: Song searching does not support appending lyrics using the <kbd>Ctrl</kbd> or <kbd>Command</kbd> key.

![presenting song searching]({{ page.relpath }}assets/img/present-song-lyrics-search.png){: .rounded .img-fluid}