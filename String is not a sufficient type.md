## `String` is not a sufficient type

### How type systems can help you make better software

---

^ Who am I?

## About Me

- Chris Dzombak
- iOS Frameworks Team
- dzombak@nytimes.com
- @dzombak on Slack
- @cdzombak on Twitter

---

## Relax.

^ FYI: this talk isn’t going to provide hard, actionable information, and there’s no need to take notes. This is just some food for thought.

---

## Let’s talk about `String`.

^ We use this basic type, String, to represent all sorts of things in our applications.

---

- user input
- human language words
- output for the UI
- SQL statements
- keypaths for Cocoa KVO/KVC
- …

---

- …
- XPath queries for XML
- shell commands
- HTML
- regular expressions
- and more!

---

## `String` is totally insufficient to represent all these different things

^ `String` is completely insufficient for representing all these things.

^ They all have vastly different meanings and uses,
operations you can do with one don’t necessarily apply to the others,
and you generally should not be able to combine these things.

^ In fact, using just `String`,
which _does_ allow mixing these different types of strings,
leads to a lot of really common security vulnerabilities and other user-facing problems.

---

