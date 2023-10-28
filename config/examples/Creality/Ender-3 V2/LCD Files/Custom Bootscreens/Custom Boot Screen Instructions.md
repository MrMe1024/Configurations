# Making a Custom Boot Screen

To make a custom boot screen for non stock Marlin UIs like Jyers UI or Pro UI or Creality UI there are 5 requirements for printers with a DWIN or DICAI Display Like those commonly found on the Ender 3v2, Ender-3 V2 Neo, Ender-3 Max Neo, and Ender-3 S1:

1. The file format must be JPG. (this is not the same as JPEG)
2. Progressive must be tuned off in the export settings (under "Advanced" in GIMP).
3. The Sub-sampling format must be chroma quartered (4:2:0) (also under "Advanced" in GIMP).
4. The resolution must be 480x272.
   Note: The left side of the image will be the top. You can compose the image oriented upright as 272x480, but it must be
   rotated prior to export. (Rotating during or after export only applies a "rotation" attribute that won't be parsed by DWIN / DACAI.)
5. For DACAI the file must be named "`0`" and placed in `private/image`. For DWIN the file must be named "`0_start`" and placed in `DWIN_SET`.

After replacing the Boot Screen follow the usual screen flashing instructions.

If you are tying to make a custom Boot screen for different displays or the Portrait/Landscape Marlin UI or follow the regular custom boot screen Instructions.
