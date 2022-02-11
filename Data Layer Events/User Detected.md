# User Detected

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({ page_data: null });  // Clear the previous page_data object.
dataLayer.push({
  "event": "User Detected",
    "event_data": {
        "user_sign_in_status": "<user_sign_in_status>"
    },
    "page_data": {
        "anonymous_user_id": "<anonymous_user_id>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|anonymous_user_id|string|When a user is not logged in,, this captures an anonymous user id.||||||||
|user_sign_in_status|string|Captures the current sign in status for the user \(i.e. signed\_out, signed\_in, unknown\).|logged in, logged out, guest|||||||




