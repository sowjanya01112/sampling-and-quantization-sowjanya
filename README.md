# SAMPLING AND QUANTIZATION: BRIDGING THE ANALOG-DIGITAL DIVIDE

# •	Introduction:
It is now extremely difficult to imagine a world without digital technology being part of everyone’s lives daily, starting with the cellphones we use, and extending to the music and video streaming we employ. But how do we turn or transmute the real, analog signals that we witness in day-to-day life for example sound, light or even temperature into the digital language of 0 and 1 that the computer recognizes? This transformation occurs through two fundamental processes: sampling and quantization. Two of the most important sub-techniques of digital image processing are sampling and quantization. These processes are at the heart of what is called Digital Signal Processing (DSP) and are the means by which can be converted into digital form, signals that vary smoothly with time.

In fact, sampling captures “frames” of the signal at equal periods separating them, which leads to the conversion of the continuous-time signal. Quantization, however, assigns discrete values to these samples’ amplitudes by rounding the value to the closest that is possible in a digital format. It is therefore noteworthy that these would not be achievable through digital communication, high quality audio/video recording and streaming if these processes were absent. As part of our understanding of sampling and quantization, this blog post will look at how these processes occur, why they are important and the difficulties associated with them.

# • What is Sampling?
Sampling is a technique of taking selected points from a continuous signal at equal intervals. Usually, we have a sound wave that will represent a bit of music or a voice, for instance, in this case. This is so because the signal is described to persist along the time axes, which implies that it takes an infinite set of point values between two points in time. Sampling produces a sequence of discrete samples of the signal that collects a “picture” periodically or in other words periodically slices the signal.

These intervals are relative to the sampling rate, for which the unit of measure is samples per second, or Hertz (Hz). Since the fundamental reason for sampling is to obtain a continuous signal in order to analyze it, the fundamental rule is that the higher the sampling rate the more accurately the sampled signal can reconstruct the original continuous signal. For instance, in audio processing the sampling rate is normally set to 44.1 kHz that implies that 44,100 samples are made per second. This is the standard rate for CD quality audio because it is able to pass frequencies up to 22.05 kHz which is deemed to represent the whole frequency range of the human ear (20 Hz – 20 kHz).

 
# • Nyquist-Shannon Sampling Rate:
Another crucial knowledge connected with sampling is the Nyquist-Shannon Sampling Theorem. They postulated that the sampling frequency should be not less than twice the highest frequency contained in the signal in order to get an accurate sample. If the sampling rate is set too low, there is a phenomenon known as aliasing, providing low frequency components of the signal what actually are high frequency components of other signal, which distorts the signal.

For instance, let us look at audio recording. Digital records also require that the sampling rate be twice the maximum frequency of the signal one wants to sample; for instance if one wants to record sound up to 20 kHz, the sampling rate has to be 40 kHz at the least. If you had sampled at only 20 kHz or lower, the higher frequencies would fold back into the lower spectrum a process known as aliasing.


# • What is Quantization?
The necessary procedure following sampling is called quantization. Quantization basically involves changing the amplitude of each sample from a continuous value to a discrete value. In other words, it quantises the amplitude of each sample and brings it to the closest number closer to a digital system.

Quantization is important because different from sampling, which converts the signal into discrete points in time, quantization circumscribes the precision of the points in time by assigning each the value on the predetermined scale. Quantization accuracy is defined by the bit depth, which means how many levels may be used to encode the signal’s amplitude for each sample. Higher bit depths enable the system to provide better signal representation but this comes at the cost of more storage.

For instance, in the audio application, a 16-bit depth is used, that is, 16 bits are used for each sample, and there exist 65,536 distinct levels. The above-mentioned calibration suffices as far as depicting the variability of music and speech is concerned. Electing to go to a higher bit depth of 24 as is sometimes done in the pro audiophile 24-bit audio realm, gives yet more precision or resolution of 16,777,216 levels and even greater dynamic scope as well as better sound clarity. Yet, it does so at the cost of file size, which is definitely larger compared to the previous example.


# • Uniform vs Non-Uniform Quantization:
Quantization can be either Uniform or Non-Uniform:
# 1.	Uniform quantization:
Uniform quantization has always sized the interval between the steps uniformly across the amplitude range.
# 2.	Non-Unifrom quantization:
Non-uniform quantization chosen in many audio compression systems such as MP3 uses more levels where the signal is most likely (for example, for lower amplitudes) thus yielding higher efficiency with small degradations in the accuracy of quantization.


# • Understanding the Relationship between Sampling and Quantization:
Sampling and quantization are virtually inseparable processes, which in conjunction help to pass a signal from the analog domain into the digital domain. While sampling identified when we take a snapshot of a continuous signal, quantization identifies to what precision we can describe the amplitudes of the taken data points.

Together, these processes introduce two types of errors:
# 1. Aliasing:
This is a caused by low sampling rate and high frequencies are wrongly translated as lower ones.
# 2. Quantization Noise:
This is the rounding error which is the quantization of the signal’s amplitude to the nearest levels of quantisation. Unfortunately, the noise increases as the bit depth decreases, which means that using a low bit depth will result in much higher noise levels.

Sampled data anti-aliasing filters can reduce the problem of aliasing by eliminating high-frequency information before sampling. Just as with increasing bit depth, methods that lessen quantization noise include quantizing less often, although this also enlarges the amount of data needed to store the signal.


# • Applications of Sampling and Quantization:
Sampling and quantization are applied in a vast number of the currently used technologies ranging across multimedia processing, telecommunications, up to the medical equipment.

# 1. Audio Recording:
When you listen to digital music whether from a CD or through possibly a web link, you are in essence seeing the fruits of sampling and quantization. You get the actual recording of music by converting it into electrical signals, which record the sound waves as a signal that is continuous; then by taking a view of it repeatedly at uniform intervals – in the case of 44.1 kHz – you get the samples and then quantize the amplitude of the samples to either a 16 or 24 bit value. This process means that sound in digital format can be stored and played back without suffering form major deterioration.

# 2. Video Compression:
In the digital video, each video frame is taken as the image where the amplitude or the color and brightness of each pixel is quantized. As mentioned with video codecs, H.264 or HEVC, sampling and quantization techniques are used to produced very small videos while having a reasonable quality. For example, the raising of the frame rate (sampling rate) and color depth (quantization levels) contribute to the rise of the video quality but results to massive video file size.

# 3. Image Compression:
Images, like videos, are taken in sequences with analogue means and converted into numerical format for storage purposes. The JPEG format applies some form of quantization to images by reducing the number of bits per pixel that is used to represent the pixel intensity. This results in at least a one hundredth of their original size, while still losing some image quality.


# • Challenges and Limitations:
While sampling and quantization have contributed to the achievement of the digital age they come with several problems. The first one is the conflict of interest between the characteristics of high fidelity and the separability feature. Using a low sampling rate cause aliasing and similarly, using low bit depth will cause quantization noise. Of these two, both degrade the quality of the signal.

In audio processing, highly effective technique called Dithering can be used to minimize the quantization noise audible. It operates by involving a low level of random noise to the signal before quantization to make it hard to detect the noise. But this comes with some increase in the overall noise level as a couple of points out.


# • Conclusion:
Sampling and quantization are the main fundamentals of digital signal processing, this makes it easier to sample, store and transmit analog signals in digital manner. From music, video and or images these processes make it easier for us to enjoy quality digital media and facilitate gadgets such as smart phones, streaming services or even medical equipment. Ongoing improvement in the sophistication of computing as a platform of Data Storage, we should expect further enhancement of these processes that produces more efficient discrete approximation of real-life processes in Analog Domain.

