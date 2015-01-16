# s15_sabnis_data_lecture_notes
Lecture notes for the Spring 2015 Data Engineering class

## Lecture 02
#### Markdown :
  - Invented by John Gruber (You can find his original documentation at Daring Fireball)
  - It is one of the markup languages just like HTML.
  - Allows plain text formatting to rich text like lists or tables.
  - There are 2 types : Standard markdown and Github falvoured markdown
  
### Examples of different components in markdown :
  1. Headers :
      - H1 to H6  
        \# H1  
        \## H2  
        \### H3  
        \#### H4  
        \##### H5  
        \###### H6  

  2. Bold Italics and Strikethroughs  
      - ** This is Bold **  
      - * This is Italics *  
      - ~~ This is Striketrough ~~
  
  3. Lists  
      - Unordered lists uses astericks, pulses and stars as its markers.  
        * This is unordered list  
          - First  
          - Second  
          - Third  
                
      - Orderd lists  
        * This is an ordered list  
          1. One  
          2. Two  
          3. Three 
          
  4. Links
      - This is a link example : [Google](http://www.google.com)  
      
  5. Codeblocks and syntax highlighting  
      - Used for writing code  
      - \<pre> and \</pre> tags are used  
        <p>This is a normal paragraph:</p>  
        <pre><code>This is a code block</code></pre>  
      - For syntax highlighting, we can specify the language in which the code is written  
      
  6. Tables
      - Table example with indentation details  
        | Left-Aligned  | Center Aligned  | Right Aligned |  
        |---------------|-----------------|---------------|  
        | col 3 is      | some wordy text | $1600         |  
        | col 2 is      | centered        |   $12         |  
        | zebra stripes | are neat        |    $1         |  

  7. Horizontal line  
      - Place three or more hyphens, asterisks or underscores on a line  
      -  \*** or \--- or \___ will give  
          -----

#### REST :
  - Standard web application flow 
    - In a standerd web application, a request is generated from web browser which is directed to web server or app server
    (after resolving your domain name). A typical request could be http:/ebay.com/products/10. The types of requests are 
    GET, POST, PUT, DELETE.
    - Web server forwards this query to handler who knows how to handle any type of requests. Web browser may just forward
    '/products/10' part to handler.
    - Handler resolves the request and constructs and HTML response. This response if returned to web server and then in
    turn to web browser.
    - Web browser is intelligent to perceive the response and show it to user. In the response if there are more links to
    load images or scripts, browser again sends a request to web server.
    - For ex : First page of amazon.com. It loads various parts of a page from different servers (services).
    
  - REST (Representation State Transfer) is an architecture.  
  
  - CRUD Operations : Consider URL ('http:/ebay.com/products/10')   
    - URI trying to access users : ('/products/10')  
      - GET = Read (get current state of all users)  
              if ('/users/id') then current state of user with id = 10
      - POST = Create (create new user)
      - PUT = Update (update user info)
      - DELETE = Destroy (destroy user)
        
    - GET has limit on number of url params. Hence POST is used where params are sent as a part of body.
  
