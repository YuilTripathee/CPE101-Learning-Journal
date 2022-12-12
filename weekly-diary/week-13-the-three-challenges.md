# Week 13 - The Three Challenges

November 18, 2022

The phrase "three pillar challenges" refers to the three test challenges we must complete on this day using the ATMega-168 CPU (based model) and POP168 BOARD. Given that we are provided with a few sample sheets of information and that we must update code in order to complete the objective, I would say that the obstacles today are pretty difficult in comparison to past days.

## Coursework (the 'what?') 🤷‍♂️

**The first challenge**, "racing track," requires us to create computer code to drive a robot. In addition to the robots, there are two walls that must not be hit in order for the vehicle to reach the track's terminus.

**The** **third challenge ** is to get the robot to move toward the location that is thought of as the goal without utilizing any sensors. Therefore, we had to change the code that was provided in the information and go back to the code that we wanted. To get to the location we desired, we changed both wheels' speeds and added delay to a few lines of code.

**The last challenge** is to utilize two buttons as a bumper to make the robot change course when it collides with something. Within three minutes, we must strike some toys called TAs as hard as we can.

## Impact  (the 'so what?') 🚀

We must employ the skills that are taught in the "Happy Coding" session in order to complete all of the missions that have been assigned to us. We had to exercise good judgment, and when combined with the lecture and our general knowledge, we hardly completed the one lab. I may still claim that this lesson helped me better.

## Reflections (the 'now what?') 🤔

I learned a lot in this session, and I now appreciate how valuable micro-controllers are in everyday life. For a computer engineer, understanding how they operate and how they perform is unquestionably essential. I'll therefore try to use the knowledge I've learned from these issues in future scenarios.

## A detailed exploration of this coursework/activity 📄

#### Keynotes 📝

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
