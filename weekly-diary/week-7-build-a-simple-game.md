# Week 7 - Build a Simple Game

September 30, 2022

TODOs:

- [ ] Content writing

##  A brief introduction (the 'what?') 🤷‍♂️

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

## References

Assets:
- [Mixamo](https://www.mixamo.com/#/?page=1&query=idle)

Unity tutorials:
- [navmesh unity - YouTube](https://www.youtube.com/results?search_query=navmesh+unity)
- [LEARN UNITY - The Most BASIC TUTORIAL I'll Ever Make - YouTube](https://www.youtube.com/watch?v=pwZpJzpE2lQ)
- [How To Create AI That Follow Player With Unity 3D And C# - YouTube](https://www.youtube.com/watch?v=g7d5TFon120&ab_channel=Mtir%27sCode)
- [Unity Tutorial | 3D Spinning Cube in 10 minutes | .NET](https://dotnet.microsoft.com/en-us/learn/games/unity-tutorial/install)
- [Introduction to Unity fundamentals for absolute beginners. - YouTube](https://www.youtube.com/watch?v=ozL-h75vazQ&ab_channel=EqualReality)
