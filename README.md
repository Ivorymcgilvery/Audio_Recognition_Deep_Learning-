# Audio_Recognition_Deep_Learning- Class project
Context
In the last few decades, significant advances have been achieved in the area of audio recognition. A lot of research is ongoing globally to recognize audio data or speech using Deep Learning. The most common use case in this field is converting audio to spectrograms and vice versa.

Audio in its raw form is usually a wave and to capture that using a data structure, we need to have a huge array of amplitudes even for a very short audio clip. Although it depends on the sampling rate of the sound wave, this structured data conversion for any audio wave is very voluminous even for low sampling rates. So it becomes a problem to store and computationally very expensive to do even simple calculations on such data.

One of the best economical alternatives to this is using spectrograms. Spectrograms are created by doing Fourier or Short Time Fourier Transforms on sound waves. There are various kinds of spectrograms, but the ones we will be using are called MFCC spectrograms. To put it in simple terms, a spectrogram is a way to visually encapsulate audio data. It is a graph on a 2-D plane where the X-axis represents time and the Y-axis represents Mel Coefficients. But since it is continuous on a 2-D plane, we can treat this as an image.

Objective
The objective here is to build an Artificial Neural Network that can look at Mel or MFCC spectrograms of audio files and classify them into the 10 classes that represent the 10 unique digits in the spoken Engilsh language. The audio files are recordings of different speakers uttering a particular digit and the corresponding class to be predicted is the digit itself.

Dataset
The dataset we will use is the Audio MNIST dataset, which has audio files (having .wav extension) stored in 10 different folders. Each folder consists of these digits spoken by a particular speaker.

Understanding the required packages
Librosa: Librosa is a Python package that helps in dealing with audio data. librosa.display visualizes and displays the audio data using Matplotlib. Similarly, there exists a collection of submodules under librosa that provides various other functionalities.
Run the command in the next cell to install the library.

IPython.display: Display is a public API to display the tools available in Ipython. In this case study, we will create an audio object to display the digits in the Audio MNIST data.
tqdm: tqdm is a Python package that allows us to add a progress bar to our application. This package will help us in iterating over the audio data.
