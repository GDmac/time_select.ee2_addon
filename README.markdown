**Time Select** is an EE2 fieldtype that offers a configurable dropdown menu of times. Its intended use is for events channels.

## Usage

After installing and activating Time Select, choose it as your fieldtype in either a custom field or Matrix field. You have two configuration options for each Time Select field:

* **Display Style**: whether to show the time in 12-hour or 24-hour format on the publish screen.
* **Time Increments**: you can choose to have the time options increment by 15 minutes, 30 minutes, or 1 hour.

## Template Tags

When displaying your field within your templates, you can format the output using standard PHP date tokens (see the **Time** section of the [PHP date() function documention](http://php.net/manual/en/function.date.php)). If you don't format your field outout, the time's value in seconds will be displayed.

Example:

`{my_time_field format="g:ia"}`

This yields *7:00pm*.

*Time Select has been tested with ExpressionEngine 2.1.3, and is compatible with Matrix fields.*