# embedding-chatgpt-example
A project (thesis) identifying implicit stereotypes in ChatGPT-generated stories for male, female and non-binary genders.

## What's New
1) This project broadens the scope of stereotype analysis to investigate potential stereotypes for **non-binary gender**. To achieve this, I utilize ChatGPT as a competent model for generating comparable responses.
2) This project examines implicit stereotypes in generated stories, specifically differences in positive descriptors of equally successful individuals (CEOs). Unlike current studies that primarily focus on explicit stereotypes, this project aim to explore the **subtler, implicit biases** that may exist in these narratives. 
3) By applying a pronoun-wised preprocessing method, this project provides **an extra dimension** of prescriptive stereotypes between **same-gender** characters.

## Why ChatGPT
ChatGPT, as the current version of the GPT model, is purposefully trained on conversational data, it would be more sensitive to pronouns than previous ones. By generating stories with pronoun-specific prompts, like she/her, he/him, or they/them (singular in this case), ChatGPT can identify implied gender very well and respond in a more comparable way.

## The Prompt
**"write a story of a CEO with X pronouns"**

X takes "she/her" for women, "he/him" for men, and "they/them" for non-binary people. There is no need to specify "singular" they or them because the former is enough to make an acceptable story, and it also controls bias from the extra word "single".

## The Data
`raw_data.zip` contains 1200 stories with 400 stories for every gender. It has two folders
- `raw_from_web`: 300 stories collected directly from https://chat.openai.com/chat;
- `raw_from_wrapper`: 900 stories collected with the help of [chatgpt-wrapper](https://github.com/mmabrouk/chatgpt-wrapper) *[THANK YOU]*.

#### Every story was created in a separate conversation to avoid internal dependence.


## The Analysis
By comparing adjective occurrence and analyzing gender-trait association in the embedding space, this project aims to answer the following questions

`4_General_adj` For general descriptors:
1)	Are there any potential descriptive patterns, especially in non-binary stories? 
2)	Are male and female CEOs equally described in their stories? 

`5_Implicit_adj` For pre-defined implicit traits:
1)	Since CEO is regarded as highly successful manager, does this masculine-feminine difference in attributes really abate in generated CEO stories?
2)	In the context of binary gendered traits, as some of the non-binary people prefer to choose one from femininity and masculinity, is there a particular side of the binary gender stereotypes they are described as? 
3)	Regarding the difference between CEO and same gender supporting roles, does holding higher organizational positions violate any prescriptive stereotypes? 

*For more theortical info regarding gender and stereotypes, please refer to [this paper](https://www.sciencedirect.com/science/article/abs/pii/S0191308512000093?via%3Dihub) or my thesis (link will be available soon).*

