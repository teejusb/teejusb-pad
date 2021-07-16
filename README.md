# Teejusb's Travel Pad
Guide to Build a Travel Pad with FSRs.
 
I had a couple of goals for this project:
1. **Lightweight/Portable**
    - All put together it's a bit over 10 lbs. I carried it around from place to place without issue.
    - It has a 20" x 20" footprint so not too bulky.
2. **Low Cost (Relatively)**
    - Less than $300 (not incl. Laser Cutting). If people have existing tools then this cost goes down quite a bit as well.
3. **Toolless**
    - You don't need any tools to get in and out of the pad once it's put together.
 
 <img src="images/15.JPG" height="400px" /></br><b>Check out pad in action [HERE](http://www.youtube.com/watch?v=_NM0flVgFBk)</a></b>
## Table of Contents
- [Teejusb's Travel Pad](#teejusbs-travel-pad)
  - [Table of Contents](#table-of-contents)
  - [Credits](#credits)
  - [Bill of Materials](#bill-of-materials)
  - [Parts to 3D Print](#parts-to-3d-print)
  - [Steps](#steps)
    - [Cutting the Pieces](#1-cutting-the-pieces)
    - [Before the Build](#2-before-the-build)
    - [Building the Pad](#3-building-the-pad)
  - [Adding LEDs](#4-adding-leds)
## Credits
 - To **dj505** as I used their [build log](https://imgur.com/a/IuHijaS) as the main basis when creating this travel pad.
 - To **4199** as the original design was theirs.

## Bill of Materials

I personally paid about **$300** for everything (incl. Laser Cutting) as I already had access to some existing tools/materials. If you're starting from nothing, refer to the table below for the expected cost of the project.

|   Part           |Price          |
|------------------|---------------|
|[2'x4' 1/2" Plywood](https://www.homedepot.com/p/1-2-in-x-2-ft-x-4-ft-Radiata-Pine-Plywood-Actual-0-469in-x-23-75-in-x-47-75-in-414715/313354418)<sup>1</sup>|$25|
|[3/8" Polycarbonate](https://www.tapplastics.com/product/plastics/cut_to_size_plastic/polycarbonate_sheets/516)|$24 - $56<sup>2</sup>|
|[Teensy 4.0](https://www.pjrc.com/store/teensy40_pins.html) (or equivalent)|$25|
|[4 x FSR 406](https://buyinterlinkelectronics.com/collections/new-standard-force-sensors/products/fsr-model-406?variant=31639756210313)|$30|
|[Wires](https://www.amazon.com/gp/product/B07TX6BX47)|$15|
|[30 Row Breadboard](https://www.amazon.com/dp/B07PCJP9DY)|$6|
|[Wood Glue](https://www.amazon.com/dp/B001N7X1UA)|$3|
|[Clamps](https://www.amazon.com/dp/B0875WV3CD)|$30|
|[Wood Filler](https://www.amazon.com/dp/B00K25F1UW)|$11|
|[Putty Knife](https://www.amazon.com/dp/B06XC8ZGK2)|$6|
|[Sandpaper](https://www.amazon.com/dp/B07VT261KT)|$13|
|[Primer](https://www.amazon.com/dp/B00L20TRW4)|$12|
|[Spray Paint](https://www.amazon.com/dp/B000PIK1YC)|$9|
|[Masking Tape](https://www.amazon.com/dp/B001EJMS4M)|$11|
|[Dual Lock Fastener](https://www.amazon.com/dp/B004V3RALO)|$20|
|Various 3D Prints|$20-???<sup>3</sup>|
|Center Metal Panel|$15-???<sup>4</sup>|
|Wood Laser Cutting Service<sup>5</sup>|$160|
|||
|**Total**|**$275-$307** (Not incl. Laser Cutting)|

> <sup>1</sup> Try and get the flattest piece of plywood from your local hardware store. I notice a lot my options were slightly warped so I tried picking out the one with the least warping. Even if it's slightly dinged/has holes, that's likely okay as we will be using the wood filler to smoothen it out (step 1 below).

> <sup>2</sup> For the polycarbonate, I personally got the edges chamfered and the corners cut which does cost extra (for a total of ~$56). This makes the panel identical to an ITG/DDR panel in shape. You can alternatively simply get 10 3⁄4" x 3 15⁄16" rectangles for about $6 per panel.

> <sup>3</sup> I personally had access to a 3D printer so I only spent about $20 in materials. I don't know how much it costs to print these parts using a local service.

> <sup>4</sup> The pad is designed to use a DDR/ITG/PIU square metal panel which fits perfectly on top of the 10 7⁄8" x 10 7⁄8" square wood piece. You have the following options on how to procure one some replacement options:
> 1. Buy one from someone else/Andamiro or use one from an existing pad. I personally used one from my existing machine.
> 2. Bend metal yourself. I believe they are 1⁄8" thick 304 Stainless Steel. If you make the main center part 11" x 11" and the edges less than 1⁄2" tall (3⁄8" or 1⁄4" should work) then that should fit the square wood piece.
> 3. Replace the square wood piece with another material (e.g. polycarbonate). If you go this route you'd want it to be the full 11" x 11" (instead of the 10 7⁄8" x 10 7⁄8") as you won't be adding a metal piece on top of it.

> <sup>5</sup> While I don't think laser cutting the wood was needed and one could cut it on their own, I opted to pay for the service for the precision.

## Parts to 3D Print

|   Part           |Description    |
|------------------|---------------|
|[**The Box**](https://www.tinkercad.com/things/bpEsTf4kXBO)|Houses all the electronics|
|**FSR Blocks (Comes in [1⁄2"](https://www.tinkercad.com/things/cAF0ry7Ph2o) and [5⁄8"](https://www.tinkercad.com/things/kU1zQFTylWj) variants)**|Used to attach the FSRs. If you like your panels flush with the center and want to use less tape for adjusting the height, you can get the 5⁄8" variant|
|**Front Brackets (Comes in [1⁄2"](https://www.tinkercad.com/things/evKB2N12mK5) and [5⁄8"](https://www.tinkercad.com/things/hcPSjkuzODB) variants)**|Same idea as above. Use the same height that you chose for the FSR blocks above. This part is not necessary if you have rectangular panels.|
|[**Back Brackets**](https://www.tinkercad.com/things/07s7Wb1h3cf)|Used to support the backside of the panels. If you have rectangular panels, then print this part twice so you can also use this to support the frontside.|
|[**LED Diffusers**](https://www.tinkercad.com/things/8S0zVbZenex)|This is used to both add further support for the backside of the panels, while also allowing one to diffuse LED strips if one would like to add it to the travel pad. If you're using this for LEDs, you'd want to print this with Clear PLA. This piece is optional.|
|[**Panel Brackets**](https://www.tinkercad.com/things/keSFPU1u1Jc)|Used to hold the panel in and prevent it from popping out. The design is fairly fragile, and duct tape does perform just as well|

I personally use the 5⁄8" variants as I like my panels higher by default.

## Steps
 ### 1. Cutting the Pieces
If you decide to laser cut your plywood, you can use <a href="files/travelpad.dxf">this DXF file</a> to get a quote from a local laser cutting service. To view this file, You can download <a href="https://librecad.org/">LibreCAD</a> which is a free and open source software for CAD. Check out the image below to get an idea of what it looks like. It's designed to all fit on a 2' x 4' sheet of plywood. For me it cost about $160 to get it laser cut. Alternatively, if you have access to a hand saw/table saw, cutting the plywood youself could be considerably cheaper (potentially at the cost of time/precision).
 
The DXF file actually has three extra pieces in the case someone doesn't want to 3D print "The Box" (which was the initial plan). The extra pieces are the two longer walls and a small square cover. If you go that route, you will need to drill some extra holes for the wires. Because of that, I think it is preferred to print the box as I think it's a nicer and a more convenient design.
 
<p align="center"><img src="images/padcad.png" height="400px" /></p>

For the polycarbonate you have two options.
   1. You could simply get four 10 3⁄4" x 3 15⁄16" rectangles to save some of the cost.
   2. To make it more accurate to DDR/ITG refer to the image below for the dimensions. There is also approximately a 1mm chamfer which will make the edges not be so sharp (although you can probably chamfer/sand it yourself).

The reason the panel isn't an exact 4" is because having some wiggle room I think is helpful. This prevents the body of the pad from flexing which would otherwise affect the FSR reading. You can always later add some tape on the outsides to prevent the panel from moving around as well (which you can see in the image below).

<p align="center"><img src="images/panel.png"/></p>
    
### 2. Before the Build

After your wood is cut but before putting things together, we will want to first smoothen out your pieces. It's possible that your plywood has some holes and/or uneven surfaces. You can use the wood filler and sand paper to try and even them out. This is mostly important for the larger pieces (the base and the wooden square). Simply add some wood filler to the affected areas, smoothen it out with the putty knife, and let it sit until it's dry. Once it is, then sand the surface using 100 and then 150 grit sandpaper.

### 3. Building the Pad

Note that some of the pictures are slightly outdated as I had slightly modified the 3D printed parts (the files have been updated accordingly above). You should still be able to get a good idea of all the steps from the images below.

<p align="center"><img src="images/1.JPG" height="400px" /></br>Here is the base. Not much to say about this.</p>
<p align="center"><img src="images/2.JPG" height="400px" /></br>Add on the corner triangles. First, wood glue two of the triangles together (hold tight with the clamps). Once it has dried and set, then attach it to the base using the wood glue and clamps. Repeat for each the remaining two corners </p>
<p align="center"><img src="images/3.JPG" height="400px" /></br>Attach the walls. It is </b>VERY</b> important that you use clamps here to securely attach the walls to the base. If you don't you might run into issues with your <a href="https://clips.twitch.tv/AmazonianLaconicPineappleRlyTho-e3TrOF4Ut9JD_z1f">pad breaking</a> and you'll have to reglue it down the line.</p>
<p align="center"><img src="images/4.JPG" height="400px" /></br>Attach the 4 center triangles. This will be used to path the wires for the travel pad while adding support for the wooden square. It might be hard to get the clamps in place for this so I ended up just using some heavy weights. Make sure you measure before attaching it. It should be placed in a 11" x 11" square centered with respect to the pad base.</p>
<p align="center"><img src="images/5.JPG" height="400px" /></br>A (slightly) better view.</p>
<p align="center"><img src="images/6.JPG" height="400px" /></br>Check the positioning of the square wood piece. The 4 triangles that it sits on top of will poke out from under the center squre. This is intentional as the metal panel will sit on top of square wood piece, which will then give it the full 11"x11" size. <b>Do NOT attach the square piece to the base.</b></p>
<p align="center"><img src="images/7.JPG" height="400px" /></br>Smoothen the edges. It's possible some things might have been slightly misaligned when gluing things together. You can correct some of this by using the wood filler and sanding it down to a smooth finish.</p>
<p align="center"><img src="images/8.JPG" height="400px" /></br>Once you think your base is sanded and ready, you can then prime the two large pieces. Let it dry, flip it over, and then prime the bottom as well.</p>
<p align="center"><img src="images/9.JPG" height="400px" /></br>Once the primer has dried, you can mask off the insides and prep it for the main paint job.</p>
<p align="center"><img src="images/10.JPG" height="400px" /></br>Paint the two large pieces, let it dry, flip it over, and paint the bottom as well.</p>
<p align="center"><img src="images/11.JPG" height="400px" /></br>Once the paint has dried, remove the masking tape and check out your paint job.</p>
<p align="center"><img src="images/12.JPG" height="400px" /></br>Attach the 3D printed bits for the insides. For the front brackets and FSR blocks, I attached them using the Dual Lock Fasteners in case I ever wanted to swap them with the other height variant. I superglued the back brackets, but I did notice that sometimes they would come off and I needed to reglue them. Not really a problem, just something to note. The LED diffusers don't need to be fastened as they're intended to just slide in and out of the back brackets (for easy access to potential LEDs you might want to add later).</p>
<p align="center"><img src="images/13.JPG" height="400px" /></br>Check to make sure the center panel fits.</p>
<p align="center"><img src="images/14.JPG" height="400px" /></br>Add the wiring. Check out my <a href="https://www.github.com/teejusb/fsr">FSR guide</a> on how to set up the wiring and flashing the software. Notice the two strips of Dual Lock Fasteners. This is used to to attach the square wood piece to the base while still allowing it to be removable. I use the same fastener to attach the brackets that hold the panel in. As a fair warning, it's pretty hard to pry off the square wood piece with this method which could be seen as both good and bad. If you want to make it easier make it easier, one could use smaller lengths of the fastener so there's less force holding it together.</p>
<p align="center"><img src="images/15.JPG" height="400px" /><br>Pop in the panels! This is without the white cover taken off as the panels are actually clear but I thought this looked nicer :) I used the Dual Lock Fasteners to hold the brackets as well. One thing to note is that while the brackets do hold the panel in, they seem a bit fragile and seem to come off often. I did notice that duct tape did do a better job but that seems a bit jank so I do intend to come up with a better solution soon.</p>

### 4. Adding LEDs

Coming soon! The pad is designed to also have LEDs but at the moment I haven't completed that bit and the code doesn't have FastLED support out of the box.
