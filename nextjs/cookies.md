sending http requests is done in two parts, sending headers then sending the body.
and once you start sending the body you can't go back to sending/resending the headers
as they have already been sent.

you can only set cookies using a response header (set-cookie).


when you use suspense to render a fallback for an async component that
takes some time to load, react will send headers as quickly as possible and 
then sends the html of the fallback (the response body) and then once the component
has finished loding, it replaces the sent html in the response with the actual
component.

since react already sent the headers and started streaming the html, you can't set cookies
AFTER react already started sending the response body as it has already finished
sending all headers (quickly to give the feel of a fast loading page) and can no
longer go back and send new headers (set-cookie)
