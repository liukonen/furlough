# Day 2: 
## Modules 1 and 2 of Intro to MVC
[ASP-NET-MVC](https://channel9.msdn.com/Series/Introduction-to-ASP-NET-MVC/01)

Started diving into the MVC framework and how it works.

- M is model, just a base object that is returned
- C is your controller. When you do a get into the server, it calls the controller directly, sometimes with values, sometimes without. This Controler, holds most of the bussness rules. Think of a handler event call on a winform
- V is the view. Views are nothing more then controls (cshtml, vbhtml, or ascx items) that take the model object the controller returns and generates a control for the master page with it 
