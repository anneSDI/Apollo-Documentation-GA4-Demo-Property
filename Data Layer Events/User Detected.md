# User Detected

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ page_data: null });  // Clear the previous page_data object.
dataLayer.push({
  "event": "detect_user",
  "detailed_event": "User Detected",
    "page_data": {
        "user_login_state": "<user_login_state>"
    },
    "user_data": {
        "anonymous_user_id": "<anonymous_user_id>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|page_data.user_login_state|string|Captures the current sign in status for the user \(i.e. signed\_out, signed\_in, unknown\).|logged in, logged out, guest|||||||
|user_data.anonymous_user_id|string|When a user is not logged in,, this captures an anonymous user id.||||||||




