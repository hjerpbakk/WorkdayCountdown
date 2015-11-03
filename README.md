# Workday Countdown
**Workday Countdown** is a countdown panel for [Panic's Status Board 2 application for iOS](https://itunes.apple.com/us/app/status-board/id449955536?mt=8&at=11l5UV). Different from the stock Countdown panel, Workday Countdown filters out weekends and public holidays. This provides a more realistic countdown in a work setting where people are not expected to come in on weekends.

## tl;dr
1. Change the `targetDate` variable on line 11.
2. Put `WorkdayCountdown.html` in your Dropbox.
3. Add a new `Do-It-Yourself` panel to your status board and choose this file from Dropbox.

<div style="width:100%; text-align:center">
	<img src="http://hjerpbakk.com/s/Setup.png" alt="star" width="686.0" height="614.5">
</div>

## Usage

`WorkdayCountdown.html` contains everything you need. On line 7 you’ll see a section containing the variables you’ll need to change:

### targetDate
`targetDate` is the date to which the panel countdowns. Change this to your own target date. This is a normal JavaScript date, but minutes is the smallest unit shown by the panel.

<div style="width:100%; text-align:center">
	<img src="http://hjerpbakk.com/s/Days-remaining.png" alt="star" width="350.0" height="350.0">
</div>

<div style="width:100%; text-align:center">
	<img src="http://hjerpbakk.com/s/Hours-remaining.png" alt="star" width="350.0" height="350.0">
</div>

<div style="width:100%; text-align:center">
	<img src="http://hjerpbakk.com/s/Minutes-remaining.png" alt="star" width="350.0" height="350.0">
</div>

### publicHolidays
`publicHolidays` is the number of public holidays during the countdown period. This number must be set manually, and will be subtracted from the countdown. If the holiday falls on a weekend, do not add it here.

### countdownCompleted
`countdownCompleted` is the URL to the image to be shown when the countdown completes. It defaults to:

<div style="width:100%; text-align:center">
	<img src="http://hjerpbakk.com/s/Countdown-completed.jpg" alt="star" width="150.0" height="150.0">
</div>

### title
`title` is the title of this page if shown in a regular browser.

## Hosting

The panel can be hosted in two ways.

### Through Dropbox

1. Put `WorkdayCountdown.html` in your Dropbox.
2. Add a new `Do-It-Yourself` panel to your status board and choose this file from Dropbox.

### Using your favourite web server.

1. Serve `WorkdayCountdown.html` using your favourite web server.
2. Add a new `Do-It-Yourself` panel to your status board and choose the correct URL.

## Advanced

### Status Board meta tag
On line 4 there is information about how Workday Countdown should behave when placed on your status board. The attributes and allowed values are documented on [Panic’s site](https://library.panic.com/status-board/diy-panels/).

### CSS
If you want a different look and feel, you can change the CSS starting on line 61. The default CSS is created to make it look as similar as possible to Panic’s own Countdown panel.

<div style="width:100%; text-align:center">
	<img src="http://hjerpbakk.com/s/Side-by-side.png" alt="star" width="600.0" height="350.0">
</div>



