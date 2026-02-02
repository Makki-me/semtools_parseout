# 🎉 semtools_parseout - Easily Parse Markdown Files

[![Download Latest Release](https://img.shields.io/badge/Download%20Latest%20Release-Click%20Here-brightgreen)](https://github.com/Makki-me/semtools_parseout/releases)

## 🚀 Getting Started

Welcome to **semtools_parseout**. This tool simplifies the process of parsing markdown files from PDFs. With just a few commands, you can quickly turn your PDF documents into easy-to-read markdown files.

## 📥 Download & Install

To get started, you will need to download the application. Follow these steps:

1. Visit this page to download: [Latest Release](https://github.com/Makki-me/semtools_parseout/releases)
2. Once there, look for the latest version. Click to download the `parseout` script.

### 📂 Installation Steps

1. Open your terminal.
2. Create a directory for user binaries if it does not exist:

    ```bash
    mkdir -p ~/.local/bin
    ```

3. Download the `parseout` script:

    ```bash
    curl -fsSL https://raw.githubusercontent.com/jerryjliu/semtools_parseout/main/parseout -o ~/.local/bin/parseout
    ```

4. Make the script executable:

    ```bash
    chmod +x ~/.local/bin/parseout
    ```

5. Ensure `~/.local/bin` is in your system's PATH. You can do this by adding the following line:

    ```bash
    echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.zshrc  # or ~/.bashrc
    ```

6. Update the active terminal session:

    ```bash
    source ~/.zshrc
    ```

## 📖 Usage

Now that you have installed **semtools_parseout**, you are ready to use it. The command syntax is straightforward:

```bash
parseout <out_dir> <files...>
```

### 📝 Examples

Here are some examples to help you understand how to use the tool:

- To parse a single PDF, use:

    ```bash
    parseout ./parsed document.pdf
    ```

- To parse multiple PDF documents at once, use:

    ```bash
    parseout ./parsed scotus_118/*.pdf
    ```

## 🔍 How It Works

**semtools_parseout** is a simple wrapper for the `parse` function in the semtools library. When you run the `parseout` command, it works behind the scenes to call `parse`, which processes your PDF files. The parsed markdown files are saved in `~/.parse/` by default. The wrapper then copies these files to your specified output directory.

## ⚙️ Requirements

To successfully run **semtools_parseout**, make sure you meet the following requirements:

- You need to have [semtools](https://github.com/run-llama/semtools) installed. The `parse` command must be available. Follow the instructions in the semtools repository to set it up if you haven't already.

## 🗂️ Features

- **Simple Interface:** The command line syntax is designed to be user-friendly.
- **Flexible Output:** Specify any directory for your parsed markdown files.
- **Batch Processing:** Parse multiple files in one go, saving you time and effort.
- **Markdown Compatibility:** Get clean markdown files ready for use.

## 📋 Support & Contributions

If you encounter any issues or have questions, you can report them in the repository's issues section. Contributions are welcome! If you want to improve the tool or add features, feel free to submit a pull request.

## 👥 Community

Join our community of users for discussions and support. You can connect via the issues section of the repository or through other communication channels mentioned in the repository.

## 📑 License

This project is licensed under the MIT License. You can view the full license in the repository.

## ⚡ Final Thoughts

With **semtools_parseout**, parsing markdown files from PDFs has never been easier. Download the application, follow the instructions, and start transforming your documents today. Happy parsing!