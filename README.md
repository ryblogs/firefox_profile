# firefox_profile

## userChrome.css

Copy `userChrome.css` to your active Firefox profile directory, in a folder named `chrome`

## Sidebery Styles Editor

Paste this into Sidebery `Settings > Styles editor`

```css
#root.root {--tabs-inner-gap: 5px;}
#root.root {--frame-el-overlay-hover-bg: #092e54ff;}
#root.root {--general-margin: 4px;}
#root.root {--frame-bg: #000000ff;}
#root.root {--toolbar-bg: rgb(43,42,51);}
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
```
