# firefox_profile

## userChrome.css

Copy `userChrome.css` to your active Firefox profile directory, in a folder named `chrome`

## Sidebery Styles Editor

Paste this into Sidebery `Settings > Styles editor`

```css
#root.root {--toolbar-bg: rgb(43,42,51);}
#root.root {--tabs-inner-gap: 5px;}
#root.root {--frame-el-overlay-hover-bg: #092e54ff;}
#root.root {--general-margin: 4px;}
#root.root {--frame-bg: #000000ff;}
#root.root {--tabs-indent: 20px;}
#root.root {--general-border-radius: 10px;}
#root.root {--tabs-activated-bg: #7f7f7fff;}
#root.root {--tabs-activated-fg: #000000ff;}

/* Pinned Tabs Styling */
#root .TabsPanel .PinnedTabsBar {
  display: flex;
  flex-wrap: wrap;
  margin: 0;
  padding: 10;
}

.PinnedTabsBar .tab-wrapper {
  flex-grow: 1;
  min-width: 25px;
  --tabs-pinned-width: auto;
}

#root.root {
  --tabs-pinned-height: 36px;
}

/* Non-selected pinned tabs background */
.Tab[data-pin="true"] .body {
  background: #171717;  /* Change this color to whatever you want */
}

/* Push right edge of tabs leftward a bit to make room for the scrollbar.
See fix here: https://github.com/mbnuqw/sidebery/discussions/1581
*/
.TabsPanel > .ScrollBox > .bottom-shadow[data-show="true"] ~ .scroll-container,
.TabsPanel > .ScrollBox > .top-shadow[data-show="true"] ~ .scroll-container {
  padding-right: 8px;
}


/* Hide `Search...` text in Search Input area */
#root .SearchBar .placeholder {
    display: none;
}
```
