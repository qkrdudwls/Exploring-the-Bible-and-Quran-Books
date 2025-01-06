# Exploring the Bible and Quran Books

## Datasets Used 
- [The King James Version of the Bible](https://www.gutenberg.org/ebooks/10)
- [The Koran (Al-Qur'an) by J. M. Rodwell and G. Margoliouth](https://www.gutenberg.org/ebooks/2800)

## Background

Christianity and Islam are the two largest religions in the world, with 2.8 billion and 1.9 billion followers, respectively. Both religions are considered Abrahamic and are monotheistic, originating from the Middle East. However, they have experienced moments of conflict and opposition through historical events such as the Battle of Yarmouk in 636, the Crusades from 1095 to 1291, the Battle of Vienna in 1683, and the terrorism by al-Qaeda and the Taliban. Despite these historical conflicts and opposition, both Christianity and Islam share the common goal of answering universal questions about human life, and their scriptures, the Bible and the Quran, are at the heart of their faith and teachings. The Bible and the Quran play a crucial role as texts that provide guidance for life, establish moral norms, and form the foundation of faith for their respective followers.

This project starts with an attempt to objectively compare the similarities and differences between the Bible and the Quran through text analysis, focusing on the data itself rather than interpretation of the text. The goal is to clarify the common messages and moral values conveyed by the two scriptures, analyze the structure and linguistic features of the texts in a data-driven manner, and uncover the moral values and messages that both scriptures aim to convey.

## Goal

This project aims to calculate the similarity between the Bible and the Quran through objective, data-driven comparison, excluding subjective religious perspectives, and to derive commonalities and differences. Various text mining techniques will be utilized to analyze the structural and content-related characteristics of both scriptures, and multiple similarity measurement methods will be applied to perform a quantitative comparison.

## Data Mining Methods and Algorithms Used

1. TF-IDF
2. Shingling
3. Min-Hashing
4. Locality Sensitive Hashing
5. TextRank

## Evaluation Criteria

1. Cosine Similarity
2. Jaccard Similarity
3. Hash Collisions

## Results

### Analysis of Word Importance Using TF-IDF

#### Bible

Applying TF-IDF to the Bible's text data, words like "lord" and "god," referring to deities, were found to be mentioned the most. Additionally, the word "said" indicates that dialogue or speech is an important element in the Bible. Words such as "son," "israel," "king," "land," "man," and "children" also played a significant role, suggesting that the Bible contains abundant references to historical events and figures, as well as detailed descriptions of places and governance.

#### Quran

In the case of the Quran, similar to the Bible, the highest TF-IDF scores were found for words like "god," "lord," and "said," indicating that God is central. The Quran also addresses various themes through words related to faith and reverence, such as "believe" and "fear," nature and creation, such as "earth" and "created," as well as certainty in truth and knowledge, such as "verily" and "truth." Compared to the Bible, the Quran emphasizes the Day of Judgment and the end times more frequently, using words like "day," "fear," and "verily," while also focusing on the essence of faith and inner reflection of humanity through words like "believe," "truth," and "signs."

#### Common Words

By analyzing the common words between the Bible and the Quran, it is evident that the shared terms focus on the relationship between God (‘god,’ ‘lord’) and humans (‘man,’ ‘children’), emphasizing the guidance humans are given to follow God's teachings and the importance of the Day of Judgment or salvation. Additionally, the message is conveyed through the words of the prophets or God’s speech (‘said’), while themes such as nature (‘earth’) and warnings (‘fear,’ ‘fire’) highlight that God creates and controls the world.

### Similarity Analysis Between the Bible and the Quran

#### Similarity Calculation

The cosine and Jaccard similarities between the text data of the Bible and the Quran were calculated as approximately 0.934 and 0.226, respectively. When Shingling was applied, the cosine similarity between the shingles was about 0.799, and the Jaccard similarity was around 0.665. After applying Min-Hashing, the similarity between the minhashes was calculated as approximately 0.675. The cosine similarity shows that the Bible and the Quran overall cover very similar themes, while the Jaccard similarity reveals that the proportion of common vocabulary at the word level is low. After applying Shingling, the cosine similarity decreased, while the Jaccard similarity increased significantly, indicating that breaking the text into smaller units allowed contextual differences to be reflected more precisely. When Min-Hashing was applied, the value of hash collisions was 0, and the similarity value of approximately 0.675 suggests that the Bible and the Quran share structural similarities.

#### Most Similar Document Pair

Using Locality Sensitive Hashing (LSH), the most similar document pair between the Bible and the Quran was found to be Chapter 33 of the Bible and Chapter 40 of the Quran. Both chapters share common themes, including the concepts of God's judgment, restoration, and forgiveness, with a particular focus on the message of redemption. Although the texts are expressed differently, they both ultimately discuss human sin, redemption, and restoration centered on God's justice and mercy. Therefore, the primary concepts and themes align, and the documents contain many similar sentences with comparable words, which led to them being identified as the most similar document pair.

### Similarity Analysis Using TextRank

#### Similarity Calculation

The TextRank algorithm was applied to the text data of the Bible and the Quran to generate summaries. The cosine similarity was calculated as approximately 0.954, and the Jaccard similarity was approximately 0.23. After applying Shingling, the cosine similarity was about 0.796, and the Jaccard similarity was around 0.659. When Min-Hashing was applied, the value of hash collisions was 0, and the similarity between minhashes was calculated as approximately 0.62. After applying TextRank, the cosine and Jaccard similarities for the entire data slightly increased, while the similarities for Shingling and Min-Hashing decreased. This indicates that while TextRank made the core thematic similarities between the Bible and the Quran clearer, the summarization process reduced contextual diversity.

#### Most Similar Document Pair

After applying TextRank and using LSH to find the most similar document pair, the summary of Chapter 45 of the Bible and Chapter 39 of the Quran were identified as the most similar document pair. Both documents deal with the theme of a shift in action or the delivery of a message, and the core keywords appear simultaneously, making them structurally and contextually similar. Compared to before applying TextRank, there is a tendency for the similarity to decrease. This is because TextRank more carefully considers the semantic connections and context between sentences, reflecting both structural and semantic differences more precisely.

## Conclusion

This project analyzed two major religious texts, the Bible and the Quran, using various data mining techniques to compare their linguistic, literary, and structural characteristics, drawing out similarities and differences. After preparing the text data for data-driven analysis through crawling and preprocessing, TF-IDF was used to identify the key words and characteristics of both texts, TextRank was applied to extract key sentences, and similarity was calculated using techniques such as Shingling, Min-Hashing, and LSH.
The Bible and the Quran show high thematic similarity but significant differences in the words used and their expressions. Through TextRank and LSH, the key themes and sentences of each text were extracted. Both the Bible and the Quran share common themes such as love and forgiveness. However, the Bible is characterized by sentences built around descriptive and narrative themes, while the Quran is structured with sentences centered on imperative and normative themes.
