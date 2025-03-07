# Buttons

Buttons are essential to enable users to perform actions. Buttons should be used for action items such as Create, Save, Delete, and should not be used for navigational elements. Instead, use links to take the user to a new page.

## Types of Buttons

There are several types of buttons to choose from based on the intended action:

| Type            | Purpose                                                                         |
| --------------- | ------------------------------------------------------------------------------- |
| Primary         | Used for the most important call-to-action on a page, such as Save or Deploy.   |
| Secondary       | Used primarily for a call-to-action that is a link.                             |
| Warning         | Used to advise caution.                                                         |
| Danger          | Used to highlight something dangerous that can't be undone, such as "Delete".   |
| Icon only       | Use when an icon is enough to represent the action, such as "Create a Service". |
| Icon with label | Use when an icon by itself is not obvious enough, such as "Kill Task".          |

## Button States

Buttons can have different states depending on their availability and whether an action is being processed:

| State      | Purpose                                                                                                                                          |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| Disabled   | Disable a button when the action is not applicable but we want to show the user that it may be possible. Disabled buttons should have a tooltip. |
| Processing | When a user clicks or taps a button and an API request is initiated, provide feedback so they know their action was received.                    |
| Hidden     | Hide a button when there is no way a user can interact with the button.                                                                          |

## Using Buttons as Links

Sometimes there is a button that is actually a link to somewhere else. If the appropriate props are set, the button is rendered as an anchor tag, but it is styled like a button.

It is not recommended to use a button as a link when it triggers a dropdown. It would be frustrating if a user clicked a button and expected to see a dropdown appear, but they are taken to a new page.

## Button Content

Button labels should be concise and descriptive, tell users what will happen when they click the button.

Examples of acceptable labels:

- New {Item}
- Create {Item}
- Edit {Item}
- Save {Item}
- Delete {Item}
- Deploy {Item}
- Scale {Item}
- Restart {Item}

Use sentence-style capitalization (only the first word in a phrase and any proper nouns capitalized). Include no more than three words for button labels.

For sets of buttons, use descriptive action words in labels. For example, use Save or Cancel instead of Yes and No. This is particularly helpful when the user is confirming an action.

## ResetButton

A `ResetButton` component is essentially an unstyled HTML `<button>` element. It can be used for an element that is semantically a button, but is not intended to look like a button.

## Feedback

Buttons should have hover, active, focus, disabled states. When a user interacts with a button, either via click or tap, and an action is being completed, e.g. an API call, the button should change to disabled and provide feedback via the label to the user that it received the interaction and is busy performing the action e.g. “Saving…”.

## Tooltips

Buttons may or may not require tooltips to help communicate their intent. Icon buttons that do not have labels should always have a tooltip so the user knows what will happen when they click it. Disabled buttons should always have a tooltip to explain why it is disabled so the user is aware.
