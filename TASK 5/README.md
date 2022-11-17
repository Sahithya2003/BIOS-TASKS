# IQ SIGNALS
- Quadrature signals, also called IQ signals, IQ data or IQ samples, are often used in RF applications. They form the basis of complex RF signal modulation and demodulation, both in hardware and in software, as well as in complex signal analysis

- A pair of periodic signals are said to be in “quadrature” when they differ in phase by 90 degrees.

- The “in-phase” or reference signal is referred to as “I,” and the signal that is shifted by 90 degrees (the signal in quadrature) is called “Q.”
- COSINE WAVE-IN-PHASE
- SINE WAVE-QUARATURE

- Software Defined Radio (SDR) systems use these concepts extensively because the baseband I & Q signals are often represented as discrete time sampled data. Therefore,   digital signal processing (DSP) can be used to literally define the transmitter and receiver characteristics including filtering, modulation and demodulation,SDR       receivers often feature a baseband bandwidth of a few hundred kHz or more, giving the ability to perform a wide variety of functions including “wide” bandscope and spectrogram functions, as well as being able to simultaneously monitor and demodulate several signals of different types at once.

- The general conclusion you can draw from this is that a RF signal with any type of modulation can be created with the appropriate I(t) and Q(t) baseband signals 

- If you take I and Q signals of equal amplitude and add them, the result is a sinusoid with a phase that is exactly between the phase of the I signal and the phase of the Q signal.

-  Sampling is the operation of observing a continuous signal and taking a finite number of samples at a given sampling rate fs. Hence IQ signals are used for signal modulation  for solving complex number equations while sampling the signal

- While simulating some radio we have mainly two type of signals:
 1. any low frequency or baseband signal are real signal, they are represented by real signals
 2. every passband signal(Energy =0 at 0hz frequency,and a spectrum located near a high frequency) must be represented by their equivalent baseband complex signal (excepted for systems having very low carrier frequency)
 
- When the maximum frequency of the signal spectrum do not respect Nyquist theorem, one should filter the signal with a low pass filter having a cutt-off frequency lower then Fs/2 before sampling: this correspond to the anti-aliasing filter used in every SDR hardware.(optional)-USE OF A LOW PASS CAPACITOR in AM MODULATION
- The I-channel preserves the symmetry in the RF input signal, while the Q-channel
converts even components to odd and vice versa. Every modern radio communication uses IQ modulator for emitting and IQ demodulator for receiving. The IQ demodulator is able to recover incoming i(t) and q(t)
- IQ-demodulator application is an image rejection/cancellation receiver with nonzero IF frequency,
- The image rejection (IR) is degraded in the presence of a quadrature phase error φ or
gain mismatch α between I- and Q-channels. The phase error introduces crosstalk
between the channels, while gain mismatch results in imperfect cancellation by the
adder:
