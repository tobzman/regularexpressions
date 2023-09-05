# regularexpressions

# Exploring Regular Expressions: Matching URLs

## Introduction

Regular expressions (regex) are powerful tools used in programming to define search patterns within strings. In this tutorial, we will break down and explain each part of the regex used for matching URLs.

## Summary

The regular expression `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/` is designed to match URLs, including both HTTP and HTTPS protocols. It consists of several components that capture different parts of a URL, such as the protocol, domain, path, and more.

## Components of the Regex

### Protocol

The protocol component `(https?:\/\/)?` is optional and allows for both HTTP and HTTPS. The `https?` part matches either 'http' or 'https', while the `\/\/` matches the two forward slashes after the protocol in a URL.

### Domain

The domain component `([\da-z\.-]+)` matches the subdomain and domain name. The `[\da-z\.-]+` part matches one or more alphanumeric characters, dots, and hyphens, allowing for a variety of domain names and subdomains.

### Top-Level Domain

The top-level domain (TLD) component `\.([a-z\.]{2,6})` captures the domain extension. The `\.([a-z\.]{2,6})` part matches a dot followed by 2 to 6 lowercase letters, covering a range of TLDs like .com, .org, .io, and more.

### Path

The path component `([\/\w \.-]*)*\/?` deals with the URL path. The `([\/\w \.-]*)*` part matches zero or more occurrences of forward slashes, alphanumeric characters, spaces, dots, and hyphens, allowing for flexibility in the path structure. The `\/?` at the end makes the trailing slash optional.

## Examples

Let's explore some examples to understand how the regex works:

- `https://www.example.com`: Matches a URL with HTTPS protocol, 'www' subdomain, and '.com' TLD.
- `http://sub.example.org/path`: Matches a URL with HTTP protocol, 'sub' subdomain, '.org' TLD, and '/path' path.
- `ftp://ftp.example.net`: Does not match since the regex expects HTTP or HTTPS protocols.
- `https://sub.example.longtld`: Does not match due to the missing TLD characters.

## About the Author

As a web development enthusiast, I'm passionate about sharing knowledge and helping others learn. Feel free to connect with me on GitHub for more tutorials and projects!

---

You can copy and paste this content into a Markdown file for your project.

**Step 3: Create a GitHub Gist**

Now, you'll create a GitHub Gist to host your tutorial content:

- Log in to your GitHub account or create one if you don't have an account.
- Click on the "Gist" option in the top-right corner (it looks like a little notepad icon).
- In the Gist creation form, paste your tutorial content into the text area.
- Give your Gist a name, like "regex-tutorial.md".
- Ensure the Gist is set to "Public."
- Click the "Create public gist" button.

**Step 4: Submission**

You will need to provide the URL of your GitHub Gist as part of your assignment submission.

That's it! Your tutorial project on regular expressions is now hosted on GitHub Gists, and you can share the Gist URL as your assignment submission.
