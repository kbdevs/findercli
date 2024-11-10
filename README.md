### 1. Create the Shell Script
Create a new file called `finder` (or `fn` if you prefer that as the command name) in a directory like `/usr/local/bin/`.

```bash
#!/bin/bash
# Open Finder to the current working directory
open .
```

This script uses the `open` command, which is a built-in macOS command to open files, folders, and applications. The `.` means it will open the current directory in Finder.

### 2. Make the Script Executable
Give the script executable permissions by running the following command in the terminal:

```bash
chmod +x /usr/local/bin/finder
```

If you created the script with the `fn` name, replace `finder` with `fn` in the path above.

### 3. Add the Script to Your PATH (if needed)
If `/usr/local/bin` is already in your PATH, you can skip this step. If it’s not, add it by appending this line to your `.zshrc` or `.bash_profile`, depending on your shell:

```bash
export PATH="/usr/local/bin:$PATH"
```

Then, reload your shell configuration:

```bash
source ~/.zshrc  # or source ~/.bash_profile
```

### 4. Test the Command
Navigate to any directory in your terminal, then run:

```bash
finder
```

or

```bash
fn
```
