README

Project: Hybrid Sci-Fi Generator
Student: Md Kashfi Or Rashid Pranta (301540943)
Course: IAT460 A2 - Rule-Based System
Option: Option 3 (Hybrid System)

Description
A hybrid generative system that combines three rule-based engines — generative
grammars, Markov chains, and L-Systems — to produce sci-fi themed text
narratives paired with procedural alien flora visuals. Generated text content
drives the visual output through a keyword-based biome detection system,
creating coherent connections between narrative and image.

How to Run
1. Open the notebook in Google Colab
2. Run all cells from top to bottom (Runtime > Run all)
3. Re-run any Sample Output cell to generate new unique stories and visuals
4. Use the Interactive Mode cell at the bottom to choose mood, grammar,
   and chain at runtime via input prompts

Interactive Mode
The final cell provides user-facing parameter adjustment:
- Mood selection: dread, wonder, tension, or press Enter for random
- Grammar selection: mission (structured logs) or planet (world descriptions)
- Chain selection: space (ship/deep space) or alien (planet surface)
The system detects a biome from the generated text and draws a matching
L-System visual automatically.

What to Adjust (in code)
- mood: 'dread', 'wonder', 'tension', or None
- markov_words: controls length of Markov-generated field notes
- temperature: lower (0.6) = coherent, higher (1.6) = surprising
- L-System parameters: iterations, angle, distance in rulesets
- Training text: swap in different sci-fi passages for new vocabulary

Systems Used
1. Generative Grammar — two rulesets (Mission Grammar, Planet Grammar)
   producing structured mission logs and planet descriptions
2. Markov Chain — two order-2 models (Space Log, Alien World) generating
   atmospheric descriptive passages with mood biasing
3. L-System — three rulesets (Spiral Flora, Crystal Spire, Bioluminescent
   Tendril) rendered via matplotlib with four sci-fi color palettes

Sample Outputs
The notebook includes 5 sample outputs, each with a markdown explanation
describing the grammar, chain, and mood combination used and how it
affects the generated result.

Requirements
- Python 3
- matplotlib (pre-installed in Google Colab)
- Python standard library: random, math, collections
- No additional libraries or requirements.txt needed
