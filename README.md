# Using the Sellout Checkout Modal

### Embedding the modal

The Sellout Checkout modal can easily be embedded on any website via a simple script in the head tag of an HTML document. The script is below.

```.html
<script src="https://embed.sellout.io/embed.js"></script>
```
The above script should be placed in the head of the HTML document as illustrated below.

```.html
<head>
  <!-- Other script, meta, link, etc tags here --->
  <script src="https://embed.sellout.io/embed.js"></script>
</head>
```

The modal is now loaded on the page.

### Opening the modal

This step requires an EVENT_ID string value that looks something like `qQxc3bJS`. The EVENT_ID for your event will be different, but you can use the provided EVENT_ID to test the integration. If you do not know how to get the EVENT_ID for your event, please contact the Sellout Team.

The script loaded above exposes a JavaScript object at `window.Sellout` that allows you to interact with the Sellout Checkout Modal. To open the modal, call `window.Sellout.open('qQxc3bJS')`. Replace the first parameter with your EVENT_ID to open the modal with your event details.

An example of how this might look in an HTML document:

```.html
<div onClick="window.Sellout.open('qQxc3bJS')">Buy Tickets</div>
```

