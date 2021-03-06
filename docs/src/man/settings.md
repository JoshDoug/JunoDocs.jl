# Settings

**Julia Path**: The location of the Julia binary. This is the command that Atom uses to call Julia. It defaults to the command `julia` which requires that Julia has been added to the path. If Julia is not in the path, this must be the path to the Julia binary.

#### Julia Options
**Arguments**: Sets the `ARGS` variable to emulate calls to `julia script.jl arg1 arg2`.
**Boot Mode**: This is the type of process list that atom-julia-client is using.
  -  The default is `Basic`, which only has one process running at a time.
  - `Cycler` instead has a process queue per window, meaning that if you quit the REPL (`Ctrl+j`+ `Ctrl+k`) then there exists an already running process which will seamlessly replace it.

**Console Style**: Switch between a REPL-based console (default) and the legacy
HTML based console.

**Deprecation Warnings**: Checkbox for whether to show the Julia deprecation warnings in the console.

**Number of Threads**: Sets the number of threads -- `global` will use whatever is set in `$JULIA_NUM_THREADS` and `auto` will set it to the number of physical cores.

**Optimization Level**: Sets the `-O` optimization level for the Julia LLVM compiler. The default is `3` corresponding to `-O3` which is the default for the Julia REPL. Higher levels take longer to compile but produce faster code.

---

**Enable Powershell Wrapper** (Windows only): Use a Powershell wrapper to spawn Julia. This is required in order to allow interrupts for in-editor evaluation.

**Notifications**: Enables popup notifications when the evaluation finishes.

**Error Notifications**: When evaluating a script, this will show a popup when errors are encountered instead of only printing the error to the console.

**Enable Menu**: Enables the Julia menu in the menu bar. This option requires a restart of Atom for the change to take effect.

**Enable Tool Bar**: Shows the Julia icons in the tool bar. This option requires a restart of Atom for the change to take effect.

**Maximum Console Size**: Limits the number of displayed lines in the Console (default: 10,000). A larger value will display more entries at the cost of slowing down Atom.

**Shell**: Sets the shell used for spawning a new terminal via `Julia Client: New Terminal`.

**Terminal**: The command which is used to open a new REPL.

**Result Display Mode**: Determines where the result of an inline evaluation is displayed:
  - **Float results next to code**
  - **Display results under code**
  - **Display results in the console**
