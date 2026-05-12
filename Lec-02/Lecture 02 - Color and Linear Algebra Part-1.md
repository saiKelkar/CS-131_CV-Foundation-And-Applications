**Color:** (it's an internal interpretation)
-- Physical property: Light has wavelengths and intensities. 
-- Psychological property: Brain's way of associating the wavelengths with the color names so we can tell the objects apart. 
-- Summary: Color exists only in the mind of the beholder. Without a visual system (an eye and a brain), the universe is just a mix of electromagnetic radiation of varying frequencies. 

*Note:* 
*-- wavelength $(\lambda)$ is a primary metric we use to define the type or identity of light*
*-- it is the physical distance between two consecutive peaks (or troughs) of a wave*
*-- for visible light, we use nanometer (nm)*
*-- wavelength is inversely proportional to energy*
*(longer wavelength = lower energy; e.g., red light)*
*(shorter wavelength = higher energy; e.g., blue light)*

**Electromagnetic Spectrum:** (visible light is just a tiny part of the massive spectrum that includes everything from radio waves to x-rays)

color -- wavelength range (approx.)
violet ( 380 - 450 nm )
blue ( 450 - 495 nm )
green ( 495 - 570 nm )
yellow ( 570 - 590 nm)
orange ( 590 - 620 nm )
red ( 620 - 750 nm )

-- visual spectrum of light ranges from 400nm to 700nm, humans are most sensitive to light with wavelengths in the middle of this spectrum
-- our eyes are evolved to match the sun's output, as sun is a giant ball of gas at a specific temperature and hence pumps out the most energy in the visible range
-- if we lived near a much cooler, redder star, our visible spectrum might be shifted towards the infrared

*Note:*
*-- EM spectrum is the entire range of all possible frequencies of electromagnetic radiation - light is just a tiny slice of this*

*region - wavelength size - common usage / source*
*radio waves - buildings to water bottles - Wi-Fi, radio, tv signals*
*microwaves - centimeters - microwave ovens, radar*
*infrared - needle point - heat lamps, remote controls, thermal cameras*
*visible - protozoa - human vision (400nm - 700nm)*
*ultraviolet - molecules - sunburns, sterilization*
*x-rays - atoms - medical imaging*
*gamma rays - atomic nuclei - radioactive decay, cosmic events*


**Planck's Law and Blackbody Radiation:**
-- blackbody is an idealized object that absorbs all radiation and emits energy based solely on its temperature
-- Planck's law describes the spectral density of this radiation:

$$B(\lambda, T) = \frac{2hc^2}{\lambda^5} \frac{1}{e^{\frac{hc}{\lambda k_B T}} -1}$$

h = Planck constant
c = speed of light
$k_B$ = Boltzmann constant
T = absolute temperature (Kelvin)

Wien's Displacement Law (a derivative of Planck's) 
-- as an object gets hotter, the peak wavelength shifts to the blue (shorter wavelengths)
-- this is why a heating element glows red first, then yellow, then eventually blue-white if it gets hot enough

*Note:*
*-- spectral density (a way of saying, "how is the energy spread out?")*
*e.g., imagine we have a bag of 100 marbles (the total energy)*
*-- if we put 20 marbles in red bucket, 50 in green, and 30 in blue, we have described the density or distribution of those marbles across the colors*
*-- spectral density does the same for light - it tells us exactly how much power (energy per second) is present at each specific wavelength*
*-- if a light source has high spectral density in the 650nm range, it means that light source is pumping out a lot of red energy*

**Physics of Light (Spectra):**
-- every light source has a power spectral distribution (PSD)
-- sunlight: relatively flat, contains all colors (white light)
-- fluorescent light: has sharp spikes at specific wavelengths
-- led: often have a big spike in blue and a broad hump in yellow/orange

-- surface reflectance: objects don't have a color, they have a reflectance function (a tomato doesn't possess redness, it's molecular structure is simply very good at absorbing blues and greens and spitting back the red wavelengths)

Interaction of Light and Surfaces:
-- the light that actually hits your eye is called the color signal
$$C(\lambda) = I(\lambda) \times R(\lambda)$$
$I(\lambda)$ = the illuminant (the light source spectrum)
$R(\lambda)$ = the surface reflectance (what the object keeps vs. what it reflects)
$C(\lambda)$ = the color signal (the light that actually enters your eye)

-- the missing piece is the observer (to turn the color signal into an actual perceived color, you have to multiply it by the sensitivity of the human eye's cones - long, medium, and short wavelengths)

*Note:*
*-- PSD is a graph or a data set that shows the fingerprint of a light source. It plots Power (vertical axis) against Wavelength (horizontal axis)*
*-- Why spectral matters: if we know the PSD of a light bulb and the Reflectance Spectrum of a wall paint, we can mathematically predict exactly what color that wall will look like under that light.*

**Rods and Cones (the Sensors):**
-- our eye is like a digital camera, but instead of a uniform grid of pixels, our sensor (the retina) has two very different types of light-detecting cells
-- rods(night vision): 
	-- these are incredibly sensitive
	-- they can trigger from a single photon
	-- they all have the same filter, so they can't distinguish between colors (this is why everything looks grayscale in a very dark room)
-- cones(color / detail):
	-- these require much more light to fire
	-- they are packed mostly in the center of your vision (the fovea), providing the high resolution you need for reading or recognizing faces

**Three Number concept:**
-- human eye compresses a complex, continuous spectrum of light into just three electrical signals
-- each type of cone acts like a filter, we call them S, M, and L (short, medium, and long wavelengths)
	-- S-cones: Peak around 440nm (Blue)
	-- M-cones: Peak around 530nm (Green)
	-- L-cones: Peak around 560nm (Red / Yellow)

-- when light hits our eye, our brain doesn't see the whole graph (spectrum); instead, it does a quick calculus problem for each cone type
$$V = \int_{400}^{700} \Phi(\lambda) \cdot S(\lambda) \, d\lambda$$
V = response of a cone
$\Phi$ = light spectrum
S = cone's sensitivity

-- because we have three types of cones, our eye sends exactly three numbers to the brain
-- this is why we use RGB (Red, Green, Blue) in screens

**Metamerism - the Great Illusion:**
-- because we compress a complex spectrum (which could have infinite variations) into just three numbers, we lose data
-- metamers are two different light spectra that result in the exact same three numbers being sent to the brain
(e.g., pure yellow laser - one spike at 580nm, might look identical to a mix of red and use green light. Even though the physics are different, our brain can't tell them apart because they stimulate our M and L cones in the same proportion)

**Color Matching and Trichromatic Theory:** (color matching experiment - a proof that our vision is trichromatic)
-- a subject looks at a test light (a color)
-- they are given three primary lights - typically RGB
-- by adjusting the weights (intensity) of those three primaries, they can recreate the appearance of almost any test light
(this is the foundation of every display technology we use)

**Color Space:**
-- color space is like a coordinate system - (R, G, B) or (H, S, V) triplet tells us where a color sits in a color space
-- the goal is to map every perceivable color to a unique set of numbers so that a computer or a printer can reproduce it exactly

**Linear Color Space (RGB and XYZ):**
-- Grassmann's Law: human color perception behaves like linear algebra (e.g., if you mix two lights, the resulting color is simply the sum of their vectors)
-- RGB Space (the Problem): because of how our cones overlap, there are some 'real-world' colors that a standard monitor cannot recreate by just adding R, G, and B. To match them in a lab, you'd actually have to subtract light (which is physically impossible for a screen)
-- CIE XYZ (the Master space): to fix the negative numbers problem in RGB, CIE XYZ is created. 
Y = Luminance (specifically designed to match the human perception of brightness)

As both are linear, we can convert RGB to XYZ using a simple 3x3 matrix:
$$\begin{bmatrix} X \\ Y \\ Z \end{bmatrix} = \mathbf{M} \begin{bmatrix} R \\G \\ B \end{bmatrix}$$
**Nonlinear Color Space (HSV):**
-- Hue (H): the flavor of the color (Red, Orange, Blue). Usually mapped to an angle (0° to 360°)
-- Saturation (S): the purity or vibrancy. 0% is gray and 100% is the pure color
-- Value (V): the brightness. 0% is black

**White Balancing:**
-- Different light sources have different temperatures. 
For e.g., a candle or a sunset gives off a warm, orange glow, while a cloudy sky or a fluorescent office light gives off a cool, blue tint. 
-- Our brains are smart - if you hold a white piece of paper under a yellow light bulb, our brain tells us 'that paper is white'. A camera, however, just sees 'yellow paper'.
White balancing is the process of telling the camera to ignore those tints so that neutral colors (whites and grays) look natural. 

Importance of white balancing: (without white balancing, images would look off - usually too orange or too blue)
- Our eyes vs. Sensors: The brain auto-corrects light in real-time. A camera sensor is a literal machine; it just records exactly what it sees without the benefit of human perception.
- Screens aren't the same: An image might look perfect on our phone but looks slightly green on a laptop or different again when printed. White balancing provides a standardized neutral starting point so the image looks consistent across different devices. 
- The vibe of the room: When we take a photo in a dimply lit cafe, our eyes adapt to the mood. But when we look at the same photo later in bright daylight, the yellowish tint from the cafe lights will look messy and unnatural unless the white balance was adjusted to compensate. 

**Von Kries Method (The Volume Knob Approach):**
(most basic way to fix color) Imagine our image has three volume knobs: Red, Green, and Blue. If the photo looks too blue, we simply turn the blue knob down or the red/green knobs up until it looks balanced.

- Gray Card Method: to do this accurately, we hold up a card that is perfectly neutral gray in front of the camera. The camera looks at it and says, 'this should be neutral, but I'm seeing it as 10% too blue'. 
  It then calculates exactly how much to turn down the blue channel across the whole photo to make the card look gray again. 

**Other Methods (The Guessing Game):**
If you don't have a gray card, the computer has to guess what 'neutral' should look like. 

- Gray World Assumption: This assumes that if we took every single pixel in a normal photo and mixed them all together in a blender, the result would be a middle-gray. 
  *The computer calculates the average color of the whole photo. If the average is slightly orange, it shifts the entire image toward blue to bring that average back to neutral gray.* 
- Brightest Pixel Assumption: This assumes that the brightest part of a photo (like a reflection on a window or a white shirt) is the same color as the light source. 
  *It finds the brightest pixels and assumes they should be pure white. If those pixels looks slightly yellow, the computer adjusts the whole image to remove that yellow tint.* 
- Gamut Mapping: A gamut is like a boundary map of all the colors present in a photo. 
  *It treats the colors like a 3D shape. It takes the tilted shape of your off-color photo and mathematically stretches and squashes it until it matches the shape of a standard photo taken under perfect while light.* 

**Other uses of Color in CV:**
Color isn't just for making photos look pretty; it's a tool for AI to understand what it's looking at:

- Detection: Certain things have very specific color signatures. For e.g., skin tones (regardless of ethnicity) fall into a very specific range on the color spectrum, making it easier for AI to find people in a crowd or filter out inappropriate content. 
- Segmentation: Color helps the computer 'cut out' objects from the background. If a blue chair is sitting on a green floor, the color difference is the easiest way for the computer to draw a line between the chair and the ground. 

**Linear Algebra Primer: Vectors and Matrices**
Vectors and matrices are collections of ordered numbers that represent something: movement in space, scaling factors, pixel brightness, etc. 

Column vector ($v$): This is a standing list (numbers stacked on top of each other)
Row vector ($v^T$): This is a lying down list (numbers are side-by-side)
Transpose ($T$): This is the flip (if we have a standing list and we transpose it, it becomes a lying down list and vice versa)

What do these numbers actually represent?
- Point in space (geometric) -- (most intuitive version)
  if we have a 3D space, a vector like [3, 4, 5] represents a specific location or an offset (move 3 units right, 4 units up, 5 units forward)
- A collection of data (abstract) -- (the numbers are attributes)
  imagine a vector that stores the brightness of 100 pixels in a row
  even if these numbers aren't locations, we can still use math to find the distance between two data vectors. if the distance between two pixel-data vectors is small, it means the two images look very similar. 

