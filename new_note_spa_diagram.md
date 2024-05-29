```mermaid
sequenceDiagram
    participant browser
    participant server


    Note right of browser: The browser has already loaded the webpage and executed all the JavaScript code necessary to render the webpage properly

    
    Note right of browser: A note is created and the Javascript code on the browser sees that the form has been submitted , and the event handler function for the form is run.
    Note right of browser: The function adds a note to the page using the DOM API and redraws the notes.
    Note right of browser: The function also sends a POST request to the server to save the note to the server's memory. 
    
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
     with the form data (the content and the timestamp)

```