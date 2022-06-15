# icc-profiles

ICC profiles for many of my computers' displays.

These profiles also include calibration info. That is, they contain gamma ramps
for the VCGLUT (Video Card Gamma Lookup Table).

They might be good for your systems - and they might not be.

### Notes on the 'saturation' intent

All of the profiles currently on here are set up so that the 'saturation'
intent is actually a 'luminance preserving perceptual' intent (in the words of
Argyll's documentation for `collink` at
http://argyllcms.com/doc/collink.html#i ; see the `lp` intent for details.

For devices with a gamut smaller than sRGB being mapped into sRGB, this can do
a nice job of preserving details while still providing better colors than
uncorrected; the human eye is more sensitive to luminance changes than to
chromatic changes.

I have occasionally noticed some shades of blue turning purple with this
intent, but that seems to happen with all perceptual intents due to the
way that the matrix transformation is done.
