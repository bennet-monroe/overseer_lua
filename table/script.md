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
### `create_in_fiber(function func)`

- **Parameters:**
  - `func` (function): Function executed once within the fiber pool for efficient thread management.

- **Description:**
  Executes a function once in the fiber pool, allowing the use of natives and script utils such as yielding or sleeping.

- **Usage:**
```lua
script.create_in_fiber(function (script)
     -- Yielding until the next frame.
     script:yield()
end)
```
