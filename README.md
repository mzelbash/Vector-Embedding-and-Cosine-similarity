# Vector Cosine Similarity: Interactive Explainer

# Visit my Github page to see this interative demo

https://mzelbash.github.io/Vector-Embedding-and-Cosine-similarity/

An interactive, self-contained HTML file that teaches vector cosine similarity through word embedding examples. No libraries, no build step — open the file in any browser.

## Demo

Three interactive sections:

**1. Dot Product and Angle**
Use a slider to rotate vector B and watch the cosine similarity update in real time. The canvas shows both vectors, the arc between them, and a projection line. Color coding: green (positive), gray (zero), red (negative). Preset buttons jump to Same / Perpendicular / Opposite.

**2. Word Similarity**
Four word vectors (dog, dog show, cat, airplane) are drawn as arrows from the origin. Click any of the six word pairs to highlight those vectors, draw the angle arc between them, and display the cosine similarity. Shows intuitively why related words (dog / dog show) have a smaller angle than unrelated ones (dog / airplane).

**3. Plurality Direction**
Step-by-step demonstration of vector arithmetic on word embeddings:

- Step 1: See the dog and dogs vectors side by side
- Step 2: Compute `dogs − dog` to extract a "plurality direction"
- Step 3: Project one, two, three, four onto that direction — an animated bar chart shows their scores increasing in order

## Usage

```
open Vector_Cosine_Similarity.html
```

No server needed. Works in Chrome, Edge, and Firefox.

## Concepts Covered

- Dot product as a measure of directional alignment
- Cosine similarity formula: `cos(θ) = A·B / (|A| × |B|)`
- Why similar words point in similar directions in embedding space
- Vector arithmetic: extracting semantic directions by subtraction
- Projecting word vectors onto a direction to rank words

## Notes

- The 2D word vectors are illustrative projections, not real trained embeddings.
- Real word embeddings (Word2Vec, GloVe, fastText) operate in 100–300 dimensions but follow the same geometric principles demonstrated here.

## Author

Dr. Elbasheer
