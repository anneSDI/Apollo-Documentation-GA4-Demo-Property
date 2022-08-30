# Link Clicked

### This event is used for cases in which an anchor tag is used as a link.

For example, if an `<a>` tag is used to represent a  link, you would need to add these attributes to trigger the event to be collected when the anchor is clicked.

Do not include the “data-dom-event” data attribute on any other elements that you do not want to be tracked.

Check the implementation notes for data-dom-event descriptions.
```
<a
  data-dom-dom_event="<dom_event>"
  data-dom-link_text="<link_text>"
  data-dom-link_url="<link_url>"
>
```

## Parameters Definitions

|Data Attribute Name|Data Source Type|Data Source|Description|
| --- | --- | --- | --- |
|dom_event|Custom Code|Custom Code|The value in the data-dom-event attribute|
|link_text|Static|Static|The HTML\/CSS ID of the link.|
|link_url|Static|Static|The full text of the link.|



