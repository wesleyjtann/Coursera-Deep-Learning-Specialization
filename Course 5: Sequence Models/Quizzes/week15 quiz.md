### Week 15 Quiz - Natural Language Processing & Word Embeddings

1. Question 1
Suppose you learn a word embedding for a vocabulary of 10000 words. Then the embedding vectors should be 10000 dimensional, so as to capture the full range of variation and meaning in those words.

	[x] False

2. Question 2 
What is t-SNE?

	[x] A non-linear dimensionality reduction technique

3. Question 3
Suppose you download a pre-trained word embedding which has been trained on a huge corpus of text. You then use this word embedding to train an RNN for a language task of recognizing if someone is happy from a short snippet of text, using a small training set.

x (input text)					y (happy?)
I'm feeling wonderful today!	1
I'm bummed my cat is ill.		0
Really enjoying this!			1

Then even if the word “ecstatic” does not appear in your small training set, your RNN might reasonably be expected to recognize “I’m ecstatic” as deserving a label y=1y = 1y=1.

	[x] True

4. Question 4
Which of these equations do you think should hold for a good word embedding? (Check all that apply)

	[x] `e_boy−e_girl ≈ e_brother−e_sister`
	[x] `e_boy​−e_brother​ ≈ e_girl​−e_sister​`

5. Question 5  
Let E be an embedding matrix, and let $o_{1234}$​ be a one-hot vector corresponding to word 1234. Then to get the embedding of word 1234, why don’t we call $E * o_{1234}$ in Python?
	
	[x] It is computationally wasteful.

6. Question 6    
When learning word embeddings, we create an artificial task of estimating $P(target \mid context)$. It is okay if we do poorly on this artificial prediction task; the more important by-product of this task is that we learn a useful set of word embeddings. 
	
	[x] True

7. Question 7    
n the word2vec algorithm, you estimate $P(t \mid c)$, where $t$ is the target word and $c$ is a context word. How are $t$ and $c$ chosen from the training set? Pick the best answer.

	[x] c and t are chosen to be nearby words.

8. Question 8    
Suppose you have a 10000 word vocabulary, and are learning 500-dimensional word embeddings. The word2vec model uses the following softmax function:

`P(t∣c)=eθtTec∑t′=110000eθt′Tec`

Which of these statements are correct? Check all that apply.

	[x] θ_t​ and e_c​ are both 500 dimensional vectors. 
	[x] θt_​ and e_c​ are both trained with an optimization algorithm such as Adam or gradient descent. 

9. Question 9 
Suppose you have a 10000 word vocabulary, and are learning 500-dimensional word embeddings.The GloVe model minimizes this objective:

`min∑i=110,000∑j=110,000f(Xij)(θiTej+bi+bj′−logXij)2`

Which of these statements are correct? Check all that apply.

	[x] $θ_i$​ and $e_j$​ should be initialized randomly at the beginning of training. 
	[x] $X_{ij}$​ is the number of times word i appears in the context of word j.
	[x] The weighting function f(.) must satisfy f(0)=0. 


10. Question 10    
You have trained word embeddings using a text dataset of m1m_1m1​ words. You are considering using these word embeddings for a language task, for which you have a separate labeled dataset of m2m_2m2​ words. Keeping in mind that using word embeddings is a form of transfer learning, under which of these circumstance would you expect the word embeddings to be helpful?

	[x] m_1​ >> m_2