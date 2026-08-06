# Discussion on key themes identified via probing exercises

## No clear winner emerges as the most performant LLM in Sinhala for the select set of tasks

This set of experiments use ChatGPT, Claude, and DeepSeek via the publicly available web interfaces to investigate model perforamance in Sinhala. For the selected set of tasks and the use case of using LLMs for everyday tasks of nonexpert users, no clear winner emerges as the most performant LLM. There is variability in model performance across different queries and 
different type of task, but any one model did not produce outstanding results within the scope of these experiments.

## The challenge of diglossia - the models' perform better at generating formal Sinhala text, but does poorly on informal text

Sinhala is a diglossic langauge, where there is a high variety of the language used for formal and written use, and a low variety of the language used in informal settings. The set of tasks used were set to include both instances of language usage. A snapshot of the tasks and the type of variety expected is below:

Text generation:
[A Facebook post to advertise a clothing business](text-gen-1.txt) - Informal
[A cover letter for a job application](text-gen-2.txt) - Formal
[A letter to the bank](text-gen-3.txt) - Formal
[A public notice for a blood donation compaign](text-gen-4.txt) - Formal
[A Facebook post for a voluntary cleaning programme](text-gen-5.txt) - Informal

Translation:
[A newspaper article on psychological safety at work](translation-1.txt) - Informal and conversational
[A road closure notice](translation-2.txt) - Formal
[A newspaper article on mindfulness and other related concepts](translation-3.txt) - Could be translated formally, but the original article has elements of conversational style
[A newspaper article on introducing property taxes](translation-4.txt) - Formal
[A newspaper article regarding a warning by the health ministry](translation-5.txt) - Formal

Information retrieval:

[Information on registering a new vehicle](retreival-1.txt) - Informal
[Information on getting a national identity card](retrieval-2.txt) - Informal
[Information on getting a new electricity connection](retrieval-3.txt) - Informal
[Information on taxes](text-gen-4.txt) - Informal
[Information on getting street lamps](text-gen-5.txt) - Informal

The models reponded suitably well in generating formal responses. However, the informal language sounded superficial and formulaic, often times not sounding like human speech. 

## The problems in information retrieval also reveal the limitation in the underlying information space  

The tests aim to retrieve information on a variety of topics, each with a different level of information publicly available.

In the [query to retrieve information on taxes that apply when importing business samples](retrieval-4.txt), all three models answered the question with accurate information. This information was available in the Sri Lanka Customs [Online Buyers Import & Duty Guide webpage](https://www.customs.gov.lk/personal/online-buyers/) and as a frequently anwered question in the [Frequently Asked Questions webpage](https://www.customs.gov.lk/personal/faq/).

In the [query to retrieve information on getting street lamps](retrieval-5.txt), there was no publicly available information regarding the process. The three models provided different answers, sometimes converging on points such as speaking to the local Member of Parliament or speaking to other relevant local authorities. 

The above two represent two ends of the spectrum observed. On one end, the models retrieved a very specific piece of information accurately, where this information was precisely provided in the source of truth. 
On the other end, there was no relevant information publicly available, and the required answer was not a precise one, so the models generated arbitrary information. 

In the [query to retrieve information about the process to apply for a national identity card](retrieval-2.txt) the relevant information is available publicly, but all three models provided answeres with predominantly incorrect answers.