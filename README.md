Ext.field.TimePicker
====================

A time picker form field for Sencha Touch 2.0

About
-------------------------

TimePicker adds easy-to-use and easy-to-configure  time-picking abilities to your Sencha Touch 2.0 forms. Like the Ext.field.DatePicker, TimePicker displays a OS-like picker that allows the user to select a specific time. 

Although TimePicker allows you to selectively create "time" values via segments, it inevitably treats the value like a single date, so keep this in mind when use it to bind to your models.

Currently, TimePicker allows you to configure 5 slots:
* Hour
* Minute
* Second
* Millisecond
* Meridiem (e.g., AM/PM)

Installation
------------
Installing this is super simple. Simply copy both js files into your SDK's src/ux folder.

NOTE: Both files are required as TimePicker relies on Ext.ux.picker.Time for it's implementation of the picker.

Configuration
-------------

Configuring TimePicker, like DatePicker, is a combination of setting up config for both classes. All configuration for the picker needs to be set via the "picker" config within Ext.field.TimePicker:

> Ext.create('Ext.field.TimePicker', {
>     picker: {
>       // Ext.ux.picker.Time config here...
>     }
>});

###Ext.ux.field.TimePicker Configuration
* dateFormat {String} The format to be used when displaying the value in the field
* default {String} The default string representation of the time to use. Example: '8:00', '14:50'

###Ext.ux.picker.Time Configuration
* AMText {String} The text to use for the ante-meridiem
* PMText {String} The text to use for the post-meridiem
* endHour {Number} The end hour for the time picker
* endMillisecond {Number} The end millisecond for the time picker
* endMinute {Number}The end minute for the time picker
* endSecond {Number} The end second for the time picker
* hourIncrement {Number} The increment value for hour
* hourList {Array} Array of hours to use in the hour picker
* hourText {String} The text to use for the hour title
* meridiemText {String} The text to use for the meridiem title
* millisecondIncrement {Number} The increment value for millisecond
* millisecondList {String} Array of hours to use in the millisecond picker
* millisecondText  {String} The text to use for the millisecond title
* minuteIncrement {Number} The increment value for minute
* minuteList {Array} Array of hours to use in the minute picker
* minuteText {String} The text to use for the minute title
* secondIncrement {Number} The increment value for second
* secondList {Array} Array of hours to use in the second picker
* secondText {String} The text to use for the second title
* slotOrder {Array} The order of slots in the picker
* startHour {Number} The start hour for the time picker
* startMillisecond {Number} The start millisecond for the time picker
* startMinute {Number} The start minute for the time picker
* startSecond {Number} The start second for the time picker
