Python 3 fork of suffix-lemmatizer.

# suffix-lemmatizer

Suffix-lemmatizer is a lemmatizer for Estonian language, which handles both in- and out-of-vocabulary (OOV) words. OOV issue is addressed by generating candidate lemmas based on suffix transformations and ranking them using a statistical model.

## Installation
```
git clone https://github.com/estnltk/suffix-lemmatizer.git
cd suffix-lemmatizer
python setup.py install
```

## Usage
```python
  from suffix_lemmatizer import SuffixLemmatizer
  sl = SuffixLemmatizer()
  lemma = sl('metsast')
  print(lemma)
  >>> 'mets'
```
