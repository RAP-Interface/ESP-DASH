---
{
  "title": "ESP-DASH Wiki: Status Card"
}
---
## Status Card


#### Preview:
<br>

<img src="~@assets/status-card-idle.png" width="280px" alt="Preview">
<img src="~@assets/status-card-success.png" width="280px" alt="Preview">
<img src="~@assets/status-card-warning.png" width="280px" alt="Preview">
<img src="~@assets/status-card-danger.png" width="280px" alt="Preview">

<br>
<br>

As it's name suggests, status card is used to display some kind of status on your dashboard. It can show 4 different kinds of status along with a short message.

<br>

#### Type:
`STATUS_CARD`

<br>

#### Valid Data Types:
- `String`

<br>

#### Valid Statuses:
- `"success"` - Green
- `"danger"` - Red
- `"warning"` - Yellow
- `"idle"` - Grey

<br>

#### Initializer:
```cpp
/* 
  Status Card
  Valid Arguments: (ESPDash dashboard, Card Type, const char* name, const char* status (optional) )
*/
Card card1(&dashboard, STATUS_CARD, "Test Status", "success");
```

<br>

#### Updaters:

Status card updater allows you to set a message:

```cpp
card1.update("message");
```

Or, message + status at the same time:
```cpp
card1.update("Message", "success");
```