#### <script crossorigin src="https://unpkg.com/react@18/umd/react.production.min.js"></script>


The crossorigin attribute in an HTML <script> tag is used to control how cross-origin requests for scripts are handled,<br>
specifically in the context of Cross-Origin Resource Sharing (CORS).<br>
This attribute is crucial for security and proper functioning when a script is loaded from a<br>
different domain than the web page itself.

The crossorigin content attribute on media elements is a CORS settings attribute.<br>
These attributes are enumerated, and have the following possible values:
<ol>
<li>
anonymous : Request uses CORS headers and credentials flag is set to 'same-origin'. 
There is no exchange of user credentials via cookies, client-side TLS certificates or HTTP authentication,
unless destination is the same origin.</li>
<li>use-credentials :
Request uses CORS headers, credentials flag is set to 'include' and user credentials are always included.</li>
<li>"" :
Setting the attribute name to an empty value, like crossorigin or crossorigin="", is the same as anonymous.</li></ol>
<br>

By default (that is, when the attribute is not specified), CORS is not used at all.
The user agent will not ask for permission for full access to the resource and in the case of a cross-origin request,
certain limitations will be applied based on the type of element concerned:
Element Restrictions:<br>
<ul><li>img, audio, video - When resource is placed in <canvas>, element is marked as tainted.</li>
<li>script - Access to error logging via window.onerror will be limited.</li>
<li>link - Request with no appropriate crossorigin header may be discarded.</li></ul>
