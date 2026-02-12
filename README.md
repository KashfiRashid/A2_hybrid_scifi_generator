README

Project: Hybrid Sci-Fi Generator
Course: IAT460 A2 - Rule-Based System
Option: Option 3 (Hybrid System)

Description
A hybrid generative system that combines generative grammars, Markov chains,
and L-Systems to produce sci-fi themed text narratives paired with procedural
alien flora visuals. Text content drives visual output through keyword-based
biome detection.

How to Run
1. Open the notebook in Google Colab
2. Run all cells from top to bottom (Runtime > Run all)
3. Re-run any Sample Output cell to generate a new unique output

What to Adjust
- mood: 'dread', 'wonder', 'tension', or None
- markov_words: controls length of Markov-generated field notes
- temperature: lower (0.6) = coherent, higher (1.6) = surprising
- L-System parameters: iterations, angle, distance in rulesets
- Training text: swap in different sci-fi passages for new vocabulary

Systems Used
1. Generative Grammar — structured mission logs and planet descriptions
2. Markov Chain — atmospheric descriptive passages with mood biasing
3. L-System — procedural alien flora/crystal visuals via matplotlib

Requirements
- Python 3
- matplotlib (pre-installed in Google Colab)
- Python standard library: random, math, collections
