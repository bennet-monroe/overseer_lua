# table > script (1) functions 
Documentation detailing key functions for thread creation and script management in GTA scripting.
### `create_thread(string name, function func)`

- **Parameters:**
  - `name` (string): The name assigned to the created thread.
  - `func` (function): The function to be executed repeatedly in the thread's loop.

- **Description:**
  Creates a new thread to run a specified function in a loop.

- **Usage:**
```lua
script.create_thread("THREAD_NAME", function(script)
    -- Add your scripts here, including natives, globals, locals, etc.
end)
```
