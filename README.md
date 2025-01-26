# Cycle 
### Cycling through a woman's phases. 

## Problem Statement
We’re addressing the challenge of inaccessibility and lack of personalization in wellness plans for woman. It's tailored to the four phases of the menstrual cycle (menstrual, follicular, ovulatory, luteal).

This issue impacts millions of menstruating individuals who experience fluctuating physical, emotional, and mental health needs throughout their cycles.

Existing wellness resources often provide generalized advice that doesn’t account for the hormonal changes and their effects on energy levels, mood, productivity, and physical health, leaving many feeling unsupported. This app is meant to provide woman with specialized workout and diet plans that are synced to their cycle and profile. 

## Technical Stack
We implemented a Retrieval Augmented Generation (RAG) pipeline to enhance our AI system's capabilities. The process involved two main components:

1.  Vector Database: We used Milvus, a vector database, to generate embeddings from our sourced health documents and store them efficiently. 

2.  Generation with Mistral API: For the generation phase, we utilized the Mistral API. When a query is received, the system retrieves relevant information from the Milvus vector database and uses it to augment the prompt sent to the Mistral language model. This approach allows the model to generate responses based on both its pre-trained knowledge and the specific health information we provided. 

This RAG pipeline enables our system to produce more accurate and contextually relevant responses by combining the power of large language models with our custom health dataset

## Conclusion
This app is a first step to allow women to take control of their health and cater their lifestyles to their body's natural cycle. Let's empower women to optimize their daily routines, including workouts and diets, based on their menstrual phases.
