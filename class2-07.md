## Redaing Notes 07

## How I explained REST to my brother

### Who is Roy Fielding?

Roy Fielding is one of the authors who build the first web servers, sending document acroos the internet [^1].

### Why don’t the techniques that we use today work well when we need to be able to talk to all of the machines in the world?

Every machine or programming languages have differnt ways of talikng to each other. Fielding and his colleagues aim to build a web, having the ability to "tatlk to any machine anywhere in the world", but "most of the techniques developers later used to get computers to talk to each other didn't have those requirements [^1]".

### What is the HTTP protocol that Fielding and his friends created?

Roy Fielding created many aspects of what is now known as HTTP. His Web architecture dissertation was adopted and end up as a "guiding framework for Web applications [^2]".

### What does a GET do?

The *get method* is used to request data from the web resource [^3]. People often used the wird *get* when searchin g in the internet, Roy Fielding and his community stated building/revising that standard, "allowing users to send and receive hypertext documents [^2]"

### What does a POST do?

The *POST* method is useed to "send data to a server to create/update a resource" [^3]. Tha data sent over this is stored in the HTTP request body.

### What does PUT do?

According to MDN, the *PUT* method can create "a new resource or replaces a representation of the target resource with the request payload [^4]. It means that if the resource target does not have a represebtation, the the *PUT* method can successfully create one, but must inform the user by sending the HTTP code 201 which means *ok or successful*.

### What does PATCH do?

According to MDN, the *PATCH* request can apply "partial modifications to a resource [^5]". It contains instructions or information on how to make partial changes on the resource.

### Request a personal API key from the following APIs. You should receive these in your email within a few hours, often within minutes. Please request these keys prior to lecture to allow adequate time because you will need them in order to complete your lab assignment. Note: do not post your API keys in the Canvas discussion or on GitHub. Save them in a secure place.

Geocoding API
Did you get your API key?  >>> yes

Weather Bit API
Did you get your API key?  >>> Yes

Yelp API Docs
Did you get your API key?   >>>> Not showing where to get

The Movie DB API Docs 
Did you get your API key?   >>>> Yes


[^1]: [A Conversation about REST with my brother](https://gist.github.com/brookr/5977550)
[^2]: [Roy Fielding stands on protocol](https://www.universityofcalifornia.edu/news/roy-fielding-stands-protocol#:~:text=%E2%80%9CI%20did%20not%20invent%20the,version%2C%20HTTP%2F1.1.%E2%80%9D)
[^3]: [HTTP Request Methods](https://www.w3schools.com/tags/ref_httpmethods.asp)
[^4]: [MDN Docs: HTTP PUT](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/PUT)
[^5]: [MDN Docs: HTTP PATCH](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/PATCH)
