# Holy Grail Three-Tier
## Description
This is a simple three-tier app that includes holy grail layout with React, server through Express, and data store through Redis and Docker. Buttons in each section allow you to update the count for each section. Each time the count is updated it is passed through to the data store. The data store is set up with Redis and run through Docker.

You can also update the database by hitting /update/:section/:value. 
  Example: localhost:3000/update/footer/2
  This will increase the footer counter by 2.
  
To display all data you can hit /data.
  Example: localhost:3000/data
  This will display something similar to this:
  {"header":-3,"left":5,"article":4,"right":-1,"footer":7}
  
Tech stack: Node, React, Express, Redis, Docker

## Instructions
Download all files to your machine and install all dependencies. With Docker, create a Docker image of Redis and run the image. Start the app through npm start to use nodemon, or through node index.js to run without nodemon. Navigate to localhost:3000 to access the holy grail UI. 

Additional routes:
  /update/:section/:value
    -This updates the database for the given section (i.e. header) by adding the given value to it's current value.
    -Example: localhost:3000/update/header/1
    
  /data
    -This displays all data
    
## Roadmap
Updates to UI aesthetics and additional routes for resetting sections are some of the planned future improvements.



