# CSS filter: blur() issue with background-image using data URI

This repository demonstrates a bug where the CSS `filter: blur()` property doesn't work as expected when applied to an element with a background-image that uses a data URI.  The expected behavior is a blurred background image. The actual behavior is either no blur or a partially applied, unexpected blur.

## Steps to Reproduce

1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe the unexpected blurring (or lack thereof) of the background image.
4. Compare with the corrected behavior in `bugSolution.html`

## Possible Causes and Solutions

The exact cause is unclear and might be related to how browsers handle data URIs in conjunction with the `filter` property.  The solution shown in `bugSolution.css` involves using a different approach to achieve the blurred effect, possibly by using a separate element for the image and applying the blur to that.

## Contributing

Contributions to identify the root cause or provide improved solutions are welcome.