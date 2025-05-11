# Modeling Neurotoxicity of Microplastics

Over the past couple years, many studies have found micro- and nanoplastics passing through the blood-brain-barrier (BBB). This is a big deal because the BBB is an extremely selective part of the neuroimmune system that prevents unwanted substances in the blood from entering the brain [1]. If these substances pass through, they get into the central nervous system (CNS), putting them into a direct contact with neurons, microglia, and astrocytes [2]. This contact may cause several disruptions, as described by the studies done on various species of nematodes, bivalves, crustaceans, fish and rodents. The disruptions include neuroinflammation caused by microglia (immune cells), disturbance in synaptic signaling, triggering of oxidative stress,  morphological changes, seizures, and increased risks of neurodegenerative diseases or mortality [3]. Microplastics are also known to cause cell obstruction, leading to reduced blood flow and neuronal abnormalities in mice [4]. Additionally, they can damage myelin sheaths within brain tissue, impairing the transmission of electrical signals and compromising the structural integrity of neurons [5].

Given the intriguing neurological effects of microplastics on organisms, I decided to model it as part of the project. The primary reference [3] for my project provides an overview of the literature that investigated the neurotoxic effects of micro- and nanoplastics. And one of the most frequently occuring effects was the inhibition of AChE activity. Acetylcholinesterase, AChE, is an enzyme that performs rapid hydrolysis of the neurotransmitter acetylcholine, ACh [6]. With exposure of microplastics, the activity of AChE gets inhibited, resulting in the accumulation of ACh in the synaptic cleft. This prolongs the depolarization caused by ACh. To simulate this, I am using the NEURON library where I model the membrane potential response of a postsynaptic neuron in the normal condition and compare that with the inhibited condition where the decay rate of ACh is reduced. 

The Jupyter notebook contains the code written.

# AI Contributions
I started with reading some of the papers mentioned in the reference section. Once I was sure that I want to model the neurological effects of microplastics wherein I compare what happens with a neuron or a network of neurons when there is no plastic and when there is, I took ChatGPT's help to get an idea of where to get started. The prompts given:

1. hey as part of my computational neuroscience project, i wanted to model the neurological effects of micro/nano plastics on brain (specifically, neuronal functions and interactions b/w neurons) upon passing through the BBB. I have been reading some paper that describe the neurotoxic effects of these plastics injected into organisms. And, there's papers that talk about how things passing through BBB affects the CNS and the brain. In fact, microplastics can carry pathogens too, so if they can pass, so can harmful pathogens colonizing the micropplastics. 

I want to model this. How do I go about using the tutorial models out there like NEURON, BRIAN, etc to do this? If there's something else I could use, please let me know.

2. there's this paper that mentions many studies done where organisms were dosed with plastic and their neurotoxicity was tracked. and a lot of them are AChE inhibition. so i want to work on that.

ChatGPT provided me with a basic script to do that, but by then I was not aware of NEURON script. So, I went through the documentation and practiced the python tutorials. Then I used the code ChatGPT provided as a reference and finished simulating.

# References
1. Blood–brain barrier. In Wikipedia. Retrieved May 11, 2025, from https://en.wikipedia.org/wiki/Blood%E2%80%93brain_barrier
2. Evans, T. American Society for Microbiology. (2020, April). How pathogens penetrate the blood-brain barrier. ASM. https://asm.org/articles/2020/april/how-pathogens-penetrate-the-blood-brain-barrier
3. Prüst, M., Meijer, J., & Westerink, R. H. S. (2020, June 8). The plastic brain: Neurotoxicity of micro- and nanoplastics - particle and fibre toxicology. BioMed Central. https://doi.org/10.1186/s12989-020-00358-y 
4. Huang, H., Hou, J., Li, M., Wei, F., Liao, Y., & Xi, B. (2025, January 22). Microplastics in the bloodstream can induce cerebral thrombosis by causing cell obstruction and lead to neurobehavioral abnormalities | science advances. ScienceAdvances. https://www.science.org/doi/10.1126/sciadv.adr8243 
5. Kim, D. Y., Park, M. K., Yang, H. W., Woo, S. Y., Jung, H. H., Son, D. S., Choi, B. Y., & Suh, S. W. (2025). Effects of Microplastic Accumulation on Neuronal Death After Global Cerebral Ischemia. Cells, 14(4), 241. https://doi.org/10.3390/cells14040241
6. Acetylcholinesterase. In Wikipedia. Retrieved May 11, 2025, from https://en.wikipedia.org/wiki/Acetylcholinesterase
7. Acetylcholine. In Wikipedia. Retrieved May 11, 2025, from https://en.wikipedia.org/wiki/Acetylcholine
