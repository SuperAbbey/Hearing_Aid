The functionality of the device can be classified into 4 main components.
The first component of bit and the y-axis to the amplitude or power of the device is the microphone. Cylewet cylindrical electret condenser microphone was used Fig. 4: Screenshot from the Teensyduino since it was small, portable, and had a frequency range of 50Hz to 20kHhz (considering that code showcasing the user-interface after inputting their dead region, allowing the humans can hear 1-20kHz). device to transpose accordingly

The second component is the processor. The Teensy 4.1 Processor was chosen for its Arduino compatibility and capabilities of real-time use with the speed of 600 MHz. Real time capabilities are crucial for hearing aid as the goal is to have little to no delays in sound output for the user.
Additionally, the processor comes with 1MB of RAM and 8MB of flash memory. Anticipating a memory problem with the code, a SD card was inserted.   T
The shield allows the device to convert between analog and [4] and [5]
digital signals. 
The audio shield consists of a 16 bit with a 44.1 kHz sample rate and an audio share is behind the ear hearing devices at 40 percent 

 One effect is the amplification that is filtered from the high review clearance2. In order to satisfy the quality system pass filter. The filter was used to focus on high frequencies. The library also allows data regulations, set by the FDA, this hearing device will collection of FFTs. Shifting of bins that are made during Fast Fourier Transform (shift the follow the consensus standards set through the American Standards National Institute (ANSI).
frequencies from high to low) is applied to satisfy the hearing range.

Our most difficult task of the project is to be able to successfully perform Fast Fourier
Transform on any audio data that the Teensy takes in and make it sound pleasant to the user. Our plans go as follows for the hearing aid:
- Take in Audio Data (Audio Shield) Take samples in the time domain
- Take FFT to convert to frequency domain (Teensy) Manipulate the frequency bins to do the
frequency shifting
- Take (Inverse)IFFT to convert back to time domain
- Send samples back to the audio interface(Audio Shield)
   Currently, we have completed the following, but when audio is heard by the user, it sounds
very robotic and lacks some natural sound to it. We are currently working on making the sound of the hearing aid feel more natural to the user and allowing the person to be able to have the adaptability to change the filtering so that higher or lower frequencies can be shifted according to the user. Additionally, we will be working on adding more bins to the code so that instead of there being around 700 there is around 100, we believe that this will help the user hear more
precise sounds and have natural flow to it.
   The naturality of the sound can also be fixed by adding another microphone to the processor and combine the sounds so that the parts that cannot be heard seem a little clearer.
   Also, we want to solder on a battery so that the device can be carried around by a user and be easily replaced when it runs out of battery, but of course, with this comes the case that has to be 3-D printed so the user can carry it around their neck or have it on their side.
