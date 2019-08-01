# life-notes
Don't forget these things in your life

* *Dynamic type vs Static type*
~~~~
[ Thursday, August 1, 2019 2:43 PM ] Quoc Ho: With python or node, you can start a server in 10 lines
[ Thursday, August 1, 2019 2:43 PM ] Quoc Ho: Not with anything jvm
[ Thursday, August 1, 2019 2:43 PM ] Quoc Ho: The question is for a big project, I don't like dynamically typed stuff
[ Thursday, August 1, 2019 2:45 PM ] Hoang Nguyen Huu: you don't like dynamically typed language even it's strong type?
[ Thursday, August 1, 2019 2:45 PM ] Hoang Nguyen Huu: why?
[ Thursday, August 1, 2019 2:46 PM ] Hoang Nguyen Huu: dynamically type's code is shorter and still as safe as statically type
[ Thursday, August 1, 2019 2:46 PM ] Hoang Nguyen Huu: as long as it has strong type
[ Thursday, August 1, 2019 2:46 PM ] Hoang Nguyen Huu: am i wrong?
[ Thursday, August 1, 2019 3:01 PM ] Quoc Ho: People like statically typed languages for a reason
[ Thursday, August 1, 2019 3:01 PM ] Quoc Ho: Not just for fun
[ Thursday, August 1, 2019 3:02 PM ] Quoc Ho: If everything is the same like you said, theres no reason for something like Java or haskell to exist
[ Thursday, August 1, 2019 3:02 PM ] Hoang Nguyen Huu: less readable?
[ Thursday, August 1, 2019 3:02 PM ] Quoc Ho: Using a statically typed language has many advantages
[ Thursday, August 1, 2019 3:02 PM ] Quoc Ho: Let me list them
[ Thursday, August 1, 2019 3:03 PM ] Quoc Ho: The first one is : more error catching at compile time
[ Thursday, August 1, 2019 3:03 PM ] Quoc Ho: With something like haskell, for example, your code is already very solid without testing
[ Thursday, August 1, 2019 3:04 PM ] Quoc Ho: In python or js, just null checking is a pain
[ Thursday, August 1, 2019 3:04 PM ] Quoc Ho: Let alone more complicated stuff
[ Thursday, August 1, 2019 3:04 PM ] Quoc Ho: With scala or Kotlin, null becomes less of an issue
[ Thursday, August 1, 2019 3:05 PM ] Quoc Ho: Second advantage : tooling
[ Thursday, August 1, 2019 3:05 PM ] Quoc Ho: With a dynamically typed language, tooling can not be very good
[ Thursday, August 1, 2019 3:05 PM ] Quoc Ho: Since IDE cannot know what type they are working with
[ Thursday, August 1, 2019 3:06 PM ] Quoc Ho: Obviously, you can code in a more restrictive way
[ Thursday, August 1, 2019 3:06 PM ] Quoc Ho: To make use of IDE features
[ Thursday, August 1, 2019 3:06 PM ] Quoc Ho: But then, why bother? Just use a statically typed language if you do that
[ Thursday, August 1, 2019 3:06 PM ] Quoc Ho: Third advantage : dynamically typed language has to be interpreted and can not be compiled
[ Thursday, August 1, 2019 3:07 PM ] Quoc Ho: This makes it very slow
[ Thursday, August 1, 2019 3:07 PM ] Quoc Ho: Just try to sum 1000000000 integers in python in a single simple loop
[ Thursday, August 1, 2019 3:07 PM ] Quoc Ho: And compare with Java
[ Thursday, August 1, 2019 3:07 PM ] Quoc Ho: I'm not surprised if it's 100 times slower
[ Thursday, August 1, 2019 3:10 PM ] Quoc Ho: 4th advantage : maintainability
[ Thursday, August 1, 2019 3:10 PM ] Quoc Ho: This includes refactoring, readability etc
[ Thursday, August 1, 2019 3:10 PM ] Quoc Ho: Try to refactor in js or python
[ Thursday, August 1, 2019 3:10 PM ] Quoc Ho: A good ide might fail less often
[ Thursday, August 1, 2019 3:11 PM ] Quoc Ho: But cannot be compared to a statically typed language
[ Thursday, August 1, 2019 3:12 PM ] Quoc Ho: Try nesting futures in python
[ Thursday, August 1, 2019 3:13 PM ] Quoc Ho: To make it not crash at runtime, you really need to make sure on your head how many nested level things are to use map, flatmap correctly
[ Thursday, August 1, 2019 3:13 PM ] Quoc Ho: Or read a function and know what type it returns
[ Thursday, August 1, 2019 3:14 PM ] Quoc Ho: Obviously, you can read the comments, if the code has it
[ Thursday, August 1, 2019 3:14 PM ] Quoc Ho: But do you trust human reading comments more or Machine checking the types at compile time?
[ Thursday, August 1, 2019 3:15 PM ] Quoc Ho: Because of these reasons, and many others, there are so many languages which start as dynamically typed languages, but then many projects show up adding types to them, to gain the benefit of being in the statically typed world
[ Thursday, August 1, 2019 3:16 PM ] Quoc Ho: Look at js, there are typescript and like 100 others
[ Thursday, August 1, 2019 3:16 PM ] Quoc Ho: Look at python
[ Thursday, August 1, 2019 3:16 PM ] Quoc Ho: Even python itself has a typed extension
[ Thursday, August 1, 2019 3:17 PM ] Quoc Ho: Before, there are also cython, and many other projects
[ Thursday, August 1, 2019 3:17 PM ] Quoc Ho: Is there any statically typed language which becomes dynamically typed later on?
[ Thursday, August 1, 2019 3:17 PM ] Quoc Ho: No!
[ Thursday, August 1, 2019 3:18 PM ] Quoc Ho: So the question is : why do people still use dynamically typed language? Because it's more convenient in smaller projects and easy to get going
[ Thursday, August 1, 2019 3:18 PM ] Quoc Ho: Less verbose
[ Thursday, August 1, 2019 3:21 PM ] Quoc Ho: So what are the perceived disadvantages of a statically typed language?
[ Thursday, August 1, 2019 3:21 PM ] Quoc Ho: 2 main things
[ Thursday, August 1, 2019 3:21 PM ] Quoc Ho: 1. It's verbose
[ Thursday, August 1, 2019 3:22 PM ] Quoc Ho: 2. Sometimes your are constrained by the type system from expressing your idea
[ Thursday, August 1, 2019 3:22 PM ] Quoc Ho: Because of this, there are a lot of design patterns etc. which is also verbose and not elegant
[ Thursday, August 1, 2019 3:23 PM ] Quoc Ho: The verbose issue could be fixed by having a good type inference system
[ Thursday, August 1, 2019 3:24 PM ] Quoc Ho: So that even when it's statically typed, it feels like dynamic
[ Thursday, August 1, 2019 3:24 PM ] Quoc Ho: The second issue could be fixed by having a more powerful typesystem
[ Thursday, August 1, 2019 3:24 PM ] Hoang Nguyen Huu: I have not lunch yet, just go out for "bánh bèo chay" recently lol
[ Thursday, August 1, 2019 3:24 PM ] Hoang Nguyen Huu: chờ tí đọc lại đã nha
[ Thursday, August 1, 2019 3:25 PM ] Quoc Ho: So that you can do things you like while staying safe and concise
[ Thursday, August 1, 2019 3:26 PM ] Quoc Ho: This is why scala and haskell have very powerful type systems
[ Thursday, August 1, 2019 3:27 PM ] Quoc Ho: It's not to make your life complicated, but rather to make sure you write things concisely, safe, and performant
[ Thursday, August 1, 2019 3:27 PM ] Quoc Ho: Same go with Rust
[ Thursday, August 1, 2019 3:27 PM ] Quoc Ho: Not so much for go, in this direction
[ Thursday, August 1, 2019 3:30 PM ] Quoc Ho: Of course, nothing is for free. To use statically typed language, you have to learn more
[ Thursday, August 1, 2019 3:30 PM ] Quoc Ho: And the more powerful the type system is, the more you have to learn
[ Thursday, August 1, 2019 3:30 PM ] Quoc Ho: But this is not learning for the sake of learning, since it actually enables you to write powerful code
[ Thursday, August 1, 2019 3:32 PM ] Quoc Ho: That's why dynamically typed languages are easy to make and to learn
[ Thursday, August 1, 2019 3:32 PM ] Quoc Ho: So there are many libraries
[ Thursday, August 1, 2019 3:32 PM ] Quoc Ho: That you can just use
[ Thursday, August 1, 2019 3:33 PM ] Quoc Ho: But do you trust the level of robustness of most js libraries?
[ Thursday, August 1, 2019 3:33 PM ] Quoc Ho: For a small project, or a script, or doesn't matter much
~~~~
