```

    title Exercise 0.4 part 0

    actor User

    User -> browser : Click button Save
    browser -> server: HTTP POST https://studies.cs.helsinki.fi/exampleapp/new_note
    note right of browser: Send content input text


    note left of server : Ajax code server
    note left of server : add new note

    server-->browser :  Status 302 redirection

    note right of browser: reload


    browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/notes
    server-->browser: HTML-code
    browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.css
    server-->browser: main.css
    browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.js
    server-->browser: main.js

    note over browser:
    browser starts executing js-code
    that requests JSON data from server
    end note

    browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/data.json
    server-->browser: [{ content: "HTML is easy", date: "2019-05-23" }, ... more notes]

```
