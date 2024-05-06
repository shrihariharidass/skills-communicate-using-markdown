# This README.md file demonstrates the regular expression (?<!#)#{1,6}([ \t](.*))?$

This file showcases the usage of a regular expression to match heading levels (h1-h6) in Markdown documents.

**Explanation of the Regex:**

- `(?<!#)`: This negative lookbehind assertion ensures the match doesn't start immediately after a hash (#) symbol, preventing accidental matching of inline code blocks.
- `#{1,6}`: This matches one to six hash symbols (#), representing heading levels h1 to h6.
- `[ \t]`: This matches either a space or a tab character, allowing for optional whitespace after the heading level indicator.
- `(.*)`: This captures any characters following the heading level and whitespace, representing the heading content.
- `$`: This matches the end of the line, ensuring the entire heading is captured.

**Example Usage in index.md:**

This regular expression can be used in various tools to extract heading information from Markdown files. Here's an example usage in the `index.md` file:

```markdown
# This is an h1 heading
This is some content within the h1 heading.

## This is an h2 heading
This is some content within the h2 heading.

### This is an h3 heading
This is some content within the h3 heading.
