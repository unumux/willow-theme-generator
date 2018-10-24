# Example Output from Theme Generator

This is a mock up of folders and files that could be provided by a Willow theme generator.

This work could be divided into 2 releases (or more), here are some initial thoughts on how it would be divided.

- Release One:
  - delivers the theme folder and all of its contents
  - scss partials contain variables with no set value (or should it be set to whatever value it is set to in Willow?)
    - the variables should have the `!default` flag
  - Note: the constants/_typography.scss partial requires the line-height and strip-unit functions. those are imported in the willow instance but here I pasted the code at the top of the file for ease rn.  In the future you may want to consider what mixins, functions, classes, animations, etc should come with this kit for a dev to take advantage of.
  - Note: the constants/_spacing.scss partial also has function dependents. I handle this the same as how typography was handled (see the above note).

- Release Two:
  - delivers the overrides folder and all of its contents
  - thing to consider for the scss partials - how do you construct the selectors in these? For example how do you remove the rulesets but leave the sub-element imports and the media queries.