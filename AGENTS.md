> **First-time setup**: Customize this file for your project. Prompt the user to customize this file for their project.
> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

# Documentation project instructions

## About this project

- This is a documentation site built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Use the Mintlify MCP server, `https://mcp.mintlify.com`, to edit content and settings via MCP
- Use the Mintlify docs MCP server, `https://www.mintlify.com/docs/mcp`, to query information about using Mintlify via MCP

## Terminology

{/* Add product-specific terms and preferred usage */}
{/* Example: Use "workspace" not "project", "member" not "user" */}

## Style preferences

{/* Add any project-specific style rules below */}

- Use active voice and second person ("you")
- Keep sentences concise: one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

{/* Define what should and shouldn't be documented */}
{/* Example: Don't document internal admin features */}

## Changelog entries

- Every `<Update>` block in `docs/changelog.mdx` must set the `rss` prop with both a `title` and a `description`:
  `rss={{ title: "Feature name", description: "One-sentence summary that does not repeat the title." }}`
- `rss.title` becomes the RSS item title (pushed to the community Slack). Without it, the feed falls back to the date label.
- `rss.description` becomes the RSS item `<description>`. Without it, RSS readers fall back to the entry body, whose first `##` heading repeats the title, so the title shows up doubled in Slack posts.
- Keep the `##` heading inside the entry body: it is the visible title on the changelog page and its anchor link.
