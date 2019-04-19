# Odd-One-Out-using-Word2Vec
Finding the Odd One Out using Word2Vec

### You can download the dataset from the given link.
https://drive.google.com/uc?id=0B7XkCwpI5KDYNlNUTTlSS21pQmM&export=download

This module implements word vectors and their similarity look-ups.

Since trained word vectors are independent from the way they were trained (Word2Vec, FastText, WordRank, VarEmbed etc), they can be represented by a standalone structure, as implemented in this module.

The structure is called “KeyedVectors” and is essentially a mapping between entities and vectors. Each entity is identified by its string id, so this is a mapping between {str => 1D numpy array}.

The entity typically corresponds to a word (so the mapping maps words to 1D vectors), but for some models, the key can also correspond to a document, a graph node etc. To generalize over different use-cases, this module calls the keys entities. Each entity is always represented by its string id, no matter whether the entity is a word, a document or a graph node.
