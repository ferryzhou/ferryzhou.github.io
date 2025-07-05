---
title: "Encoder only models"
date: 2024-12-20
---

<a href="https://huggingface.co/blog/modernbert">https://huggingface.co/blog/modernbert</a>

many practical applications need a model that’s lean and mean! And it doesn’t need to be a generative model.

Of course, the open-ended capabilities of these giant generative models mean that you can, in a pinch, press them into service for non-generative or discriminative tasks, such as classification. This is because you can describe a classification task in plain English and ... just ask the model to classify. But while this workflow is great for prototyping, you don’t want to pay prototype prices once you’re in mass production.

The popular buzz around GenAI has obscured the role of encoder-only models. These are the workhorses of practical language processing, the models that are actually being used for such workloads right now in many scientific and commercial applications.

The output of an encoder-only model is a list of numerical values (an embedding vector). You might say that instead of answering with text, an encoder model literally encodes its “answer” into this compressed, numerical form. That vector is a compressed representation of the model's input, which is why encoder-only models are sometimes referred to as representational models.

While decoder-only models (like a GPT) can do the work of an encoder-only model (like a BERT), they are hamstrung by a key constraint: since they are generative models, they are mathematically “not allowed” to “peek” at later tokens. They can only ever look backwards. This is in contrast to encoder-only models, which are trained so each token can look forwards and backwards (bi-directionally). They are built for this, and it makes them very efficient at what they do.

Basically, a frontier model like OpenAI's O1 is like a Ferrari SF-23. It’s an obvious triumph of engineering, designed to win races, and that’s why we talk about it. But it takes a special pit crew just to change the tires and you can’t buy one for yourself. In contrast, a BERT model is like a Honda Civic. It’s also an engineering triumph, but more subtly, since it is engineered to be affordable, fuel-efficient, reliable, and extremely useful. And that’s why they’re absolutely everywhere.

Another example is supervision architectures, where a cheap classifier might be used to ensure that generated text does not violate content safety requirements.

In short, whenever you see a decoder-only model in deployment, there’s a reasonable chance an encoder-only model is also part of the system. But the converse is not true.
