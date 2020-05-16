# Day 21

cheated a bit here, as over the weekend  I 
 - worked on my resume part of my site over the weekend
 - as well as helped make my homepage a bit more mobile-friendly.
 - Emailed UWM Lubar School about looking at my resume
 - Signed up for an Agile workshop on Tuesday
 


That said... decided that it might be wise to learn [Angular JS](https://channel9.msdn.com/Series/Introduction-to-AngularJS)

[video 1](https://channel9.msdn.com/Series/Introduction-to-AngularJS/01)
    -Angular is MVC client-side
    - Is also declarative programing
    - reminds me a lot of the template items I am using now

Break, because UWM got back to me, woot

[video 2](https://channel9.msdn.com/Series/Introduction-to-AngularJS/02)
 - Controllers
 - global $scope object... kind of the global modal... what work refers to a view, even though there view is not a view {I know right}
 - scope is global. Can have children scopes, but inherit off base scope
 - scope is not the model, its the "glue" though between the model and the view (model binds to scope, view pulls from scope)
 - Demonstration of a Factory... which can be shared across controllers... but you need to pass it in as a param in the constructor of the controller
    - reminds me a lot of say, a property, but it's not
    - looks more like a "base class" without the limitation of one to many
    - dependency injection
 -controller as function... turns your controller as an object
    - in that way, you don't need scope, instead you can bind against the object output from the as function

[video 3](https://channel9.msdn.com/Series/Introduction-to-AngularJS/03)
 - expressions and filters
 - expressions are just the variables in the HTML... can have low limit if statements, but not for complex items
 - filters. Number of filters, similar to jquery filters
 - ng-repeat acts as a repeater on multiple items :)
 - filters go in expressions, and use a pipe to invoke them
 
[video 4](https://channel9.msdn.com/Series/Introduction-to-AngularJS/04)
  -Directives
    - little chunks of HTML contained
    - ability to have external shared "controls" on a page
[video 5](https://channel9.msdn.com/Series/Introduction-to-AngularJS/05)
  - URL Routing
  - Still a base page, with an ng-view attribute to load the directive into the master page
  - to get true pretty URLs
    - this requires special web server configuration, location provider, setting HTML mode to 5
    - also requires you to set the base of your relative URL
    - otherwise you have a # tag at the end of the base part of your URL
  - UI router another external item with more bells and whistles
    - can change based on applications state
  - both work in similar ways. UI router is more popular
  
[video 6](https://channel9.msdn.com/Series/Introduction-to-AngularJS/06)
- Factories, provider, service
- loading external data
    -$http - build in request
- Service - you are provided a function.
- Factory - you are returned a result that is returned from calling that function.
- Provider - can be configured, are passed back an instance of it.


After playing around I found out that IOS and safari do not like the webp image format. Wrote some JS to load PNG if the browser doesn't support it. The only thing I don't like is the fact the browser still loads the webp, and then loads the png... webp is small enough... I'll think of it as an Apple tax for now, till I figure out something better.