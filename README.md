# Term-Project
multi-speaker identification 
# Literature Review:

**Speaker Diarization:**

- **Speech Detection: ** Extract speech part in one audio recording using a Voice Activity Detector (VAD) module.
- **Speech Segmentation:** Extract out small segments of your audio call in a continuous manner.
- **Embedding Extraction:**  This system creates a neural-network based embedding of your speech segments extracted in the previous step. An embedding is a vector representation of data which could be used by the deep learning framework.
- **Clustering:**  Cluster embeddings we created above and the system will training itself by using supervised learning method in order to identify which embeddings are belong to same speaker and assigned the label of that speaker as well.
- **Transcription:** Segment out the audio into clips belonging to each speaker, and pass it to a Speech-to-Text model (or  **ASR** ) which produces the transcript of the speech segment.

**Speech Recognition:**

Practical speech recognition systems start by listening to a chunk of sound read through a microphone. The first step involves digitizing the sound by a piece of hardware (or software) called an analog-to-digital (A/D) converter. The digital data is converted into a spectrogram using a mathematical technique called a Fast Fourier Transform (FFT)), then broken into a series of overlapping chunks called acoustic frames, each one typically lasting 1/25 to 1/50 of a second. These are digitally processed in various ways and analyzed to find the components of speech they contain. Assuming we&#39;ve separated the utterance into words, and identified the key features of each one, all we have to do is compare what we have with a phonetic dictionary (a list of known words and the sound fragments or features from which they&#39;re made) and we can identify what&#39;s _probably_ been said.

There are two common methods used to how computers recognize speech:


### Statistical analysis

### Virtually all modern speech recognition systems also use a bit of complex statistical hocus-pocus to help figure out what&#39;s being said. The probability of one phone following another, the probability of bits of silence occurring in between phones, and the likelihood of different words following other words are all factored in. Ultimately, the system builds what&#39;s called a [hidden Markov model](https://en.wikipedia.org/wiki/Hidden_Markov_model) (HMM) of each speech segment, which is the computer&#39;s best guess at which beads are sitting on the string, based on all the things it&#39;s managed to glean from the sound spectrum and all the bits and pieces of phones and silence that it might reasonably contain.


### Artificial neural network

###  computer scientists developed &quot;connectionist&quot; computer models that could mimic how the brain learns to recognize patterns, which became known as [artificial neural networks](https://www.explainthatstuff.com/introduction-to-neural-networks.html) (sometimes called ANNs).
