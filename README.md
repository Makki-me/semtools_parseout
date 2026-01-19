# parseout

A simple wrapper for [semtools](https://github.com/run-llama/semtools) `parse` that copies parsed markdown files to a specified output directory.

## Install

```bash
mkdir -p ~/.local/bin
curl -fsSL https://raw.githubusercontent.com/jerryjliu/semtools_parseout/main/parseout -o ~/.local/bin/parseout
chmod +x ~/.local/bin/parseout
```

Make sure `~/.local/bin` is on your PATH:

```bash
echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.zshrc  # or ~/.bashrc
source ~/.zshrc
```

## Usage

```bash
parseout <out_dir> <files...>
```

## Examples

```bash
# Parse a single PDF
parseout ./parsed document.pdf

# Parse multiple PDFs
parseout ./parsed scotus_118/*.pdf
```

## How it works

`parseout` calls `parse` under the hood, which outputs parsed markdown files to `~/.parse/`. This wrapper copies those files to your specified output directory.

## Requirements

- [semtools](https://github.com/run-llama/semtools) installed with `parse` command available
