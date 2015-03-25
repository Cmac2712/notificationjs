# Notificationjs

A simple javascript library for displaying notifications in the browser.

Vanilla javascript. No dependancies.

View example here: [cmac2712.github.io/notificationjs](http://cmac2712.github.io/notificationjs)

## Setup

Just include the css in your project (or you can compile the scss yourself) 

```HTML
<link rel="stylesheet" href="styles/main.css">
```
And include the js before the closing \</body\> tag.

```HTML
<script src="lib/notificationjs.min.js"></script>
```

## Usage 

To create a new notification: 

```javascript
var myNotification = new Notification({
			    title: "My Notification",
			    description: "Lorem ipsum dolar sit amet",
			    image: "images/my-image.jpg",
			    imageAlt: "My Image",
			    enterClass: "animated fade-in", 
			    exitClass: "animated fade-out",
			    duration: 5000
});
```

enterClass, and exitClass are classess added just after initiation and after the specified duration.

To activate the notification:

```javascript
myNotification.go();
```

