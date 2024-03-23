# MakeMoreFr

In this project, I've developed a model aimed at generating names based on their French counterparts. This endeavor was inspired by methods discussed by Andrej Karpathy, as presented on his [YouTube channel](https://www.youtube.com/@AndrejKarpathy). My approach incorporates slight modifications to tailor the model for the peculiarities of the French language, particularly its dataset. 

The dataset employed contains 11,627 first names, encompassing a character set of 55 unique symbols. These names predominantly range from 6 to 7 characters in length, reflecting a typical structure in French nomenclature. A notable challenge in adapting English-based naming models to French is the latter's use of special characters, such as hyphens ('-') and apostrophes ('\''), not to mention various accentuated characters which are integral to the language.

The character mapping used in the model is as follows:

```plaintext
{0: '.', 1: ' ', 2: "'", 3: '-', 4: 'a', 5: 'b', 6: 'c', 7: 'd', 8: 'e', 9: 'f', 10: 'g', 
11: 'h', 12: 'i', 13: 'j', 14: 'k', 15: 'l', 16: 'm', 17: 'n', 18: 'o', 19: 'p', 20: 'q', 
21: 'r', 22: 's', 23: 't', 24: 'u', 25: 'v', 26: 'w', 27: 'x', 28: 'y', 29: 'z', 
30: 'à', 31: 'á', 32: 'ã', 33: 'ä', 34: 'å', 35: 'æ', 36: 'ç', 37: 'è', 38: 'é', 39: 'ê', 
40: 'ë', 41: 'ì', 42: 'í', 43: 'ï', 44: 'ð', 45: 'ñ', 46: 'ò', 47: 'ó', 48: 'ô', 49: 'õ', 
50: 'ö', 51: 'ø', 52: 'ù', 53: 'ú', 54: 'ü', 55: 'þ'}
```
![image](https://github.com/Slmaking/MakeMoreFr/assets/58626257/275deb27-d5d6-4be9-a905-5153f25f0032)

This character set reflects the linguistic richness and diversity of the French language, including punctuation and accent marks that are pivotal for accurate name representation. 
Through careful adaptation and testing, the model aims to produce names that are not only phonetically and structurally coherent but also culturally resonant with French linguistic patterns.

## the Bigram Model 

In the initial phase of our project, we explored the application of a bigram model for generating French names, a methodology inspired by the classical approaches in natural language processing. The bigram model, which considers pairs of characters (or "biograms") to predict subsequent characters in sequences, was applied to our dataset of French first names. The implementation details and findings are documented in our [GitHub repository](https://github.com/Slmaking/MakeMoreFr/blob/main/code/MakemoreFr_biogram.ipynb).


The bigram model operates on the principle that the likelihood of a character appearing in a name depends on its preceding character. This approach is particularly suited to languages like French, where character combinations frequently follow specific patterns, influenced by the language's phonetic and grammatical rules.


Given that you're transitioning from a bigram approach to experimenting with a Multilayer Perceptron (MLP) model for name generation, it's clear you're delving into more complex neural network architectures for this task. Here’s a structured way to discuss or document the MLP model based on your reference to the Colab notebook:

## MLP Model 

The details of this implementation are captured in a publicly accessible [Google Colab notebook](Given that you're transitioning from a bigram approach to experimenting with a Multilayer Perceptron (MLP) model for name generation, it's clear you're delving into more complex neural network architectures for this task. Here’s a structured way to discuss or document the MLP model based on your reference to the Colab notebook:

Following the exploration of bigram models, our project advanced to employing a Multilayer Perceptron (MLP) model, aimed at capturing more nuanced patterns within the French naming dataset. The details of this implementation are captured in a publicly accessible [Google Colab notebook](https://github.com/Slmaking/MakeMoreFr/blob/main/code/MakeMoreFr_MLP.ipynb).
