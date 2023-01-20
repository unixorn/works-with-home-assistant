# Contributing

First and foremost, thanks for the help. I appreciate all contributions, and the list wouldn't be nearly as complete without them. You may add to the list by submitting a pull request or creating an issue with a link.

You can add entries for things that _don't_ work - just be clear why they didn't work in the notes. We want to warn fellow users off before they waste money buying something they'll end up wanting to e-waste.

## Entry Guidelines

### General

- Entries should be clear, concise, and non-promotional.
- Please only make entries for devices you have _personally_ used. You can't say something works well if you haven't worked with it yourself.
- Please include a link to purchase each addition to the list, but don't include referral codes in the links.
- Amazon links should be in the form https://amazon.com/gp/product/XYZZY/
- If the item needs to be reflashed with Tasmota, ESPHome or something else before it is usable with Home Assistant, make sure to put that in the **Notes** column.
- If the device you're adding won't work in a local-only mode, please say so in the **Notes** column of your entry.
- If it requires a remote service, definitely note that - A lot of people prefer to not buy anything that will brick if the vendor goes out of business or decides to cancel the product line.
- If it tries to phone home - note that too.
- For consistency in entries, please capitalize `Tasmota` and `ESPHome`.
- For consistency, please spell `Z-Wave` with a dash instead of `ZWave` and always spell `Zigbee` and `Z-Wave` with a capital `Z`.
- The list is split into sections for Hubs, Wifi devices, Tools and Utilities, Z-Wave devices and Zigbee devices. Please keep the sections sorted alphabetically.
- Descriptions should follow the link, on the same line, as a markdown table row with capitalization consistent with the other entries in the document. If you're unsure how to format markdown rows, ~steal~ copy another line and then edit the individual columns in your copy, or add a comment to your PR, I'm happy to help.
- Paragraphs in the **Description** and **Notes** columns should be single lines with no internal line breaks. Let GitHub's markdown formatter handle adding any required line breaks rather than embedding breaks inside paragraphs within entries, this makes the list look good with any browser window width.
- Your PR should pass the GitHub automatic check actions. If the checks show an error that you didn't make (a previous entry has gone `404`, for example) while you don't _have_ to fix those errors, I'll certainly appreciate the help if you do, or if you create an issue documenting the problem so I can fix it later.

## To remove an entry:

Open an issue to discuss why the entry should be removed, or create a PR.

Entries that have gone `404` do not require an issue to remove - just make a PR and note that the link is dead.

Discontinued products should get a note added that they're discontinued, but we should keep the entry since existing devices still work.
