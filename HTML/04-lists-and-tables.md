# 04 — Lists and tables

## Unordered list

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```

## Ordered list

```html
<ol>
  <li>Plan</li>
  <li>Design</li>
  <li>Build</li>
</ol>
```

Use `ol` when sequence matters and `ul` when it does not.

## Description list

```html
<dl>
  <dt>HTML</dt>
  <dd>Describes webpage structure.</dd>
  <dt>CSS</dt>
  <dd>Controls presentation and layout.</dd>
</dl>
```

## Tables

Use tables for tabular data, not page layout.

```html
<table>
  <caption>Weekly study plan</caption>
  <thead>
    <tr><th scope="col">Day</th><th scope="col">Topic</th></tr>
  </thead>
  <tbody>
    <tr><th scope="row">Monday</th><td>HTML forms</td></tr>
    <tr><th scope="row">Tuesday</th><td>CSS selectors</td></tr>
  </tbody>
</table>
```

Important elements: `table`, `caption`, `thead`, `tbody`, `tfoot`, `tr`, `th`, `td`. Use `scope` to clarify header relationships. `colspan` and `rowspan` span cells.

## Practice
Create a timetable with a caption, header row, and at least three data rows.
