### Async and Defer in javascript 
The async and defer attributes in JavaScript <script> tags control how external script
are downloaded and executed, impacting page loading performance.
They are used to prevent scripts from blocking the parsing and rendering of the HTML document.

<ul><li>Async scripts are executed as soon as the script is loaded, so it doesn't guarantee the order of execution
(a script you included at the end may execute before the first script file)</li>

<li>Defer scripts guarantee the order of execution in which they appear in the page.</li></ul>



<img width="1558" height="1542" alt="image" src="https://github.com/user-attachments/assets/82a4d023-3302-47c8-a87c-d6b7432f04a3" />
