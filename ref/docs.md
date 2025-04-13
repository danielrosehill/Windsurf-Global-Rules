13-05-2025

 ## [​](https://docs.windsurf.com/windsurf/memories\#windsurfrules)  .windsurfrules

Users can explicitly define their own rules for Cascade to follow. Cascade will be aware of your rules at all times, even if you change them in the middle of your conversation, and will try its best to follow them.

Rules are defined in designated files:

`global_rules.md` \- rules applied across all workspaces

`.windsurfrules` \- rules for the local workspace that the `.windsurfrules` file is in

To ensure that the rules are only applied to your local project, add `.windsurfrules` to your project’s `.gitignore`.

You can find example rule templates curated by the Windsurf team at [https://codeium.com/windsurf/directory](https://codeium.com/windsurf/directory) to help you get started.

Edit these rules files by clicking on the Windsurf - Settings menu, select the “Settings” tab, and clicking “Edit Rules” next to either `Set Global AI Rules` or `Set Workspace AI Rules`.

`global_rules.md` and `.windsurfrules` are limited to 6000 characters each. Any content above 6000 characters will be truncated and Cascade will not be aware of them.

If your window has multiple workspaces, the `.windsurfrules` from each workspace will be applied. 

If the total of your global rules and local rules exceed 12,000 characters, priority will be given to the global rules, followed by the workspace rules. Any rules beyond 12,000 characters will be truncated.

### [​](https://docs.windsurf.com/windsurf/memories\#best-practices)  Best Practices

To help Cascade follow your rules effectively, follow these best practices:

- Keep rules simple, concise, and specific. Rules that are too long or vague may confuse Cascade.
- There’s no need to add generic rules (e.g. “write good code”), as these are already baked into Cascade’s training data.
- Format your rules using bullet points, numbered lists, and markdown. These are easier for Cascade to follow compared to a long paragraph. For example:

Copy

```
# Coding Guidelines
- My project's programming language is python
- Use early returns when possible
- Always add documentation when creating new functions and classes

```

- XML tags can be an effective way to communicate and group similar rules together. For example:

Copy

```
<coding_guidelines>
- My project's programming language is python
- Use early returns when possible
- Always add documentation when creating new functions and classes
</coding_guidelines>

```
 