# Few-shot GPT3 for ProtoQA

**Prompt**
```
Generate 10 different answers to the given question.

Question: Name something around the house that’s often replaced.
Answers: light bulb, garbage bags, toilet paper, food, furniture, carpet, batteries, water filter, blankets, painting.

Question: Name something that gets caught in your hair.
Answers: bubble gum, hair brush, hair comb, necklace, earring, glasses, louse, bugs, dust, snow.

Question: Name something that would make someone change their return flight.
Answers: urgent matters, urgency of family member, bad weather, snow storm, sickness, forget the passport, flight delay, bad service, work meeting, cheaper seats.

Question: Name something people do while getting checked by their dentist.
Answers: describe their oral condition, open mouth, relax, laying down, close eyes, get nervous, check phone, get bored, look at the lamp, say ahhhh.

Question: Name something parents would criticize their children for having.
Answers: drug, smoke, beer, video games, bad habits, long nails, expensive phone, misbehavior, bad performance in school guns, bad friends.

Question: {question}
Answers:
```
**Dev result**

|Inc@1|Inc@3|Inc@5|Ans@1|Ans@3|Ans@5|Ans@10|Ans@all|
|-|-|-|-|-|-|-|-|
|27.69|48.10|52.70|43.08|50.11|51.50|59.18|68.54|

Note: r1q14, r2q6, r2q10, r2q27, r2q42 are removed, since they are used to desigin prompt.
