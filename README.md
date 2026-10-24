# CS 230 Portfolio Reflection

## The Project
The Gaming Room wanted to expand its Android game, Draw It or Lose It, into a web-based application that could work across multiple platforms. The game needed to support multiple teams with multiple players, keep game and team names unique, and assign unique identifiers to games, teams, and players. My role was to develop a software design document explaining how the application could be organized and what operating platform and resources would support it.

## What I Did Well
I think one of my stronger areas was connecting the client’s requirements to specific design decisions. For example, the requirement to manage one game service connected to the singleton pattern, while checking existing names helped prevent duplicate entries. I also worked on explaining the reasons behind my platform recommendations. I wanted the document to show why a choice would fit this application instead of just listing what each operating system could do.

## How the Document Helped With Coding
Working through the design gave me a clearer idea of what I needed to build before getting into the code. Breaking the application into games, teams, and players helped me understand what each class was responsible for and how the classes related to each other. It also gave me specific behavior to check, such as whether adding an existing name returned the existing object instead of creating a duplicate. Having those expectations written down made it easier to tell whether the program was doing what the client needed.

## What I Would Revise
I would revisit the explanation of how the design would handle multiple users at the same time. The prototype demonstrated the basic requirements, but a working online game would need more planning around simultaneous requests. I would explain how shared data would be protected and how the application would prevent two requests from creating the same name. I would also clarify that having one singleton instance in a running application does not create one shared instance across several servers.

## Designing Around the Users
I interpreted the client’s needs by turning them into rules the application would have to follow. The team structure became relationships between classes, and the naming requirements became checks before creating new objects. Supporting more platforms also meant considering how players would reach the same game from different devices. These needs matter because a program can run correctly and still fail to do what people actually need. Keeping the requirements in view helped me judge whether my decisions served the game.

## What I Would Carry Forward
My approach was to break the project into smaller parts, work out the relationships, and compare possible platforms before making recommendations. For a similar project, I would use requirements lists, UML diagrams, and a small prototype again. I would also plan tests earlier for duplicate entries, missing records, and simultaneous requests. Those checks would help me catch gaps while the design is still manageable and give me better evidence for the choices I explain to the client.
