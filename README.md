# Analysis of Factors Affecting Student Satisfaction

## How Did the Idea Come About?

I spent quite a long time choosing the topic for this research. The assignment seemed genuinely interesting to me, so I really did not want to choose an overused topic like: “Will water in a glass become colder if you put ice in it?” And, of course, I did not want to artificially inflate the survey results either.

The idea came from a completely unexpected conversation. While talking to an acquaintance of mine from Perm State University, I heard the phrase: “All third-year students hate their university.” At that moment, I became curious: do students from top universities feel the same way?

On the one hand, the obvious answer would be: “Of course they do. They are students just like us, and they can also be dissatisfied with their university.” But on the other hand, a question arises: why would they dislike it if the quality of education is higher, there are more opportunities, and a professor is unlikely to grade a programming lab assignment based on how nice the console output looks, whether the presentation has speaker notes, or, even worse, how their favorite hockey team played.

That is how the hypothesis appeared: **a university’s ranking affects student satisfaction**. I am Connor, and I am going to check how it actually works.

## Searching for a Ranking of Russian Universities

At first, I thought that the most difficult stage would be data collection, because it requires time, people, and patience. In practice, however, the hardest part turned out to be finding a suitable source with university rankings. I considered several options.

1. **The Ministry of Science and Higher Education of the Russian Federation**  
   <https://minobrnauki.gov.ru/%D0%BE%D0%B1%D1%89%D0%B8%D0%B8%CC%86.pdf>  
   This is a reliable source, but the data did not seem entirely realistic to me. Let us be honest: if Ural Federal University and Perm State University were truly among the best universities in Russia, olympiad students would probably talk about them more often. Therefore, the evaluation criteria used in this source did not suit my research.

2. **Tabiturient**  
   <https://tabiturient.ru/globalrating/>  
   This source did not seem the most official one, but it contains information on a large number of universities, and the data looks more or less realistic.

3. **RAEX**  
   <https://raex-rr.com/education/russian_universities/top-100_universities/2025/>  
   This ranking looks quite convincing, but it includes only 100 universities.

4. **Forbes**  
   <https://www.forbes.ru/education/558029-lucsie-rossijskie-vuzy-2026-rejting-forbes>  
   The situation is similar to RAEX: the ranking looks credible, but it does not cover all the universities included in my sample.

Rankings from different websites differ noticeably. Formally, it would have been more logical to use data from an official source, but those results did not fully match public perception. Therefore, I chose **Tabiturient** as the main source, since it contained information on all universities included in the study.

Yes, these data may not be perfectly accurate, but this is not critical for this particular research. What mattered more to me was not the exact position of a university in the ranking, but the possible relationship between the ranking and students’ evaluations.

## Data Collection

At this stage, I had to use almost all the connections I had. I am very grateful to my friends who helped me share the survey and collect responses.

I consider the obtained data reliable enough for an educational research project. The sample was intentional: many of the respondents were olympiad students, high-achieving students, and simply active students from different universities. As a result, the answers were not random responses “from nowhere”, but opinions from people who could consciously evaluate their university and their learning experience.

The survey included the following questions:

1. Which university do you study at?
2. What year of study are you in?
3. What is your mode of study?
4. How old are you?
5. To what extent did the university’s ranking influence your choice when applying?
6. Do you think your university’s ranking reflects the actual quality of education?
7. Do you feel proud to study at your university, considering its reputation and ranking?
8. How satisfied are you overall with studying at your university?
9. Please evaluate your satisfaction with the following aspects of university education: quality of teaching, curriculum content, facilities and equipment, and organization of the educational process.
10. To what extent does the university support your interests and initiatives, such as sports, student projects, creativity, research activities, and other forms of self-realization?
11. How satisfied are you with the way your university makes student life more interesting and diverse?
12. How satisfied are you with your decision to choose this particular university?

## Survey Results

### Average Values for Each University

There were two unreliable responses in the survey results: **213**, which was most likely a typo, and **42**, which was probably someone deliberately trying to spoil the data. I corrected these values manually, since there were only 69 responses in total.

Principal component analysis (PCA) was applied to combine several survey questions into a single generalized indicator. These questions reflected students’ satisfaction with their studies, the quality of teaching, the organization of the educational process, and the overall student life experience.

The table below shows the average values for each university, together with its ranking and the calculated PCA-based satisfaction score.

| № | university | course | age | q4_rating_choice | q5_rating_quality | q6_pride | q11_choice | university_rating | PCA_7_10 |
|---:|---|---:|---:|---:|---:|---:|---:|---:|---:|
| 1 | БГМУ | 5.00 | 26.50 | 1.00 | 2.00 | 2.50 | 2.50 | 119 | -3.17080662 |
| 2 | БГПУ | 3.00 | 21.00 | 1.00 | 1.00 | 1.00 | 1.00 | 136 | -4.94044884 |
| 3 | БашГАУ | 4.00 | 21.00 | 1.67 | 2.67 | 4.33 | 4.67 | 237 | 0.06015573 |
| 4 | ВШЭ | 2.50 | 20.50 | 2.00 | 3.00 | 2.00 | 4.50 | 2 | 2.72087838 |
| 5 | ИТМО | 3.00 | 20.00 | 4.00 | 3.00 | 3.00 | 5.00 | 7 | 2.65920569 |
| 6 | Ижевский ГМУ | 3.00 | 20.67 | 1.67 | 3.00 | 3.00 | 3.67 | 125 | 1.15300449 |
| 7 | КГЭУ | 2.00 | 19.25 | 3.00 | 3.00 | 3.50 | 4.00 | 81 | 1.42640519 |
| 8 | КФУ | 2.60 | 20.20 | 3.60 | 2.80 | 3.00 | 3.60 | 54 | -1.70326050 |
| 9 | МГУ | 2.33 | 20.00 | 4.33 | 4.33 | 4.00 | 5.00 | 11 | 2.51661190 |
| 10 | МГЮА | 3.00 | 20.33 | 4.00 | 4.33 | 4.00 | 4.67 | 12 | 0.50558458 |
| 11 | МИИГАиК | 4.00 | 20.00 | 4.00 | 5.00 | 5.00 | 5.00 | 102 | 2.45352622 |
| 12 | МИСИС | 1.00 | 18.00 | 4.00 | 3.50 | 4.00 | 3.00 | 68 | -0.82079189 |
| 13 | МИФИ | 3.60 | 21.00 | 4.20 | 2.60 | 2.60 | 3.20 | 5 | -1.55240823 |
| 14 | МТУСИ | 3.00 | 20.00 | 2.00 | 2.00 | 4.00 | 5.00 | 35 | 2.07642182 |
| 15 | МФТИ | 4.00 | 22.00 | 5.00 | 4.50 | 4.50 | 4.50 | 1 | 2.03358010 |
| 16 | НИУ ВШЭ-Пермь | 3.00 | 21.00 | 3.50 | 3.00 | 2.00 | 3.50 | 65 | -1.09329915 |
| 17 | ПГМУ | 2.00 | 19.00 | 3.25 | 3.50 | 3.75 | 4.50 | 115 | 1.13399468 |
| 18 | ПГНИУ | 3.00 | 20.00 | 2.00 | 1.00 | 1.00 | 1.00 | 180 | -3.59803552 |
| 19 | РАНХиГС | 1.00 | 18.00 | 3.00 | 3.00 | 1.00 | 5.00 | 13 | -1.09152734 |
| 20 | УГНТУ | 3.00 | 20.33 | 3.33 | 2.33 | 3.00 | 3.33 | 116 | -0.16558105 |
| 21 | УРГЮУ | 3.00 | 20.00 | 5.00 | 5.00 | 5.00 | 5.00 | 31 | 0.04019275 |
| 22 | УУНиТ | 3.43 | 20.43 | 2.00 | 2.86 | 2.29 | 2.86 | 167 | -1.59459022 |
| 23 | УрГАУ | 3.00 | 21.38 | 1.75 | 3.12 | 3.12 | 4.00 | 376 | 1.29797303 |
| 24 | ЮУрГУ | 2.33 | 19.67 | 1.67 | 3.67 | 2.33 | 3.67 | 181 | -0.34678522 |

After calculating the average values, it can be observed that students from universities with a stronger reputation were more likely to consider university rankings when applying.

The most satisfied students study at HSE, ITMO, and Moscow State University, whose ranking positions are 2, 7, and 11 respectively. In contrast, the least satisfied students study at Bashkir State Pedagogical University, Perm State University, and Bashkir State Medical University, with ranking positions of 136, 180, and 119.

### Determining the Impact of University Ranking on Other Parameters

The correlation analysis showed that the university ranking does not have a significant relationship with any of the analyzed parameters: the influence of ranking on university choice, pride in the university, overall satisfaction with the university, and satisfaction with choosing this particular university.

It was also found that the year of study and student satisfaction are not meaningfully related to each other.

### Determining the Most Significant Factor Affecting Student Satisfaction

I conducted a correlation analysis and built a model to determine which factors influence overall student satisfaction with university education. During the modeling process, I gradually removed insignificant factors one by one, starting with the factor that had the highest `Pr > 0.05`.

As a result, only two statistically significant factors remained: the organization of the educational process and an active, diverse student life. This result was somewhat unexpected, but it can be explained: students’ satisfaction appears to depend not only on the academic quality of the university, but also on how well the learning process is organized and how engaging university life feels outside the classroom.

### Cluster Analysis

As a result, three clusters of universities were identified. These clusters represent groups of universities that are similar to each other based on students’ evaluations. The cluster number does not indicate a position in the ranking: Cluster 1 is not necessarily better than Cluster 2 or Cluster 3. It is simply the number assigned to the group.

1. **Cluster 1:** ITMO, MSU, MSAL, MIIGAiK, MISIS, MIPT, USLU.
2. **Cluster 2:** BSMU, BSPU, KFU, MEPhI, HSE Perm, Perm State University, RANEPA, UUST.
3. **Cluster 3:** Bashkir State Agrarian University, HSE, Izhevsk State Medical Academy, KSPEU, MTUCI, PSMU, USPTU, Ural State Agrarian University, SUSU.

To describe the clusters, let us consider which factors have the greatest importance within each of them.

| Cluster | Count | q4_rating_choice | q6_pride | PCA_7_10 | q11_choice | university_rating |
|---:|---:|---:|---:|---:|---:|---:|
| 1 | 7 | 4.33 | 4.21 | 1.34 | 4.60 | 33.1 |
| 2 | 8 | 2.54 | 1.92 | -2.34 | 2.83 | 92.4 |
| 3 | 9 | 2.26 | 3.23 | 1.04 | 4.15 | 141.0 |

Cluster 1 includes universities with the highest values for `q4_rating_choice`, `q6_pride`, `PCA_7_10`, and `q11_choice`. These universities also have the best average ranking position. This means that students in this cluster were more likely to consider the university ranking when applying, feel proud of their university, and evaluate both their education and student life positively.

Cluster 2 is characterized by the lowest values of student satisfaction. It has the lowest `PCA_7_10` score, the lowest level of pride in the university, and the lowest satisfaction with university choice. Therefore, this cluster can be described as a group of universities where students are generally less satisfied with their educational experience.

Cluster 3 includes universities where the ranking had the least influence on students’ choice. However, students in this cluster still show relatively high levels of pride, satisfaction, and positive evaluation of student life. This suggests that even though these universities have lower ranking positions on average, students may still be satisfied with their university experience for reasons not directly related to ranking.

### Identifying the Best Universities by Overall Score

The highest `total_score` values were obtained by MIIGAiK, MIPT, MSU, USLU, and ITMO. This indicates that students from these universities, on average, rate their choice more highly, feel more pride in their university, and demonstrate a higher overall level of satisfaction.

Middle positions are occupied by universities where some individual indicators are relatively high, but the overall level of satisfaction or the influence of ranking is less pronounced. The lowest positions are taken by universities with lower `total_score` values, which is associated with negative `PCA_7_10` values and lower scores for pride in the university or satisfaction with choosing it.

| University | Total score |
|---|---:|
| МИИГАиК | 16.4 |
| МФТИ | 16.0 |
| МГУ | 15.8 |
| УРГЮУ | 15.0 |
| ИТМО | 14.7 |
| МГЮА | 13.2 |
| МТУСИ | 13.1 |
| ПГМУ | 12.6 |
| КГЭУ | 11.9 |
| ВШЭ | 11.2 |
| БашГАУ | 10.7 |
| МИСИС | 10.2 |
| УрГАУ | 10.2 |
| Ижевский ГМУ | 9.49 |
| УГНТУ | 9.49 |
| КФУ | 8.50 |
| МИФИ | 8.45 |
| НИУ ВШЭ-Пермь | 7.91 |
| РАНХиГС | 7.91 |
| ЮУрГУ | 7.32 |
| УУНиТ | 5.56 |
| БГМУ | 2.83 |
| ПГНИУ | 0.40 |
| БГПУ | -1.94 |

## Conclusion

In this study, I tested the hypothesis that a university’s ranking affects student satisfaction. To do this, I collected responses from students of different universities, calculated average values for each university, created a generalized satisfaction indicator using principal component analysis, and conducted a correlation analysis.

The results showed that the hypothesis was only partially confirmed. University ranking can indeed play a role in the choice of university, especially for students who initially focus on prestige. However, ranking alone does not guarantee high satisfaction with education. A student may study at a highly ranked university and still be dissatisfied with the organization of the learning process, teaching quality, or student life. On the other hand, a university may not occupy a top position in the rankings but still provide students with a supportive environment and a feeling that they made the right choice.

Although the hypothesis was not fully confirmed — which is honestly disappointing, and I still feel that the dataset was not large enough and the study should be repeated with more data — the research still led to an important conclusion. To make students truly satisfied, universities should not focus only on rankings and formal indicators. They should also create a lively student environment, support students’ initiatives, and help them find friends and a sense of belonging.

After all, suffering through lab assignments is much more pleasant when you are not doing it alone. In other words, we were looking for copper, but found gold.
