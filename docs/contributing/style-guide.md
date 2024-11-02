# Documentation style guide

To make the documentation consistent and accessible, you should try to align your content with the following style standards.

Best effort is much more important than perfection. Follow the style guide as best you can and allow others to edit your content to bring it in line with the style standards.

## Content structure

Content is organized by:

* Tabs
* Pages
* Sections

The tabs and left navigation are defined in `mkdocs.yaml`, and populated by individual `.md` files.
The right table of contents (ToC) for a page is defined by the sections (`##` and below) within the file.

### File naming conventions

Use lowercase, hyphenated names for all Markdown files, such as `getting-started.md`. Use consise and descriptive names. The file name should match the H1 heading for the page, but it's okay to use abbreviations.

For example:
```
contributing-to-the-docs.md
# Contributing to the documentation
```

### Page structure

Pages should follow this structure:

```
# Topic name

Author: Your Name (Optional)

1-2 paragraph introduction for context.

## Section

### Sub-section

```

#### Headings

- Start each document with a H1 title (`# Title`).
- Use H2 (`##`) for primary sections, H3 (`###`) for subsections, and so on.
- Avoid skipping header levels.
- Include a blank line under headings for readability in the source Markdown.
- Use sentence case (that is, capitalize only the first letter) for headings, such as `## Installation guide`.

### Writing Style

These style guidelines help make the documentation accessible to people from various language backgrounds and abilities.

- Tone: Use a clear, friendly, and professional tone.
- Voice: Prefer the active voice (e.g., “Install the package” rather than “The package is installed”).
- Pronouns: Address the reader as “you” when giving instructions.
- Tense: Use present tense where possible (e.g., “This command installs…”).
- Clarity: Aim for concise, plain language. Avoid jargon, idioms, and complex sentences.


### Lists

- Bulleted Lists: Use for lists where the order doesn't matter. For consistency, use `-` instead of `*`.
- Numbered Lists: Use for lists where the ordered matters. If there is only one ordered step in a section, use `-`.
- Keep list items parallel in structure (e.g., start each item with a verb or noun for consistency).

### Links
- Use descriptive text for links.
    - Prefer: "For more information, see the [GitHub Markdown Guide](https://example.com)"
    - Avoid: "For more information, [click here](https://example.com)"
- Use inline links where possible, but reference links are okay if they improve readability.

### Images

Place images in a designated assets or images folder and link relative paths, such as `![Diagram](assets/diagram.png)`.
Add descriptive alt text for accessibility.
Use PNG for diagrams and SVG for vector images when possible.

### Tables

Use tables sparingly and only for structured data that’s difficult to read in list format.
Keep tables simple, avoiding excessive width.

### Examples
- Use "such as" or "for example" (instead of "e.g.")
    - Prefer: "For more information, see the [GitHub Markdown Guide](https://example.com)"
    - Avoid: "For more information, [click here](https://example.com)"
- Use "that is" instead of "i.e."
- Use "and similar" instead of "etc."