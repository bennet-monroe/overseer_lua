# table > tool (6) functions 
Documentation detailing key functions for tool management, including useful functions such as JOAAT hashes for GTAV models, logging, and notifications.

### `send_log(string title, string message)`

- **Parameters:**
  - `title` (string): The title of the log message.
  - `message` (string): The content of the log message.

- **Description:**
  Sends a log message with a specified title and content.

- **Usage:**
```lua
 tools.send_log("title", "message")
```

### `send_log(int color, string title, string message)`

- **Parameters:**
  - `color` (int): The color of the log message (using enum values from `log_color`).
  - `title` (string): The title of the log message.
  - `message` (string): The content of the log message.

- **Description:**
  Sends a log message with a specified color, title, and content.

- **Usage:**
```lua
tools.send_log(log_color.yellow, "title", "message")
```

### `send_notify(string title, string message)`

- **Parameters:**
  - `title` (string): The title of the notification.
  - `message` (string): The content of the notification.

- **Description:**
  Sends a notification with a specified title and content.

- **Usage:**
```lua
tools.send_notify("title", "message")
```

### `send_notify_log(string title, string message)`

- **Parameters:**
  - `title` (string): The title of the notification and log message.
  - `message` (string): The content of the notification and log message.

- **Description:**
  Sends a notification with a specified title and content, and also logs the message.

- **Usage:**
```lua
tools.send_notify_log("title", "message")
```

### `joaat(string string)`

- **Parameters:**
  - `string` (string): The input string for which the Jenkins One At A Time (JOAAT) hash will be calculated.

- **Returns:**
  - int

- **Description:**
  Calculates the Jenkins One At A Time (JOAAT) hash for the input string.

- **Usage:**
```lua
local hash = tools.joaat("string")
```

### `to_string(int value)`

- **Parameters:**
  - `value` (int): The integer value to be converted to a string.

- **Returns:**
  - string

- **Description:**
  Converts the integer value to its string representation.

- **Usage:**
```lua
local string = tools.to_string(123)
```
