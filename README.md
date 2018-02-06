# LECTURE_02_06

# Annoucements

* Exam 1 week from today
* Fair Game:
    * H00-H06, IC00, IC01
    * Lectures through 02/08
    * lab00, lab01, lab02, proj00
    * Readings in book that go with homework and ic00

# Intellij

* Commercial IDE for Java 
* Community edition is Free and Open Source
* UCSB CMPSC56 students encouraged to install on personal Mac, Win, Linux systems
* Possibly available on CSIL at this link
    * This is a fresh "guerrila" install, not an official one
    * It is inadequately tested, but it might work.  Give it a try.
    * It will work best if you are physically at a CSIL or Phelps 3526 terminal--doing this over remote X11 access will probably be painful, or not work at all
    * The command to type: `/cs/faculty/pconrad/intellij/bin/idea.sh`

# Guest Lecture Dillon Kearns

Experiences with bad code

* bad variable names
* shadowed parameters
* classes were named `Class1`, `Class2`, etc.
* many others...

When editing bad code, you have an uneasy feeling about changing it.

# Four concepts from Dillon Kearns

* Self-documenting code
    * You don't need comments to tell you what it does
    * That's because of good choices of variables names, method names, structure
    * Comments are "lies waiting to happen"
        * Your code will break if you make changes
        * But comments stay, even if they are untrue
        
* Microcommits
    * Not being afraid to put something into version control
    
* Safe Refactoring
    * Especially if you have an IDE
    * The IDE can help you do refactoring in a way that is guaranteed to be safe
        * E.g. renaming `Class1, Class2, Class3` to `User, Student, Instructor` the IDE can help you do that without introducing any changes.
        
* Incremental improvement
    * Really important in refactoring; some student were afraid to make a change because they didn't know what the perfect change was
    * Give yourself permission to make a change that makes it better, even if it doesn't make it perfect.
    * Don't let perfect be enemy of the good (or better)
    
# Why do we refactor?
    

# Strong Style Pairing

* <http://llewellynfalco.blogspot.com/2014/06/llewellyns-strong-style-pairing.html>

# Short cut keys for refactoring in Intellij

* `Alt-Enter` gives you a quick hint (or click the light bulb)
    * Example of a safe-refactor: convert a `switch` statement to an equivalent `if/else`
    * Doesn't need to be tested (unless you are paranoid)---you are relying on the IDE's guarantee that the `switch` and `if/else` are semantically equivalent.
* `Control-T` for "refactor this"
    * Context specific menu of various ways of refactoring the code.
* `Control-R` for run all tests
