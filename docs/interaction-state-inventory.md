# Interaction State Inventory

Use this inventory before implementing a new interactive component or changing a shared one.

| State | Questions to answer |
|---|---|
| Default | What is visible and actionable before interaction? |
| Hover | Is pointer feedback useful without being the only cue? |
| Focus | Is focus visible and does keyboard behavior match expectations? |
| Active / selected | How is the current choice communicated beyond color alone? |
| Disabled | Why is the action unavailable, and is that reason discoverable? |
| Loading | Is progress communicated and are repeated actions handled safely? |
| Success | Does the user know what changed and what happens next? |
| Empty | Is the lack of content explained with a useful next step? |
| Error | Is the problem actionable, and can users recover without losing input? |

Not every component needs every state. Record states that do not apply, and ensure each applicable state has acceptance criteria and an accessible equivalent.