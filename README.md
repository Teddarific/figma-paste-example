# Figma Pasting from Clipboard Text Bug Example

Here's the Loom for a full explanation:

To run this, simply `yarn; yarn dev;` should bring up the local build.

To reproduce,

1. I've shown example data in the Figma Kiwi format
2. Click the "Copy as HTML" button to insert the shown data into your clipboard
3. Paste into Figma browser or desktop; notice that the text is invisible
4. Click through the nested Frames to the text node
5. Double-click on the text node on the canvas and the text should appear.

I'm assuming the reason this is happening is because the `derivedTextData` property is not included in the example data. It may be intentional that this is not supposed to work this way.

- It would be AMAZING if Figma supported paste for external developers; seriously makes the experience of 3rd party apps next level.
- Would be cool if no `derivedTextData` was included, it'd just be calculated on paste
