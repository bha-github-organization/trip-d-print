[Face Shield](#3d-printed-face-shields), [Face Mask Holder](#3d-printed-face-mask-holder) 
=========================

This site provides information on how to 3D print various COVID-19 related protective items.
The goal is to use the simplest design that will work, and is relatively fast and easy to build.

Please share your own experiences and suggestions for improvement. 

This is an Open Source project (shared under [Apache License, v2](LICENSE.txt)), so use what 
you find here as you see fit, but please do take the time to improve this site by creating 
[Issues](https://github.com/bha-github-organization/trip-d-print/issues) or better yet: [Pull Requests](https://github.com/bha-github-organization/trip-d-print/pulls). 

---------

3D Printed Face Shields
-----------------------

I’ve been working with local nurses who are helping people at Capital Health (Pennington, NJ) and at the Mercer County Covid-19
Testing center. They’ve been using 3D printed face shields that are very simple to print and assemble.
I’m asking for anyone nearby with a 3D printer who would like to volunteer to please help in this effort 
by printing the face shield frame, and maybe even assembling the transparency too. 

Here's how the Face Shields look in action:

![nurses-with-shields](images/3Nurses-FaceShield.png)

We tried a number of different designs, and this one was the best balance of functionality and ease of production.

I’m using the `US Three Hole Punch` style (mostly because I own a 3 hole punch).

There is a "nested" .stl file that prints 2 frames at once. The most updated design (version 4) prints faster and is
easier to remove from the platter when the print is complete. We've tested the files below:

  | File | Items Per Print | Print Time |
  |------|-----------------|------------|
  | [US Three Hole Punch (version 4)](stl/face-shield/3-hole/version-4/Visor_Frame_NORTH_AMERICA_letter_3-hole_v4.stl) | 1 |  |
  | [~~US Three Hole Punch (version 3-obsolete)~~](stl/face-shield/3-hole/version-2/Visor_Frame_NORTH_AMERICA_LETTER_v2.stl) | 1 | Prusa MK3: 1 hour, 34 minutes |
  | [US Three Hole Punch x 2 (version 4)](stl/face-shield/3-hole/version-4/2-Visor_Frame_NORTH_AMERICA_letter_3-hole_v4.stl) | 2 | Prusa MK3: 2 hours, 43 minutes |
  | [~~US Three Hole Punch x 2 (version 3-obsolete)~~](stl/face-shield/3-hole/version-2/Nst2Visor_Frame_NORTH_AMERICA_LETTER_v2-nested.stl) | 2 | Prusa MK3: 3 hours, 4 minutes<br>Lulzbot: 1 hour, 53 minutes |
  | [~~Big Plate US Three Hole Punch X 2 (version 3-obsolete)~~](stl/face-shield/3-hole/version-2/Lulzbot_Taz6_2FaceShields.stl) | 2 | Lulzbot: 2 hours, 10 minutes |

If you prefer a 6 hole version, the files are listed below:

  | File | Items Per Print | Print Time |
  |------|-----------------|------------|
  | [US Six Hole Punch (version 5)](stl/face-shield/6-hole/version-5/Visor_Frame_NORTH_AMERICA_letter_6-hole_v5.stl) | 1 |  |
  | [US Six Hole Punch x 2 (version 5)](stl/face-shield/6-hole/version-5/2-Visor_Frame_NORTH_AMERICA_letter_6-hole_v5.stl) | 2 |  |

Original design files are by [Erik Cederberg](https://www.youmagine.com/erikcederb) from here: https://www.youmagine.com/designs/protective-visor-by-3dverkstan

To let you know what to expect, the obsolete version 3 frame takes about 1 hour, 34 minutes to print on my 
[Prusa](https://www.prusa3d.com) MK3 printer.
Whatever filament you have handy is fine. I've been using PETG.

The transparency is a sheet (purchased from Staples):
 
* | [Apollo Write-On Transparency Film](https://www.staples.com/Apollo-Write-On-Transparency-Film-Clear-8-1-2-W-x-11-H-100-Box/product_829333) |
  |----------|
  | WO100C-B |
  | 8.5 x 11 in |
  | Write-On Transparency Film |
  | 100 sheets |

  Please share other sources if you know of any.

#### Learnings


* Mike S is taking this up a notch: He is moving the local High School's printers to the
First Aid squad, where the EMTs will start churning out these face shields. Mike also had a great comment: 
"Have you tried 'nesting' the frames so you can get more than one frame per print?". Doh! Well no, I hadn't.
If anyone can create a nested .stl file, please share it here (if you beat Mike to it)! See: [Issue #1](https://github.com/bha-github-organization/trip-d-print/issues/1)
 
  - @Sulliv26 wins! His nested file is here: [Lulzbot_Taz6_2FaceShields.stl](stl/face-shield/3-hole/version-2/Lulzbot_Taz6_2FaceShields.stl) It 
    has two frames. 
    
  - Another nested file that fits on a smaller plate, like my Prusa MK3: [Nst2Visor_Frame_NORTH_AMERICA_LETTER_v2-nested.stl](stl/face-shield/3-hole/version-2/Nst2Visor_Frame_NORTH_AMERICA_LETTER_v2-nested.stl).
    Print time: Prusa MK3: 3 hours, 4 minutes

* Kasia Q mentioned using UV to sterilize the frames, so they could be reusable!

* To help monitor print job progress, I setup [Octoprint](https://octoprint.org) on a [Raspberryp Pi 4](https://www.raspberrypi.org)
 using [these steps](https://community.octoprint.org/t/setting-up-octoprint-on-a-raspberry-pi-running-raspbian/2337).

* [Ventilator Splitter](http://ventsplitter.org) - Jason S is producing these. I'm trying to gather more info.

* [Various PPE Gear](https://3dprint.nih.gov/collections/covid-19-response) - Matthew B shared this link. These are CDC
  approved designs. I'm going to experiment with the 6 hole design using this tip:
  
    *Set the end stop on the 3 hole punch to 10 inch size (basically, 1/2" away from the normal centered location) 
    then punch once, flip, and punch again to get the right pattern.*
    
    The above trick to use a 3 hole punch to create a 6 hole layout isn't working well for me. No level of hole 
    adjustment nor transparency positioning seems to produce properly aligned holes. 
    It is possible I'm "holding it wrong", but I also suspect my old 3 hole punch maybe be 
    misaligned. I will try a different punch and see how it goes. Meanwhile, I've posted the 6 hole style files if you 
    want to give it a try.
  
---------

3D Printed Face Mask Holder
---------------------------
Nurses have asked for a mask strap holder, to ease ear fatigue. Canadian colleagues recommended the design below. 

Here's how the Mask Holder looks in action:

![nurse-with-holder](images/MaskHolderUsage.png) ![nurse-with-holder-back](images/MaskHolderBack.png)

Thanks to [Nicholas Madori](https://www.thingiverse.com/namadori/about) for sharing this design.
The original design is available here:  [Face mask holder](https://www.thingiverse.com/thing:4218199/files)

The original single buckle file is here: [Face_mask_holder_v1](stl/mask-holder-buckle/Face_mask_holder_v1.stl)

Here's an .stl that fits 7 of these on a Prusa MK3 printer: [7_Face_mask_holder_v1_Prusa](stl/mask-holder-buckle/7_Face_mask_holder_v1_Prusa.stl)

  | File | Items Per Print | Print Time |
  |------|-----------------|------------|
  | [Face_mask_holder_v1](stl/mask-holder-buckle/Face_mask_holder_v1.stl) | 1 | Prusa MK3: 33 minutes |
  | [7_Face_mask_holder_v1_Prusa](stl/mask-holder-buckle/7_Face_mask_holder_v1_Prusa.stl) | 7 | Prusa MK3: 3 hours, 20 minutes |
  | [85p_7_Face_mask_holder_v1_Prusa](stl/mask-holder-buckle/85p_7_Face_mask_holder_v1_Prusa.stl) | 7 | Prusa MK3: 2 hours, 14 minutes |
    
Notice the third file above (with 7 holders) is scaled down to 85% of the original size. We had feedback that the 
full-sized version of the model is too big for many people. Information sharing works!    
    
Thanks for reading this far.
Dan Rollo
