# Week 10 - Introduction to AI and Machine Learning

Activity session 🏫 Date: **Oct 28, 2022 Friday** Event: **Classroom session** Venue: **KMUTT S4 building 11th Floor Room 1114** Speaker(s):

1. P'North (TG: north.npk) AI researcher at NSTDA

#### Key notes 📝

**What is artificial intelligence?**

* Concept is to learn from experience (Alan Turing, Turing machine at 1953) on his report published on 1948 (Intelligent Machines)

**Evolution of AI**

* AI (1950s) was the era of Turing's work
* ML (1980s) brought things like spam filtering
* DL (2010s) brought topics like back propagation

**Machine Learning**

* TED Talk by Fei Fei Li (How we're teaching machine to understand pictures?)
* Traditional process: data + rules -> outcome
* ML process: data + outome -> rules

**Types of Machine Learning** _Based on process_: Unsupervised, Semi Supervised, Supervised, Reinforcement (reward-based)

_Based on structural data:_ Linear regression, KNN (K-nearest neighbor), Decision Tree

_For Time Series Data:_ ARIMA, Long Short Term Memory, Recurrent Neural Network

_For Natural Language:_ Also, long short term memory, Transformer model (too complex and hard to learn and use compared to others)

_For image data:_ Convolutional neural network (CNN), Vision transformer, YOLOv7

**Real world usage examples:**

1. Netflix recommendation (clustering model)
2. Falcon 9 landing (gliding system)
3. Tesla (Level 2 Automation) driver's assistance autopilot
4. Midjourney Image Generator

> What do you want AI to do? -> question (on mentimeter word cloud)

**ML Tools**: _Programming languages:_ Python 🌟, Scala, Java R

Models:

* CNN (Conovlutional Neural Network)
* ANN (Artificial Neural Network), a part of Deep learning
* GAN (Generative Adversarial Network)
* Transformers model (huge but accurate) - state of the art model nowadays

Tools:

1. Pandas - data preprocessing, data frame, import & cleaning
2. sklearn - models, criteria mindmapping
3. TF Keras
4. YOLO - Computer Vision, Object Detection
5. Kaggle - Find Datasets & example notebooks
6. Papers with code - latest papers and extra datasets
7. Teachable Machine (easily learning ML)

#### New ideas 💡

* the above key points are commonly found in general talk about machine learning, but most of the miss the calibration metrics part using confusion matrix (it is whether a model is accurate enough to deploy or not)
* Machine Learning follows Garbage In, Garbage Out workflow. Therefore, quality of data is very much crucial for proper functioning.
* Imbalance in datasheet?
  * Solution: more data, sampling method
* Also, I got the opportunity to clear some of the issues I've encountered when exploring machine learning on my own:
  1. Data format of model (JSON/Binary) - Flat file, memory, python variable? Each ML infrastructure has their own, and wrapper to work with client side with quality documentation. Therefore, no more hurdles to worry about.
  2. Deploy (JS, Qt, Flutter)? Web is the best option (JS). Flutter is quite broken. Backend and REST approach is quite laggy.
  3. Starting a career!
  4. How to choose project \[hackathon]? (hackathon/technology/fun) work with example projects a lot as a beginner

#### Resources 🎁

* Papers with Code (state of art ML workflow and papers) + extra datasets
* Kaggle to start the work with

### Reflections 🔮

What do you feel?

How do these fit with your current practice and understanding?

How will you incorporate any new understanding or skill you have learned into your day to day practice?

#### Impact 🚀

How the session turned out to be of value if it did?

#### Final Reflection 🔚

Have you identified any learning needs to look forward into your personal learning and development?

How might you address these?

TODO:

## A brief introduction (the 'what?') 🤷‍♂️

* It was the first day of the CPE101 Coursework.

> * Any materials regarding the course will go here

## Impact  (the 'so what?') 🚀

How the session turned out to be of value if it did?

> * Just wondering about the syllabus.
> * Relatable to the work we do currently.

## Reflections (the 'now what?') 🤔

> * Potential applications of the works and the lessons carried out during the course.
> * Any suggestions to yourself, the organization, and other stakeholders?

> End of learning reflection, please proceed to below reading for the further details only.

## A detailed exploration of this coursework/activity 📄

> * Here you can write the details about the coursework or the activity
> * It can include the coursework, the software, and framework used, the detailed specifications, something like that!

#### Keynotes 📝

> In points.
>
> You can discard the title if you like.

* Embedded C++

```cpp
void setup( ) {
  // run once
}

void loop() {
  // run forever
}
```

Issue: `avrdude: stk500_recv(): programmer is not responding`

Labs:

1. Blink LED
2. Frequency output (Piezo Electric Speaker) P15 (D9) -> C1 (10 uF) -> +(speaker)- -> GND

```cpp
void setup() {
	pinMode(9, OUTPUT);
}

void loop() {
	for (int i = 0; i < 500; i++) {
		digitalWrite(9, HIGH);
		delayMicroseconds(500);
		digitalWrite(9, LOW);
		delay Microseconds(500);
	}
}
	
```

1. LDR control for LED
2. Display on SLCD

#### New ideas 💡

* something new?

#### Resources 🎁

* Documentation: http://www.inexglobal.com/downloads/POP168kit\_e.pdf

### Additional Notes 📄

Anything extra you would like to add goes here.

### Further lookup suggestions 🔍

> List of further lookup suggestions

### References 🔖

> List of references
