# Text-to-Adversarial
## Proposal
Given a desired text to encrypt, is it possible to generate a system that can both encode text into an image and decode the text from the image? Moreover, is it possible for the text to serve as adversarial noise targeting a specific class?

## TODOS:
1. Implement encoder. Pipeline idea: Text -> Text encoder -> Zero-Padding -> Zero-Padded Text encoding + Image
2. Decoding in-progress brainstorming
     2.1. How will we unnormalize the data when decoding?
