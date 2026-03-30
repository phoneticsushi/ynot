# ynot: bash aliases but more so

Run scripts without breaking your flow - without worrying about where you put them.

## Y?
- make and edit scripts at light speed
- build a library of aliases to invoke common scripts
- consolidate your workflows

## Ynot?
- idk you tell me

## Installation

```bash
bash <( curl -sSf https://raw.githubusercontent.com/phoneticsushi/ynot/refs/heads/main/helpers/install-ynot )
```
...and follow the prompts

## Quickstart
```bash
ynot list
```

then:
```bash
ynot mod demo
# edit the file as you see fit ...
ynot demo
# you get the idea...
```

or:
```bash
echo "echo Hello, World!" > say-hello
chmod +x say-hello
ynot ingest say-hello
ynot say-hello
```

## Updating
```bash
ynot update
```

## Requirements
- `bash` shell (for provided commands; yours can invoke any shell you want)
- `git` (for self-update and history)
- `flock` (apparently macOS doesn't ship with this; go figure)
- GNU coreutils

## Tips
- You're not limited to bash scripts; you can use any executable file
- `#!/usr/bin/env python` is a fun shebang if you're into that sort of thing
- `ynot` try invoking `ynot` within a `ynot` command script and see what happens?

## FAQ

What was the inspiration?
- 80% practicality, 15% Makefiles, 5% sideways glance at `ujust`

So it's like Makefiles but not scoped to a project?
- no

So it's like `ujust` but worse?
- no

Why would anybody use this?
- `ynot` ?
