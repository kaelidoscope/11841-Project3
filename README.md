# 11841 Project 3

## Interactive Project using API

### Project Backgound

On 25th December 2021, NASA launched the much anticipated James Webb Space Telescope (JWST). JWST observes light in the infrared spectrum, outside the range of light detected by the human eye. The data transmitted to Earth reveals observations of distant stars, nebulas and exo-planets using the range of instruments onboard. The JWST requires temperatures of below -233°C to capture the infrared light spectrum, without heat interference from the telescope itself. It sits at the Sun-Earth L2 Lagrange Point in a halo orbit, 1.5M kilometers from Earth.
The 'images' it captures are outside of the visible light spectrum(Midinfrared MIRI -near infrared NIRI), so the composites of the image are produced by essentially shifting the lower infrared spectrum into visible light (Red-Violet) and colourising the separate image filters. The resulting images represent how humans might perceive the differences in detail were we able to view light in those wavelengths.

### Concept Ideation

When the composite images are colourised, the image artist assign colours to the filters, with red being the longest wavelength and violet on the shortest. The rest of the visible light spectrum (rainbow) of colours is then alloted to the between filters and layered together. For this project, I wondered how some of these images would look if represented within different parts if the spectrum.
What if it were possible to custom pick the colours you wanted to display the images in? It would make for some fairly thematically cohesive and amazing device wallpapers.

### Production

Elephant in the room...this may have been a little above my paygrade. Though I understand conceptually what needs to happen, and feel capable of devising various strategies to implement the creation of the project, Alas, I have not the skillset yet to gestate it into fruition.
Things started smoothly enough, with no qualms finding the JWST API, obtaining a functional data key, creating a repository on github, and creating the bones for the `.html` file.
I followed along with our class tutorials to reacquaint myself with jQuery and DOM data fetching. I have learnt some `PHP` in the past, but still feel I have a few 'blind spots' in my knowledge base.
My plan was to call the data from the JWST API, filter the data to find the image files that were `.fits` format as I discovered those were the ones most astrophotographers were using to render the compositie images. Filtering the image results by program ID would narrow the search. I Identified the program IDs with the suffixes using the JWST images already circulating on the web and found 5 from JW02727, JW02729, JW02731, JW02732 & JW02733. Filtering by suffix should have provided an array of images taken by the different instruments using different light wave filters. Sorting those `f****` images by ascending filter numbers would provide an array that a spectrum or gradient of colours could be applied to.
I stumbled upon a colour picker on W3 Schools, and was easily able to apply to my HTML file. I gave the 3 colour pickers id in order to apply an event listener that would be able to assign the user picked value to a variable that woould be dynamic, however, I was unable to find the correct coding syntax and the few times I attempted it on my own, I messed up the working JavaScript. I also had the brilliant idea of styling the colour pickers in the shape of the James Webb hexagon mirror array, but again, a tad complicated for me.
I did folow along with a brilliant [Online Tutorials](https://www.youtube.com/watch?v=YrOq7OpRV8I&t=1s) YouTube video which demonstrated how to create the button effect glassmorphism and neon light up effect.
I was able to troubleshoot some of the JWST API data with Ben, and retrieve the `.jpg` thumb nail images. After working on it on my own, I started to suspect that maybe the JWST data woulds be too complex to render. Especially if I was going to use an image processor to automate the functionality nrequired to process the raw image data. This was solidified by the fact that I was unable to find anyone else on the internet who had attempted or succeeded in this project.

### Reflection and Final Thoughts\

If I had more time to finesse and properly implement my intital idea, I would utilise NASA's Astronomy Picture of the Day API, convert it to a greyscale image so as to used the colour picker variables to assign to the RGB channels, then display the images layered ontop of each in a pop-up modal using the z-index and opacity stylings in CSS. I also came across a few interesting API projects and explored some of what IFTTT (If This, Then That) has to offer with the emergence of the new technology and Internet Of Things connecting more of our home systems.
