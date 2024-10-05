---
draft: true
draftSectionTwo: true
tags:
---

This page is a place to place text or other bits of information in, temporarily.

3. Exercise: [[Introduction to Generative Art]]
	- Use any time that remains to begin working on this task.


## Playground with goToHome function

https://www.russellgordon.ca/lcs/icd2o/GoingHomeAgainComplete.playgroundbook.zip

```swift
// Make the turtle return to the origin
func goHome() {
    
    // Pick up the pen so a trail is not left behind
    turtle.penUp()
    
    // Get the turtle's current position
    let x = turtle.currentPosition().x
    let y = turtle.currentPosition().y

    // Go home, using the opposite value of turtle's position
    turtle.diagonal(dx: x * -1, dy: y * -1)
    
    // Put down the pen again
    turtle.penDown()
}

```


## SIC Drop-In Sessions

Here is this week's schedule:

Day|Time|SIC|Location
-|-|-|-
Monday, April 29|1:00 PM to 1:30 PM|Griffin|Room 36
Tuesday, April 30|12:30 PM to 1:30 PM|Morgan|Room 36
Thursday, May 2|12:30 PM to 1:30 PM|Justin|Room 36
Friday, May 3|12:30 PM to 1:30 PM|Quin|Room 36

## Agenda
1. Tutorial: Taking Screenshots 🫥⬅️
5. 
6. Concept: [[Functions with Parameters]] 🫥⬅️
7. Tutorial: [[Syncing Files from Cloud Storage]]
8. Tutorial: [[Creating Bookmarks]] 
9. Tutorial: [[Hot Corners]]
10. Exercise: [[Keyboard Shortcuts]]
2. Discussion: Ethics 🫥⬅️

## Things to do before our next class
- [ ] If not completed in class, finish the items listed above.
- [ ] Share evidence of your progress from today's class in your portfolio [on Notion](https://notion.so) – remember to [[Taking Screenshots|include screenshots]].
