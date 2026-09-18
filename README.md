## oriGEN
![origen_demo_example](https://i.imgur.com/aJou09a.png)

oriGEN is a proof-of-concept LLM fingerprinter. It takes a random string generated (password) by an LLM, and it reports which of four trained model families the distribution most closely matches, or that it matches none of them.

The architecture is a BERT-style encoder, it uses 4 layers, 4 attention heads, and a 128-dimensional embedding. The current weights are around 800K parameters in total. 

It is highly accurate on known models on a closed set, and even generalizes to knowing the providers of models it has never seen (if the provider is supported). Open-set detection is still improving.

A demo is currently available at: http://origen.mabutaha.me. 
This repository will be updated with the source code and weights in the future. 

*This tool accompanies a talk presented at BSides Amman (September 2026).*
