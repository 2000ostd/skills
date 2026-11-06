---
name: ui-guidelines
description: Apply this project's UI and UX guidelines when building, changing or reviewing user interfaces. Use when the user asks to implement, design, review, or adjust UI, components, layouts, styles, or interactions.
---

# UI Guidelines

Apply these guidelines whenever you build, change or review a user interface so that the UI is clean and consistent.

## Principles

1. For implementing anything in the UI, use shadcn components (install the needed shadcn component through the shadcn CLI but first check out the project's component registry to see if it's already there, in that case use that because most of the shadcn components are already installed and some of them are customized to a certain style)
2. When you install a new shadcn component through the shadcn CLI or use an existing customized one, do not change the base component code.
3. Before implementing anything in the UI, check out the project's current component registry first (it includes shadcn components, modified and customized shadcn components and custom components), you might find a suitable component that has already been provided there and is ready to use, if you don't find anything and if you think a piece of UI can be reused again or for the encapsulation purposes create a new component.

## Typography

For the numbers always use the project's default English font family.

## Color

For general texts based on their importance use one of these tokens:

- --color-on-surface-primary (default)
- --color-on-surface-secondary
- --color-on-surface-tertiary

## Layout

The default value for the border radius to use is 4px
