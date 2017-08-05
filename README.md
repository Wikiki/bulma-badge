# bulma-badge
Bulma extension element named "badge" to display a number on text, button, ... 

Preview
-----

![Badge Element](https://img15.hostingpics.net/pics/241524ScreenShot20170726at124229.png)

Usage
-----

```html
<div class="column is-8">
  <div class="block">
    <span class="badge" data-badge="">
      Notifications
    </span>
    <span class="badge" data-badge="8">
      Notifications
    </span>
    <span class="badge" data-badge="88">
      Notifications
    </span>
    <span class="badge" data-badge="888">
      Notifications
    </span>
  </div>
  <div class="block">
    <button class="button badge" data-badge="">Button</button>
    <button class="button badge" data-badge="8">Button</button>
  </div>
  <div class="block">
    <button class="button is-primary badge" data-badge="">Button</button>
    <button class="button is-primary badge" data-badge="8">Button</button>
  </div>
</div>
```


Integration
---
- Clone the [bulma repo](https://github.com/jgthms/bulma)
- Under the `sass` folder, create a new folder called `extensions`
- In this new folder, create a new file `badge.sass`
- Copy the code form the `bulma-badge repo`'s [badge.sass](https://github.com/Wikiki/bulma-badge/blob/master/badge.sass) file into your new file
- In the same folder create a new file `_all.sass` (this is not required, but will help when you add more extensions)
- In this file add this code:
```
@charset "utf-8"
@import "badge.sass"
```
At the end of the `bulma.sass` file, add this line: `@import "sass/extensions/_all"`

Now, you can just build the bulma project with `npm run build`, and the output will be available in the `css folder`.
