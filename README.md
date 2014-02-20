jQuery weekpicker
=================

A weekpicker addon for the jQueryUI datepicker.

Usage
-----

The weekpicker is an extension of the datepicker. As such, all datepicker options are supported. Example:

```js
$('#selector').weekpicker({
    // options ...
});
```

There are only a three new options:

* `weekLength`: The length of the week in days. Defaults to 7. Use 5 to select from e.g. Monday-Friday.
* `startField`: Element or jQuery expression for an input field that will receive the start of the selected week.
* `endField`: Element or jQuery expression for an input field that will receive the end of the selected week.

Tips
----

If you are only interested in the start of the week, you can set the `startField` equal to the weekpicker element. Example:

```js
$('input.weekpicker').each(function (i, el) {
    $(el).weekpicker({
        firstDay: 1,
        startField: el
    });
});
```

This will override the value in the date field with the start of the week.
