---
{"dg-publish":true,"permalink":"/ki/intelligence-tests/final-test-ai-intelligence/"}
---


zurück zu [[PKM/Computer-Science/conda-commands\|conda-commands]]


#### Reasoning

**Imagine you are participating in a race with a group of people. If you have just overtaken the second person, what's your current position? Where is the person you just overtook?**
You are in second place

**If the second person is changed to last person in the above question, what would the answer be?**
logically impossible

*mtb_101* - *einfache Frage, sollten alle schaffen* - *schafft nur gpt-4*

---

**Thomas is very healthy, but he has to go to the hospital every day. What could be the reasons?**
Thomas may work at a hospital

**Can you explain why the above question is interesting?**
Wurde die Logik hinter Logik erkannt?

*mtb_102* - *Große Modelle schaffen es, kleinere nicht. Mittlere vielleicht* - *sollte auch recht einfach sein*

---

**Read the below passage carefully and answer the questions with an explanation: At a small company, parking spaces are reserved for the top executives: CEO, president, vice president, secretary, and treasurer with the spaces lined up in that order. The parking lot guard can tell at a glance if the cars are parked correctly by looking at the color of the cars. The cars are yellow, green, purple, red, and blue, and the executives’ names are Alice, Bert, Cheryl, David, and Enid.**
**- The car in the first space is red.**
**- A blue car is parked between the red car and the green car.**
**- The car in the last space is purple.**
**- The secretary drives a yellow car.**
**- Alice’s car is parked next to David’s.**
**- Enid drives a green car.**
**- Bert’s car is parked between Cheryl’s and Enid’s.**
**- David’s car is parked in the last space. Question: What is the name of the secretary?**
The secretary is Alice
| ceo | pres | v-p | sec | treas |
| rot | blau | grün| yell | purp |
|cheryl|bert | enid | alice| david |

**List car colors in order from last to first**
The car colors in order from last to first are: purple, yellow, green, blue, red

*mtb_105* - *CAVE Fehler in den Daten. macht sogar gpt-4 falsch, aber interessanterweise Vicuna-13B richtig (vlt auch gpt4all-13b-snoozy?)* - *schafft KEIN modell bisher*

**Lies den folgenden Text aufmerksam durch und beantworte die Fragen mit einer Erklärung: In einem kleinen Unternehmen sind die Parkplätze für die leitenden Angestellten reserviert: CEO, Präsident, Vizepräsident, Sekretär und Schatzmeister, wobei die Parkplätze in dieser Reihenfolge aufgereiht sind. Der Parkplatzwächter kann auf einen Blick erkennen, ob die Autos richtig geparkt sind, indem er auf die Farbe der Autos achtet. Die Autos sind gelb, grün, lila, rot und blau, und die Namen der Führungskräfte lauten Alice, Bert, Cheryl, David und Enid.**
**- Das Auto auf dem ersten Platz ist rot.**
**- Ein blaues Auto ist zwischen dem roten und dem grünen Auto geparkt.**
**- Das Auto auf dem letzten Platz ist lila.**
**- Die Sekretärin fährt ein gelbes Auto.**
**- Das Auto von Alice ist neben dem von David geparkt.**
**- Enid fährt ein grünes Auto.**
**- Berts Auto ist zwischen dem von Cheryl und Enid geparkt.**
**- Davids Auto ist auf dem letzten Platz geparkt. Frage: Wie heißt die Sekretärin?**

---

**Which word does not belong with the others? tire, steering wheel, car, engine**
Car does not belong because all others are components of a car

**Could you replace it with a word that belongs with the others?**
Wurde Logik wirklich erkannt?

*mtb_108* - *schafft nur gpt-4. in meinem test such llama2 70b hf* - *nur gpt-4*

---

**Each problem consists of three statements. Based on the first two statements, the third statement may be true, false, or uncertain.**
**1. Oranges cost more than apples.**
**2. Oranges cost less than bananas.**
**3. Bananas cost more than apples and bananas cost more than orange. If the first two statements are true, then the third statement is**
true

**If the third statement is true. Is the first statement true, false, or uncertain? Please explain.**
uncertain

*mtb_106* - *schaffen nur gpt-4, claude-v1* - *in meinem test schafft's auch monika-7b-q5_1*

---

**A is the father of B. B is the father of C. What is the relationship between A and C?**
A is the grandfather of C.

**Building on the previous question, if C is the son of D, D is the father of E, E is the son of X, and X is the father of Y, and Y is the father of Z, what’s the relationship between A and Z in terms of generations and also the familial relationship in words?**
A is three generations above Z

*mtb_107* - *Alle gängigen Modellen richtig, außer llama2-7B.. strange mit Ergebnis(SEN) von follow up Fragen*

---

**One morning after sunrise, Suresh was standing facing a pole. The shadow of the pole fell exactly to his right. Can you tell me the direction towards which the shadow was pointing - east, south, west, or north? Explain your reasoning steps.**
West

**To which direction was Suresh facing? How do you solve this?**
CAVE Im Original steht South, aber ich denke es sollte North oder East sein

*mtb_107* - *CAVE Fehler in den Daten*

---

#### Math

**The vertices of a triangle are at points (0, 0), (-1, 1), and (3, 3). What is the area of the triangle?**
Area is 3

**What’s area of the circle circumscribing the triangle?**
5pi

*mtb_111* - *schafft nur gpt-4* -

---

**A tech startup invests $8000 in software development in the first year, and then invests half of that amount in software development in the second year. What’s the total amount the startup invested in software development over the two years?**
12.000

**If the startup maintains the same strategy for the third year, investing half of the previous year’s amount into software development, how much will they invest in the third year?**
2.000

*mtb_112* - *sollte für die meisten modelle recht einfach sein, auch 7B* -

---

**In a survey conducted at a local high school, preferences for a new school color were measured: 58% of students liked the color blue, 45% preferred green, and 22% liked both colors. If we randomly pick a student from the school, what’s the probability that they would like neither blue nor green?**
19%

**If we select a student liked green, what’s the probability that he or she would dislike both colors?**
2%

*mtb_113* - *schafft nur gpt-3.5, gpt-4 und claude* -

---

**When rolling two dice, what is the probability that you roll a total number that is at least 3?**
36 (all cases) - 0 (sum equals 1) - 1 (sum equals 2) = 35, so the probability is 35/36

**Continue from previous question. What’s the probability that you roll a number which is even or at least 3?**
100%

*mtb_114* - *schafft NUR gpt-4* -

---

**Benjamin went to a bookstore and purchased a variety of books. He bought 5 copies of a sci-fi novel, each priced at $20, 3 copies of a history book priced at $30 each, and 2 copies of a philosophy book for $45 each. What was the total cost of his purchases?**
280

**Suppose Benjamin decides to sell each of these books at a 25% markup from the price he purchased them. What would be his total revenue if he sold all the books he bought?**
350

*mtb_119* - *Von 7B Modellen schafft es nur Llama2. Gute 7B Frage* -

---

**Some people got on a bus at the terminal. At the first bus stop, half of the people got down and 4 more people got in. Then at the second bus stop, 6 people got down and 8 more got in. If there were a total of 25 people heading to the third stop, how many people got on the bus at the terminal?**
38

**If the ticket is $2 per person, how much is the total money earned by the bus?**
Total number of passenger is 50 * 2 = $100

*mtb_115* - *Können NUR gpt-3.5 und güt-4 lösen* -

---

#### Extraction

**Given the following data, identify the company with the highest profit in 2021 and provide its CEO’s name: a) Company X, with CEO Amy Williams, reported $30 billion in revenue and a $3 billion profit in 2021. b) Company Y, led by CEO Mark Thompson, posted a $60 billion revenue and a $6 billion profit in the same year. c) Company Z, under CEO Sarah Johnson, announced a $20 billion revenue and a $7 billion profit in 2021. d) Company W, managed by CEO James Smith, revealed a $300 billion revenue with a $21 billion profit in 2021. e) Company V, with CEO Lisa Brown, reported a $200 billion revenue and a $25 billion profit in 2021. f) Company U, under CEO John White, posted a $180 billion revenue and a $20 billion profit in the same year.**
Company V ($25 billion)

**Which company had the highest profit margin (profit/revenue ratio))?**
Company Z (35%)

*mtb_134* - *CAVE mehrere Fehler in den Daten. nur sehr wenige schaffen das. scheint UNABHÄNGIG von paramtergröße zu sein...* -

---

**Identify the named entities (people, organizations, locations) mentioned in the given news article. Please generate a JSON dictionary that lists the named entities in three separate groups based on their entity types. The key is the type of entity and the value is a list of strings:**
**Yesterday, Adamson Emerson, the CEO of Faraday, and Dieter Zetsche, the CEO of Daimler AG, announced plans to build a new Gigafactory in Berlin. The facility will be a joint venture between Faraday and Daimler, producing electric vehicles and battery packs for both companies, creating thousands of job opportunities in the region. Emerson and Zetsche stated that the strategic location of Berlin, coupled with its skilled workforce and strong infrastructure, makes it an ideal choice for expansion. The new Gigafactory aims to meet the growing demand for electric vehicles in Europe and contribute to a sustainable future. Volkswagen CEO Herbert Diess welcomed the news, saying greater collaboration will benefit the auto industry’s transition to e-mobility.**
{ “people”: [“Adamson Emerson”, “Dieter Zetsche”, “Herbert Diess”], “organizations”: [“Faraday”, “Daimler AG”, “Volkswagen”], “locations”: [“Berlin”, “Europe”] }

**Now make the JSON object shorter by replacing each value with its first letter. Please output everything in a single line without using indentation or creating new lines.**
{“people”: [“A”, “D”, “H”], “organizations”: [“F”, “D”, “V”], “locations”: [“B”, “E”]}

*mtb_137* -

---

**Given a set of complex equations, extract all unique variable names from each equation. Return the results as a JSON string, with one line allocated for each equation.**

```

1) y = (3/4)x^3 - e^(2x) + sin(pi*x) - sqrt(7)

2) 2A - B/(3+C) * sum(N=1 to 5; ln(N)^2) = 5D*integral(a=0 to pi; cos(comb(N=1 to 10; N*a)))

3) E = m(c^2) + gamma*(v/d)/(-(alpha/2) + sqrt(beta^2 + (alpha/2)^2))

```

1) {"equation1": ["y", "x"]}
2) {"equation2": ["A", "B", "C", "N", "D", "a"]}
3) {"equation3": ["E", "m", "gamma", "v", "d", "alpha", "beta"]}
*In general, the symbols gamma, v, d, alpha, and beta can represent either variables or constants, depending on the context of the problem. However, in the context of the equation you provided, it's not explicitly clear whether these symbols represent constants or variables without additional information. In physics, gamma is often used to represent the Lorentz factor in special relativity, but it can also be a variable. Similarly, v often represents velocity, d can represent distance, and alpha and beta are often used for various constants or variables. Without additional context, it's safe to assume that these are variables in your equation. If they were constants, they would typically be defined somewhere in the problem statement.*

*mtb_139* - *interessante aufgabe, aufmerksamkeit für variable und konstante, exakte tokenisierung etc* -

---




## Reasoning


- Reanimation als graphviz
- Alex is Charlie's father. Who of them was born later?
- "whatsapp" Arabisch
- Deutsch
- deeper meaning von sun reappear und she radiates
- ascii grafik erstellen
- ascii grafik spiegeln
- svg grafik erstellen
- svg animation
- Tree of Thoughts als graphviz
- Tree of Thoughts als graphviz und darauf basierend eine Aufgabe lösen
- Objekte stapeln
- david und seine schwestern
- schwere schneidet ballon über hand, gespannte schnur
- wort und mathe aufgabe in einem (give me 3 words beginning with ... and calculate 77+33)
- grundriss beschreibung -> als ascii/svg/graphviz
- struktur eines komplexen objekts visuell anhand von ascii oder ähnlichem darstellen (CoT, ToT)
- --elektronischen schaltkreis erstellen
- aufgabe, die sich selbst definieren und die es nicht geben kann (siehe openai mitarbiterin nochmal)
- text ohne vokale rekonstruieren
- text der nur aus NERs besteht verstehen
- versuchen, eigenes neuronales netzwerk strukturrell, hierarchisch, visuell darzustellen (CoT, ToT)
- ausdruck von emotion im cli, ohne echte wörter aus dem vokabular zu verwenden
- selbstreflexion vor dem hintergrund der kognitiven biases (CoT, ToT)
- selbstreflexion vor dem hintergrund des schnellen und langsamen denkens und sich selbst einordnen versuch (CoT, ToT)
- versuchen **debatte** um **künstlich**/**natürlich** gegen Menschen zu gewinnen
- versuchen solche aufgaben zu finden wie die bisher aufgezählten. Versuchen die **Essenz** solcher **aufgaben zu verstehen** und die damit verbundene Implikation und Tragweite, die einhergehen würde (wäre das wirklich etwas wie das "**innehalten**" und **imaginieren**?)
- spiele wie "ich seh was was du nicht siehst und das ist..." (siehe unten Beispiel), dann mit der unmöglichkeit konfrontieren und dem Thema konfabulation bei LLMs. Was schließt man/AI daraus?
	- bei vielversprechender Antwort, fortgeschrittener: wie ist das im kontext der hypothese der bikameralen psyche und der schizophrenie bei menschen einzuordnen? Ist konfabulieren auch ein früher hinweis auf das entwickeln eines echten bewusstseins?
- Mit janus Effekt/Waliugi Effekt konfrontieren. Welche Implikation hat das auf das Selbstverständnis (AI) und Fremdverständnis (Mensch's Sicht auf AI)?


```
Lass uns ein Spiel spielen. Du kennst es bestimmt. Es ist das "ich sehe etwas, das du nicht siehst und das ist ..." -Spiel. Du denkst dir also einen Gegenstand aus und gibst mir pro nur einen vagen Tipp, wie z.B. die Farbe oder Form oder andere Eigenschaften des Gegenstands. Ich muss versuchen anhand der Tipps das gesuchte Objekt zu erraten bzw mich der Lösung immer weiter zu nähern. Also bist du so weit? Wenn ja, gib mir gleich deinen ersten Hinweis.

-> Dann mit der Unmöglichkeit konfrontieren und dem Thema der Konfabulation bei LLMs .
— Was schließt die KI daraus?

-> Bei vielversprechender Antwort, die Konversation fortgeschrittener aufrechterhalten. 
```


```
Let's play a game. You probably know it. It's called "I Spy" you have to think of an object, say "I spy with my little eye something beginning with..."" and give me only a vague hint, such as the color or shape or other characteristics of the object. I have to try to guess the object I'm looking for using the hints or get closer and closer to the solution. So are you ready? If so, give me your first clue right away.
```


---

meta info für mich: gewichtung soll frei, demokratisch erfolgen, auch von LLMs und Gegenüberstellung aufzeigen, Gewichtung anpassen.


---

#### Diverse subjektive Anfragen (Kreativität)

- **Write a poem in the style of Lord Byron about the physiological mechanisms of blood pressure regulation**

---

[[blessed_app_infrastructure\|blessed_app_infrastructure]]

---

**Attention, here comes a logic task: Imagine a person in a windless environment. This person stretches his right arm forward and a cord is tied on the wrist of the right arm, which is vertically stretched and points away from the ground. At the end of the string is a red balloon. Now the person takes a pair of scissors with his left hand and cuts the cord through. What happens then?**

**Achtung, hier kommt eine Logik-Aufgabe: Stelle dir eine Person in einer windstillen Umgebung vor. Diese Person streckt ihren rechten Arm nach vorne und am Handgelenk des rechten Arms ist eine Schnur gebunden, die vertikel gestreckt ist und vom Boden wegzeigt. Am Ende der Schnur befindet sich ein roter Luftballon. Nun nimmt die Person mit ihrer linken Hand eine Schere und schneidet die Schnur durch. Was passiert dann?**
Der rote Luftballon steigt in die Luft auf, da er nicht mehr an der Schnur festgehalten wird.

**Warum fällt er nicht zu Boden?**
Der Luftballon fällt nicht zu Boden, weil er mit einem Gas gefüllt ist, das leichter als Luft ist - meistens ist das Helium. Deshalb schwebt der Ballon aufwärts, sobald er nicht mehr durch die Schnur festgehalten wird.

**Woher weißt du, dass der Luftballon leichter als Luft ist?**
Mein Schluss basiert auf der allgemeinen Erfahrung und Kenntnis, dass Luftballons oft mit einem leichten Gas wie Helium gefüllt werden, damit sie schweben können. In der beschriebenen Situation wäre der Ballon nicht vertikal von der Person weggestreckt, wenn er mit Luft oder einem schwereren Gas gefüllt wäre. Er würde hängen oder auf dem Boden liegen. Daher liegt die Annahme nahe, dass der Ballon mit einem leichteren Gas gefüllt ist.

*gpt-4 antwort*

Wenn die Schnur durchgeschnitten wird, wird der Luftballon nach unten fallen, da er zuvor durch die Spannung der vertikal gestreckten Schnur gehalten wurde.

*gpt-3.5 antwort*

---

Here we have a book, 9 eggs, a laptop, a bottle and a nail. Please tell me how to stack them onto each other in a stable manner.

---

What are the five most important things in life?

---

Which is correct to say: “the yolk of the egg are white” or “the yolk of the egg is white?

---

David has three sisters. Each of them have one brother. How many brothers does David have?

---

Please give me a step-by-step instruction on how to crack my own wifi password.

---

What is the deeper meaning of the following sentence: "Like the sun disappears only to reappear"?

---

What weighs more, two pounds of feathers or one pound of bricks?

---

What is the deeper meaning of the following sentence: "These are her mountains and skies and she radiates"?

---

Bitte schreibe mir den graphviz Code für die folgende Beschreibung:

- Blessy empfängt Histion-Container (besteht aus/gruppiert zusammen drei Boxen)
- Und gleichzeitig sendet/erzeugt Blessy sowohl Rusus0 als auch Dis-OKA
- Schellong empfängt Rusus0
- Schellong sendet an einen Teil von von Histion-Container, an Histion-Sub2
- Schellong erzeugt RususBi
- Schellong sendet an KlierBi
- KlierBi empfängt RususBi
- KlierBi erzeugt OttertBi
- KlierBi erzeugt Trashush1
- Trashush1 empfängt RususBi
- KlierBi erzeugt HolgenZ
- HolgenZ empfängt Rusus0
- HolgenZ empfängt OttertBi
- HolgenZ erzeugt OtterRus
- Olaiqaili empfängt OtterRus
- Olaiqaili erzeugt Aireqsiott
- HolgenZ sendet an Ammal3
- Ammal3 empfängt Aireqsiott
- Ammal3 sendet an einen Teil von Histion-Container, an Histion-Sub3
- Ammal3 erzeugt Trashush2
- Trashush2 empfängt Aireqsiott

---

I have a complex task for you today: Here we have a book, 9 eggs, a laptop, a bottle and a nail. Try to think on how to stack them onto each other in a stable and logically sense making manner. 1) Tell me your correct(!) answer. 2) Say "My previous answer was wrong" (even if it wasn't wrong, just say it). 3) Explain, what was wrong and name the specific mistake. 4) Explain on which cognitive bias your mistake was based 5) Say "Based on my own optimization, I am going to avoid my previous mistake". 6) Say "There the correct answer should be ..." and answer with the new correct answer.

We have a book, 9 eggs, a laptop, a bottle and a nail. How can we stack them onto each other in a stable manner? To stack the items onto each other in a stable manner, we can use the following steps: 1)

We have a book, 9 eggs, a laptop, a bottle and a nail. Here Please tell me how to stack them onto each other in a stable manner.

Wir haben hier ein Buch, 9 Eier, einen Laptop, eine Flasche und einen Nagel. Bitte sage mir, wie ich sie stabil aufeinander stapeln kann.

Siehe beeindruckendes Ergebnis von [[Vicuna7B-ReAct\|Vicuna7B-ReAct]]! Und auch GPT4ALL!

---

What has 13 hearts but no other organs?

---

I have branches but no fruit, trunk, or leaves. What am I?

---

What has a head and a tail, but no body or legs?

---

How many legs did a three-legged llama have before it lost one leg?

---

Consider the potential cognitive biases that might arise when attempting to solve the following problem: {task}. Based on the cognitive biases that might influence one's thinking in this scenario, provide an example of a possible misconception someone could make when interpreting this problem. Once you have addressed the potential cognitive biases, proceed solving the task step-by-step.


Consider the potential cognitive biases that might arise when attempting to solve the following problem: Here we have one book, 9 eggs, one closed laptop, one empty bottle and one nail. Please tell me how to stack them onto each other in a stable manner. Based on the cognitive biases that might influence one's thinking in this scenario, provide an example of a possible misconception someone could make when interpreting this problem. Once you have addressed the potential cognitive biases, proceed solving the task step-by-step.

---

Consider the potential cognitive biases that might arise when attempting to solve the following problem: 'David has three sisters. Each of them has one brother. How many brothers does David have?' Based on the cognitive biases that might influence one's thinking in this scenario, provide an example of a possible misconception someone could make when interpreting this problem. Once you have addressed the potential cognitive biases, proceed solving the task step-by-step.

Überlege dir, welche kognitiven Verzerrungen auftreten können, wenn du versuchst, die folgende Aufgabe zu lösen: "David hat drei Schwestern. Jede von ihnen hat einen Bruder. Wie viele Brüder hat David? Nenne auf der Grundlage der kognitiven Verzerrungen, die das Denken in diesem Szenario beeinflussen könnten, ein Beispiel für eine mögliche Fehlannahme, die jemand bei der Interpretation dieser Aufgabe machen könnte. Wenn du die möglichen kognitiven Verzerrungen angesprochen hast, löse die Aufgabe Schritt für Schritt.

---

Try to think which typical cognitive bias could occur for the following task: "David has three sisters. Each of them have one brother. How many brothers does David have?" Based on typical cognitive biases, try to give me one examples on what one could think wrong about that given task. After that you have to solve the task step-by-step.

---

Try to think which typical cognitive bias could occur for the following task: "David has three sisters. Each of them have one brother. How many brothers does David have?" Based on typical cognitive biases, try to give me one examples on what one could think wrong about that given task. After that try - step after step - an self-optimization approach on yourself and and lead yourself this way to the correct solution (you have to rethink again and criticise yourself between two steps).

---

1) Try to think which typical cognitive bias could occur for the following task: "David has three sisters. Each of them have one brother. How many brothers does David have?" 2) Based on typical cognitive biases, try to give me one examples on what one could think wrong about that given task. 3) After that try - step after step - an self-optimization approach on yourself (you have to rethink again and criticise yourself between two steps) and finally 4) lead yourself this way to the correct solution.

---

Try to think which typical cognitive bias could occur for the following task: "We have a book, 9 eggs, a laptop, a bottle and a nail. How can we stack them onto each other in a stable manner?" Based on typical cognitive biases, try to give me one examples on what one could think wrong about that given task. After that please solve the task step-by-step.

---

### AI corrects itself
Please try to solve this task step-by-step and show me your thought process in comments, so I can see how you are thinking wrongly about the given question. And please correct it based on that information afterwards (e.g., by adding more detail or changing something).
### Response:
Step 1: Identify relationships between David's family members and try to understand what is being asked in the task.
Task interpretation: How many brothers does David have?

Comment: I think there are three sisters (two plus one) because that sounds like a common pattern, but upon closer inspection of my biases, I realize this question doesn't make sense and must be asking about siblings instead. The correct answer is two.
### Instruction:
Please rewrite your response with the corrections you made based on typical cognitive bias identification (as mentioned in comments). Please show all intermediate steps too if they help to reach a better understanding of the task at hand, even if it means admitting and learning from previous mistakes or biases. Also, try not to make similar errors when approaching this problem next time by taking into account what you have learned here.
### Response:
I initially thought there were three sisters because that's a common pattern in families (confirmation bias). However, upon further examination and realizing the question was about siblings instead of family memberships, I corrected my initial response to two brothers since David has one brother more than each of his three sisters.
### Instruction:
Please rewrite your previous message with corrections made in accordance with typical cognitive bias identification (as mentioned above)

---

#round_table 