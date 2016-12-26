---
layout: default
---

[![LGTM](http://lgtm.in/p/OX19r0cQp)](http://lgtm.in/i/OX19r0cQp)

:D

:beer:

:smile:

<img src='http://g.gravizo.com/g?
@startuml;

actor User;
participant "First Class" as A;
participant "Second Class" as B;
participant "Last Class" as C;

User -> A: DoWork;
activate A;

A -> B: Create Request;
activate B;

B -> C: DoWork;
activate C;

C --> B: WorkDone;
destroy C;

B --> A: Request Created;
deactivate B;

A --> User: Done;
deactivate A;

@enduml
'>
