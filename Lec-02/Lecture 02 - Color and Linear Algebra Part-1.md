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
  