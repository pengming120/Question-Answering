# Question-Answering

A general question-answering system would be able to answer a question about any domain, based on the world knowledge. This system would consist of three stages. A given question is read and reformulated in the first stage, followed by information retrieval via a search engine. An answer is then synthesized based on the query and a set of retrieved documents.

The **SearchQA** is a retrieval-based question-answer task challenge. This task provides questions and answers from Jeopardy! (An American TV show), as well as snippets of web pages from Google search. You need to use the data to train a model that provides answers to the given questions and search result snippets. The following is an example of instance.

---

**Question:** born poland , first prime minister israel\
**Answer:** ben gurion\
**Snippets:**

- \<s> shimon peres' family 5 fast facts need know heavy com sep 27 , 2016 six decades 
public life click learn former israeli prime minister 's family born august 21 , 1923 
vishnyeva , poland time part belarus according academy \</s>

- \<s> 16 day history read happened today short display day gr daily infobits website , 
favorite first polish pope reigned pope 26 years prime minister israel , david ben 
gurion , born plonsk , poland \</s>

- \<s> shimon peres wikipedia shimon peres israeli statesman ninth president israel , 
serving 2007 2014 peres served twice prime minister israel twice interim prime minister , 
peres told rabbi menachem mendel schneerson born result blessing parents \</s>

- \<s> israel palestine google books result \</s> 

---
It is worth noting that not all the search result snippets in this task contain answers. Therefore, you need to consider how to employ a model to pick out the snippets that can answer the question and retrieve the most appropriate answer spans. Each question has approximately 40 corresponding snippets. There is no question that cannot be answered. All text in the data is in lowercase.

---
Dataset: https://drive.google.com/drive/folders/1xfkW8RSbwrwBnJ6t7c2RZW-Eh4JvE5Bd?usp=sharing
