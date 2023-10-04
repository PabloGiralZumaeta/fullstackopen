```
    title Exercise 0.6 part 0
    actor User
    User -> Browser: Click save input with content
    Browser -> Server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    note right of Browser: Send content input text
    note left of Server: Return Status 201 Create
    Server --> Browser : Update Notes without page reload
```
