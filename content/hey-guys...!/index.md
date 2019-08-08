---
title: "hey guys…!"
description: "In last few months i am engaged with my new passion,  NLP(Natural language processing) and text processing. in these couple of month i…"
date: "2019-08-08T19:50:12.358Z"
categories: []
published: false
---

  

hey guys…! how you doing…? i hope you liked last couple of posts from SK-learn and machine learning.

  

In last few months i am engaged with my new passion, NLP(Natural language processing) and text processing. in these couple of month i learned many interesting and mind blowing things. its really an amazing journey but at the same time i missed my computer vision a lot. any way to day i am here to share one basic and really very much important topic from NLP ecosystem.

### **word Vector** Representation**.**

If you don’t heard this terms before…! it’s ok. I will going from very beginning.

First don’t go into what is it? let me answer why is needed… for what it is needed?..

we are living in a booming era of machine learning and deep learning. we heard every day one new deep learning approch out perform all the treditional ways. also here in previous post we have made many machine learning and deep learning predictive models but almost all of the models and algortiham takes input and training data in numerical forms 1,2,3,4,………,N

We trained image classifiers(dogs v/s cats) with image data than too it is made up with pixels. 1,2,3,4,…..,N . Simply these algorithms are note good with text data. yahhh. i know as a programmer in every day we are working with strings. we are comparing string, storing string and so on. but when it comes to train an predictive or classification model with text data for example document classification. these raw textual data did’t work very well.

so, we have to do Word Vector Representation for converting text into numbers so latter on we can feed this numeric reprasantion into our machine learning model.

> Word Vector Representation -> Convert word to vectors(numbers)

let’s take one example

 **“i sent you text, please reply to my text. ”**

So first we aretokenize it and remove punctualtions so it lookes like this

**“i”, “sent”, “you”, “text”, “please”, “reply”, “to”, “my”, “text”**

now we have numbers of tokens that represent our sentence. now we can create lookup dictinory for unique words { ‘i’: 0, ‘sent’: 1, ‘you’: 3, ‘text’: 4, ‘please’: 5, ‘reply’: 6, ‘to’: 7, “my”: 8} so we have 9 unique tokens in our sentence. and “i”can be represent as “0", “sent” can be “1” and so on. Count doesn’t matter; order doesn’t matter. Each token just needs a unique identifier. yes now you learned word vector representation. let dig more into it.

### **Traditional Method — Bag of Words Model**

Bag of Words uses one hot encoding, Each word in the vocabulary is represented by one bit position in a huge vector. For example, if we have a vocabulary of 500 words, and “text” is the 4th word in the dictionary, it would be represented by: 0 0 0 1 0 0 . . . . . . . 0 0 0 0.
