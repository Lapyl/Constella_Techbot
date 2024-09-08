# Constella_Techbot

Chatbot trained with technical documents of Constellation Network

## Inspiration

ChatGTPT’s outstanding performance in Generative Artificial Intelligence has captured the whole world's attention. Many companies are now deploying chatbots on their websites to improve and simplify their customer support and online marketing. We felt that Constellation Network would greatly benefit by using a reliable chatbot on their website.

Except for limited and occasional use, ChatGPT costs money. Microsoft has now released a mobile app called Copilot, with which a smartphone can use ChatGPT without having to pay. Problem with ChatGPT is that it generally fails to answer questions specifically pertaining to Constellation Network. We felt that Constellation Network would need a chatbot with a model specially trained with its own technical and other documents.

## What it does

Our website at lipy.site demonstrates two possible options for a chatbot. The left side of the the home page has a chatbot using our Llama based model. The right side has a chatbot as provided by Botpress. Visitor may ask questions to any of these two chatbots.

Unlike the Botpress chatbot, the Llama chatbot is too slow to respond, and may even fail. Good thing about the Llama chatbot is that it can be cheaper and more customizable.

## How we built it

There are many products and services for training a model with a set of specialized information. One option to control the cost of a chatbot is to train a model using an open-source base model. Another option is to use a reliable and affordable provider for model-training and hosting. We found that for an open-source base model, Meta’s Llama model is quite good, and for a a model-training and hosting provider, Botpress company is quite good.

We downloaded Constellation Network’s GitHub repository of technical documents. From there, we took .md files of markdown texts. We converted them into .txt files by using an Excel macro.

For the Llama option, we built a trained model by using Python, jupyter notebook, necessary Python packages, a good Llama model, and the .txt files. We built a node.js application, which acts as a chatbot in the front-end and uses our trained model in the back-end. We ported this node.js application as a website at our lipy.site domain.

For the Botpress option, we logged into our Botpress account. We created a new chatbot that uses ChatGPT, Anthropic, and a few other products. We fed it with our .txt files. Botpress came out with a trained chatbot. We published this trained chatbot. Botpress gave us an embeddable link of this chatbot. We added that embeddable link into our website.

## Challenges we ran into

To avoid costs of cloud computing, we built our Llama based model by using our own computer. We encountered numerous hurdles, mainly related to compatibilities of version of Python and various packages. Other minor projects were regarding nicely arranging the two chatbots on our website.

## Accomplishments that we're proud of

We learned a lot of things while doing this project.

## What we learned

At Hugging Face, we came across many open-source Natural Language Processing models. While building our model, we understood the applicability and evolution of many Python packages. Selecting a chatbot provider sharpened our skills of purchasing.

## What's next for Constella Techbot

We will train our Llama based and Botpress provided models with more documents to make these chatbots look more promising. We will find some ways and means of making our Llama based chatbot  quicker and more responsive.
