# Product Recommendation by Azure OpenAI Embedding model (text-embedding-ada-002)

In a previous repo [(Content Based Product Recommendation Samples)](https://github.com/easonlai/content_based_product_recommendation_samples), I showed how to use [TF-IDF](https://en.wikipedia.org/wiki/Tf%E2%80%93idf) to vectorize product key phrases and recommend products based on [cosine similarity](https://en.wikipedia.org/wiki/Cosine_similarity). Now, I have improved the demo by using [Azure OpenAI](https://learn.microsoft.com/en-us/azure/cognitive-services/openai/overview)’s Embedding model [(text-embedding-ada-002)](https://learn.microsoft.com/en-us/azure/cognitive-services/openai/concepts/models#embeddings-models), which has a powerful [word embedding](https://openai.com/blog/new-and-improved-embedding-model) capability. This model can also vectorize product key phrases and recommend products based on cosine similarity, but with better results. You can find the updated repo here.

TF-IDF is a statistical measure that assigns a weight to each word based on how frequently it appears in a document and how rare it is across all documents. Word embedding is a technique that converts a word to a vector of numbers that captures its semantic and syntactic features. Words that are similar in meaning or usage have similar vectors, while words that are different have different vectors. TF-IDF vectors are sparse and do not account for semantic similarities between words, while word embedding vectors are dense and can capture the relationships between words1. Word embedding can also handle words that are not in the vocabulary by using subword information1, while TF-IDF can only use the words that are in the predefined vocabulary.

Content: 
* \data\face_cosmetics_products_data.csv <-- Sample dataset of face cosmetics products from [Max Factor](https://www.maxfactor.com/en-gb).
* \data\shampoo_products_data.csv <-- Sample dataset of hair shampoo products.
* face_cosmetics_by_product_details.ipynb <-- Perform word embedding by Azure OpenAI Embedding model (text-embedding-ada-002) for the "Product Details" and provide product recommendations by cosine similarity.
* face_cosmetics_by_product_benefits.ipynb <-- Perform word embedding by Azure OpenAI Embedding model (text-embedding-ada-002) for the "Product Benefits" and provide product recommendations by cosine similarity.
* shampoo_by_product_details.ipynb <-- Perform word embedding by Azure OpenAI Embedding model (text-embedding-ada-002) for the "Product Details" and provide product recommendations by cosine similarity.
* shampoo_by_product_details.ipynb <-- Perform word embedding by Azure OpenAI Embedding model (text-embedding-ada-002) for the "Product name" and provide product recommendations by cosine similarity.

Enjoy!