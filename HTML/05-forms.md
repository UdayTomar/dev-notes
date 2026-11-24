# 05 — Forms

Forms collect user input and submit it to a server or process it with JavaScript.

## Basic form

```html
<form action="/submit" method="post">
  <label for="name">Name</label>
  <input id="name" name="name" type="text" required>

  <label for="email">Email</label>
  <input id="email" name="email" type="email" required>

  <button type="submit">Send</button>
</form>
```

Associate labels with controls. The `name` attribute identifies submitted data.

## Common input types

`text`, `email`, `password`, `number`, `tel`, `url`, `date`, `checkbox`, `radio`, `file`, `submit`.

## Other controls

```html
<label for="course">Course</label>
<select id="course" name="course">
  <option value="">Choose one</option>
  <option value="bca">BCA</option>
</select>

<label for="message">Message</label>
<textarea id="message" name="message" rows="4"></textarea>

<fieldset>
  <legend>Preferred contact</legend>
  <label><input type="radio" name="contact" value="email"> Email</label>
  <label><input type="radio" name="contact" value="phone"> Phone</label>
</fieldset>
```

## Validation attributes

- `required`: value must be provided.
- `min`, `max`: numeric/date boundaries.
- `minlength`, `maxlength`: text length.
- `pattern`: regular-expression constraint.
- `placeholder`: hint, not a label.
- `disabled`: disabled and not submitted.
- `readonly`: not editable, generally submitted.

Client-side validation does not replace server-side validation.

## GET vs POST

GET commonly requests data and puts form values in the URL query string. POST sends data in the request body. HTTPS protects data in transit; POST alone does not encrypt it.

## Practice
Build a registration form with name, email, password, date, course, radio buttons, checkbox, and submit.
