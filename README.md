# ynot: bash aliases but more so

Run scripts without breaking your flow - without worrying about where you put them.

## Y?
- make and edit scripts at light speed
- build a library of aliases to invoke common scripts
- consolidate your workflows

## Ynot?
- idk you tell me

## Installation

Acquire code:
```bash
git clone git@github.com:phoneticsushi/ynot ~/.ynot
```

...or wherever you want it, then add to path, e.g.
```bash
echo '
# use ynot for aliases but more so
if [ -d "$HOME/.ynot" ] ; then
    export PATH="$HOME/.ynot:$PATH"
fi' >> ~/.bashrc
```

Optional: configure desired text editor(s) if you haven't already, e.g.
```bash
echo '
# default text editors
export EDITOR=nvim
export VISUAL=codium
' >> ~/.bashrc

```

Open new terminal or load changes:
```bash
source ~/.bashrc
```

(more automated installation coming in the future hopefully)

## Quickstart
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
cd ~/.ynot
git pull
```

## Requirements
- `bash` shell
- GNU coreutils

## Tips
- You're not limited to bash scripts; you can use any executable file
- `#!/usr/bin/env python` is a fun shebang if you're into that sort of thing
- `ynot` try invoking `ynot` within a `ynot` command script and see what happens?

## FAQ

What was the inspiration?
- 60% practicality, 30% Makefiles, 10% sideways glance at `ujust`

So it's like Makefiles but not scoped to a project?
- no

So it's like `ujust` but worse?
- no

Why would anybody use this?
- `ynot` ?
