# nodupe


A simple tool to append unique lines to a file.


---

### Overview

nodupe is a command-line utility designed to append unique lines from stdin to a specified file. It ensures that no duplicates are added, making it a valuable tool for deduplication in various workflows.


---

### Features

Appends new, unique lines to a file.

Prevents duplicate entries by checking against the existing contents of the file.

Lightweight and easy to use.

Works seamlessly in Unix-like environments and integrates well with other tools.



---

### Installation

Using go install

To install nodupe, ensure you have Go installed and run:

```go install github.com/Karthik-HR0/nodupe@latest```

This will download and build the anew binary, placing it in your $GOPATH/bin.


---

### Usage

Basic Syntax:

cat input.txt | nodupe [output-file]

### Examples:

1. Append unique lines from a file:

```cat urls.txt | anew unique-urls.txt```


2. Use with other tools in a pipeline:

echo "example.com" | grep ".com" | anew domains.txt


3. Combine with sort to maintain sorted output:

sort new-data.txt | anew sorted-unique-data.txt




---

How It Works

anew checks each incoming line against the contents of the specified file. If the line doesn't already exist, it is appended to the file. This ensures that the output file only contains unique entries.


---

Why Use anew?

Simplifies deduplication in workflows.

Reduces redundant processing for repetitive data.

Integrates well with standard command-line tools.



---

License

anew is open-source and available under the MIT License. Feel free to use, modify, and distribute it as needed.


---

Contributing

Contributions are welcome! Feel free to submit issues or pull requests on the GitHub repository.


---

Acknowledgments

Developed by tomnomnom, a well-known contributor in the infosec and command-line tools community.


---

Enjoy deduplication made easy with anew!

