## What is this?

Machine learning is everywhere in mass spectrometry now—it powers tools that search for modified peptides, sequence peptides from scratch, and make sense of complex data-independent acquisition runs. But before any model can touch a mass spectrum, that spectrum has to be turned into numbers the model can actually work with. This step, called encoding, is usually buried inside a tool's source code and rarely explained, which makes it hard to understand why these tools work or how to adapt them to your own data.
These notebooks pull that step out into the open. Using real mass spec data, they walk through three encoding strategies that modern proteomics tools rely on:
 - Spectral hashing — how ANN-SoLo (https://github.com/bittremieux/ANN-SoLo) compresses spectra for fast open modification search
 - Positional encoding — how the Casanovo (https://github.com/Noble-Lab/casanovo) transformer represents spectra for de novo peptide sequencing
 - Augmented spectra — how Cascadia (https://github.com/Noble-Lab/cascadia) combines signal across time to do de novo sequencing on DIA data Each notebook mixes runnable code with plain-language explanations and the math behind it, so you come away understanding how a spectrum becomes machine-readable—not just that it does. No setup required: every notebook opens and runs in Google Colab with one click (links below).


[01 - Introduction](https://colab.research.google.com/github/Alexander-Sol/MS_spectra_encoding/blob/Colab/01_Introduction.ipynb)

[02 - Spectral Hashing + ANN-SOLO](https://colab.research.google.com/github/Alexander-Sol/MS_spectra_encoding/blob/Colab/02_Spectral_Hashing_and_OMS.ipynb)

[03 - Postional Encoding + Casanovo](https://colab.research.google.com/github/Alexander-Sol/MS_spectra_encoding/blob/Colab/03_Casanovo.ipynb)

[04 - Augmented Spectra + Cascadia](https://colab.research.google.com/github/Alexander-Sol/MS_spectra_encoding/blob/Colab/04_Cascadia.ipynb)
