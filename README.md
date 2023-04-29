# cc
Copy the contents of a file with a single command, `cc`.

## Installation

Linux:
```bash
cc() { cat "$1" | xclip -selection clipboard; }
```

macOS
```bash
cc() { cat "$1" | pbcopy; }
```

windows
```bash
cc() { type "$1" | clip; }
```

## Usage

```bash
cc <file-name>
```

## About
This is built with the help of ChatGPT.

- Prompt:
is there a command to copy the contents of a file in the terminal?

- ChatGPT:
Yes, you can copy the contents of a file in the terminal using a variety of commands depending on your operating system.

For Linux and macOS, you can use the cat and cp commands.

To copy the contents of a file to the clipboard, you can use:

1. cat command with xclip (for Linux)

```bash
cat file.txt | xclip -selection clipboard
```

2. cat command with pbcopy (for macOS)

```bash
cat file.txt | pbcopy
```

If you want to copy the contents of a file to another file, you can use the cp command:

```bash
cp source_file.txt destination_file.txt
```

For Windows, you can use the type and clip commands.

To copy the contents of a file to the clipboard, use:

```bash
type file.txt | clip
```

To copy the contents of a file to another file, you can use the copy command:

```bash
copy source_file.txt destination_file.txt
```

Please note that these commands may overwrite the contents of the destination file.
