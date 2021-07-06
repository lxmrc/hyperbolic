>The Hyperbolic Time Chamber is a place where one can train and get stronger in a short amount of time. 

Currently just an in-browser editor that can execute code on the server-side in containers. Eventually a platform for practicing programming using spaced repetition through "executable flashcards".

I only have the basic functionality in place: an in-browser code editor which can connect to a container on the server where the code is run and the output is then returned to the browser.

The backend is Ruby on Rails. I use the docker-api gem to start and stop Docker containers via Rails controller actions. Each instance of a browser editor is associated with its specific container through Redis. I use JavaScript on the frontend to start a container when the editor page is opened and shut it down when the tab is closed.
