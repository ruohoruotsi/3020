# Garage &rarr; Audio listening studio


In late 2020 through early 2021, I renovated my [garage](https://en.wikipedia.org/wiki/Talk%3AUK_garage#Pronunciation_of_%22Garage%22) into a quiet audio listening room to work-from-home for my audio algorithms engineering job and to do audio production at night and at the weekend.

---

<img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/IMG_1005.JPG" width="45%"/> <img height="50" hspace="20"/> <img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/IMG_2001.JPG" width="47.5%"/>

## Reno & Deco
The reno started with new electrical wiring to provide dedicated circuits, GFCI outlets & dedicated in-wall heating. Then wooden carriage doors with windows replaced the old motorized, windowless, overhead doors (not shown). A top-to-bottom paint job dealt multiple layers of eggshell and battleship gray to the ceiling, walls & floors respectively.

<img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/IMG_1174.JPG" width="32%"/> <img height="30" hspace="3"/> <img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/IMG_1176.JPG" width="32%"/> <img height="30" hspace="3"/> <img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/IMG_2067.JPG" width="32%"/>

Next up, a [studio desk](https://www.etsy.com/listing/871333545/sitstand-music-studio-desk-keyboard-tray?ref=shop_home_recs_1&crt=1) build-out, acoustic design & procurement.

<img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/IMG_1515.JPG" width="48%"/> <img height="30" hspace="5"/> <img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/IMG_1815.JPG" width="48%"/>

<img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/IMG_1816.JPG" width="48%"/> <img height="20" hspace="5"/> <img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/IMG_1820.JPG" width="48%"/>

Finally decoration with my vinyl collection, [NASA recommended](https://medium.com/@iamgreenified/12-nasa-recommended-air-purifying-plants-that-you-must-have-in-your-house-8797645054b9) air-purifying plants, a rug, an [accent armchair](https://www.wayfair.com/furniture/pdp/george-oliver-bolebroke-3825-wide-tufted-polyester-armchair-fome7534.html?piid=32660419), various lighting strips & under-desk light bars.

<img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/IMG_1852.JPG" width="48%"/> <img height="30" hspace="5"/> <img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/IMG_1960.JPG" width="48%"/>

<img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/IMG_1962.JPG" width="48%"/> <img height="30" hspace="5"/> <img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/IMG_1963.JPG" width="48%"/>

## Acoustic Design

#### Challenges
The garage has a concrete floor with lathe & plaster {walls, ceiling}. These hard, reflective surfaces make the [space](https://en.wikipedia.org/wiki/Reverberation_room) excellent at holding sonic energy, making any kind of listening very difficult, notably below 250Hz (bass). Speech intelligibility also suffered when chatting in-person, as the unfettered reverberation caused consonant smear (less distinct articulation). Video calls were a nightmare.

#### Solutions
Below is a sketch I made to [compute room-modes](http://www.mcsquared.com/modecalc.htm) and discuss acoustic treatment options with the various vendors. After a few weeks of research and several hours on the phone, I converged on the following tube traps by [Acoustic Sciences](https://www.acousticsciences.com/pro) &rarr;
 - 6-ft stacks, 16inch diameter IsoThermal (bass) TubeTraps for room resonance control in the four corners
 - 4-ft StudioTraps for treble absorption & diffusion (and to create an attack-wall around my desk)
 - 5ft SoundPlanks for the back wall and "first reflection points", mixing broad-band absorption with diffusive reflections.

<img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/acoustics/IMG_1537.jpg" width="95%"/>

## How does it sound?

It sounds brilliant, the delta is startling & delightful. It's not perfect: first reflections aren't fully controlled due to the doors, the ceiling is currently untreated and stairwell's odd shape presents on-going symmetry challenges. But there's amazing clarity, dare I say, a smooothness to the acoustic response. In the evening, when the house is quiet, it's a joy to be in here ... just listening.

Let's look at before and after measurements using the standard room acoustics measurement and analysis software &rarr; [Room EQ Wizard](https://www.roomeqwizard.com/) (REW)

### Clarity
REW [measures clarity](https://www.roomeqwizard.com/help/help_en-GB/html/graph_clarity.html) using early to late (or total) energy ratios in dB, with early defined as the first {50, 80} milliseconds. Speech & music clarity are roughly modeled by C50 & C80.

<img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/acoustics/clarity.gif" width="85%"/>


### Spectrogram
In this [time vs frequency representation](https://www.roomeqwizard.com/help/help_en-GB/html/graph_spectrogram.html), the level is indicated by the colour while the vertical axis shows time, increasing towards the top of the plot with frequency on the horizontal axis. The areas where the response is decaying more slowly show up as vertical streaks; the dashed line shows the peak level in the plot at each frequency.  

After acoustic treatment, we see decay times much more tightly and evenly controlled across the spectrum, with room modes NOT ringing out and decay times mostly staying nicely below 250ms. No longer &ldquo;muddy&rdquo; or &ldquo;boomy&rdquo;.

<img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/acoustics/spectrogram.gif" width="90%"/>

### Reverberation Time (RT60)
RT60 is a measure of how long sound decays by 60dB in a space that has a diffuse soundfield, plotted at each one-third octave center frequency. There is a separate trace for the Early Decay time (EDT) in <span style="color:cyan">cyan</span>. Note that [RT60 for low frequencies](https://www.roomeqwizard.com/help/help_en-GB/html/graph_rt60.html) is not valid in small rooms, which explains the high {EDT, T30} wild measurements between {50, 130}Hz &rarr;
```
Domestic rooms are usually too small to have anything approaching a diffuse field
at low frequencies as their behaviour in that region is dominated by modal resonances
```

Similarly to the Spectrogram, we see specific decay times (EDT, T20, T30, Topt, TS) are tightly controlled above 130Hz.

<img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/acoustics/rt60.gif" width="95%"/>

### Waterfall
REW's sweep measurement [waterfall charts](https://www.roomeqwizard.com/help/help_en-GB/html/graph_waterfall.html) plots the frequency response as it decays in time. So a 3D plot. The different decay times at different frequencies show us how the room &ldquo;rings&rdquo; after the initial measurement sound is played.

<img src="https://raw.githubusercontent.com/ruohoruotsi/3020/main/images/acoustics/waterfall.gif" width="95%"/> \

We see strong **[Axial room modes](https://www.sweetwater.com/insync/different-room-modes-explained)** at {61.4, 97.4 & 139.5}Hz + harmonics. **Tangential modes** were absent where I had expected them, manifesting largely as nulls. The only exception was 152.4Hz, so more investigation is required. **Oblique modes** on the other hand at {271.3, 542.7, 723.6, 814}Hz are much less prominent as expected, and only visible at the right zoom level.

Finally, the high-frequency response is not over-dampened or &ldquo;dead&rdquo;, so the room is still feels lively but flutter echos, which live [between 1kHz - 2kHz](http://tor.halmrast.no/Why%20Do%20Flutter%20Always%20End%20Up%20Around%201-2kHz.%20IoA%2C%20page395-408%20paper53.pdf), are much better controlled.

### Final thoughts
Boomy, muddy rooms make critical listening very difficult. By controlling treble and bass decay times, I hear my nearfield speakers & subwoofer more clearly, speech is more intelligible. When mixing or doing audio production, there's less temptation to over/under-compensate with EQ or effects processing. The next step is to fine-tune the treatment to further improve bass-response, notably from under the stairwell, which only has a single 3-ft TubeTrap.
