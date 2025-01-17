# Text-to-Adversarial
## Proposal
Given a desired text to encrypt, is it possible to generate a system that can both encode text into an image and decode the text from the image? Moreover, is it possible for the text to serve as adversarial noise targeting a specific class?

## TODOS:
1. Implement encoder. Pipeline idea: Text -> Text encoder -> Zero-Padding -> Zero-Padded Text encoding + Image
2. Decoding in-progress brainstorming.
   * ~~How will we unnormalize the data when decoding?~~ <- for now, we will multiply the data by the maximum pixel value (255) and total image dimension (width * height). Not generalized and this leads to the dependency between the data and the image size, which can be an issue.
   * How can our algorithm recognize encoded text? Is there a way of finding it while decoding?
3. How would we deal with the conversion from uint8 to float? The values have been scaled down to floats...
