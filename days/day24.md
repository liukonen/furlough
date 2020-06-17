# Day 24

While I know it, I figured I'd brush up on [Web API Design](https://channel9.msdn.com/Series/Web-API-Design)... with more focus on my part on the design part.

- [video 1](https://channel9.msdn.com/Series/Web-API-Design/01)
    - High level of what it is
    - learned a new TLA, HATEOAS (Hypermedia as the Engine of Application State)
    - my focus has always been on the response... may get a lot of learning on the put and post design aspects
- [video 2](https://channel9.msdn.com/Series/Web-API-Design/02)
    - Idea of having put or modifications wrapped in a transaction or separate object, to enforce validation on objects
    -nice tool you can include with your API. Web API 2.2 Help page
        -generates documentation for your API
        - a nugget package you can add
        - powered by MVC, so those decencies need to exist
        
- Took a small break, as someone on Slack pointed out a webinar on UX design, which has been a week spot of mine, I think
    - [DataArt Webinar](https://www.dataart.com/industry/events/free-ux-webinar-best-tools-tips-and-tricks-for-the-fast-virtual-creation-of-ux-concepts). Best tools, tips, & tricks for the fast (virtual) creation of UX concepts 
        - didn't get a lot out of this. The focus was on how to understand the question and workshop out problems and understand and knowledge gather
        - a lot of it is powered by knowledge gathering and wireframing

during the break I had some network issues at my place. This in turn killed my chatbot. I do have a potential retry logic fix that I want to implement, but it may take a bit... will implement the code on the next breaking issue (damn TWC / Spectrum)

- [video 3](https://channel9.msdn.com/Series/Web-API-Design/03)
    - cool, you can have custom formatters on your response objects, by changing your request type (my one app at work has a different API call, but could try changing it to this)
    - header tag attributes on the function can overwrite and / or indicate the function to be called based on the URL
    - 
- [video 4](https://channel9.msdn.com/Series/Web-API-Design/04)
    - from body and from uri can help
    -errors can return while also returning a payload
    - Aprove list rather than deny list items part of request
    - there are built-in helper classes for responses/conflicts, etc
    - you can have special exception messages that are reusable
    - you can overload exceptions, and filter / apply special errors to the exception (could we do this on service contracts at work I wonder?)
    
    That all said.. by this point, my head is hurting from the amount of info I've taken in... I could keep going, however, I feel like I wouldn't get a lot out of video 5 and 6 today.
    Besides, I'm starting to run low on training items that I can think of, so I'm calling it a day. 