Bootstrap has a 12 col grid.

```css
grid-template-rows: 80vh min-content 40vw repeat(3, min-content);

grid-template-rows: 80vh min-content 40vw repeat(3, min-content);
```

grid-template-columns: repeat(8, minmax(min-content, 14rem));

We want to have 8 columns and want the width of each of these columns to be between their minimum content(viewport) and 140px, 8 rem for sidebar

grid-template-columns: 8rem repeat(8, minmax(min-content, 14rem));

Full bleed section/layout

We started with 8 columns layout & on the left side we added a sidebar then we added 1fr on the left side and on the right side which occupies all the remaining space in order to in order to center these 8 columns in the middle of the page.

Had side bar not been there then we would have used margin: auto to center the 8 columns layout in in the middle of the page.

Sidebar

```css
grid-column: sidebar-start / sidebar-end;
grid-row: 1/-1;
```

We want the sidebar to start from the grid line sidebar start, end at sidebar-end

6 out of 8 columns are for header here, 2 of 8 for realtors
The columns in the middle are so useful because they allow us to build different kinds of designs.
