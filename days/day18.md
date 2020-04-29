# Day 18
I decided I needed to work on my homepages resume part... At first I was thinking about building it myself... then thought on how a template could do it for me, and if there was any open source json resume template object I could build off of. Sure enough, I found [JSONResume](https://jsonresume.org/)... researching there site, I found a 3rd party tool to make it that much easier [GitConnected](https://gitconnected.com/), and I copied, tweeked and pasted my linkedin info over to GitConnected. I then saved the page, and found that, sure enough there was a JSON object. I also found that I could, if I want, tie the themes from JSONResume over to my profile. For now though, thinking about it, I decided to host it on GitConnected, and just use an Iframe modal pop up on my homepage to direct to there theme. if GitConnected ever goes under, I have a backup of my resume object, and can build my own page if I want off it.

- Then I decided to learn about the Entity Framework Core learnings - Entity Framework Core [1](https://channel9.msdn.com/Shows/Visual-Studio-Toolbox/Entity-Framework-Core-Part-1) [2](https://channel9.msdn.com/Shows/Visual-Studio-Toolbox/Entity-Framework-Core-Part-2) [3](https://channel9.msdn.com/Shows/Visual-Studio-Toolbox/Entity-Framework-Core-Part-3) [4](https://channel9.msdn.com/Shows/Visual-Studio-Toolbox/Entity-Framework-Core-Part-4) [5](https://channel9.msdn.com/Shows/Visual-Studio-Toolbox/Entity-Framework-Core-Part-5)
    - Entity framework is vastly different under the hood, but simmilar code standard
    - doesnt appear to have SQL stored proc support off hand, but may
    - Need to be carful with tracking changes, as it can lead to a lot of memory pressure.
        - Better sometimes to keep tracking off, especially if you are doing read only
    - There is a speciallized DB set for stored procs... will want to look more into this... wasnt coverted well
    - Careful with linq and when it executes
    - when wanting to include sub tables (like foreign key lookup) with linq, you need to mark the object, and use the include method of the attribute to also grab its data

    
- Participated in a Scrum Kanban Scrumban Discussion
    - The Scrumban Cheat Sheet - Unveiling the brand new version 
    - [link](https://www.youtube.com/watch?v=EjMg9kmd85M)
    - Limit early binding - people should not be taking tasks early
    - more columns - Todo and done, limit WIP limits where you can
        - Hard when you run into obsticals
    - steps 1-5 scrum complient... however arguement made not to give estimates
    - instead, order by priority
    - This works if you are good at story slicing - small managagle tasks
    - also in Scrumban, the workload of items in backlog triggers the need to have a meeting
        - instead of having a sprint planning, when the backlog is light, we start planning
    -[Link to cheat sheet](https://www.developmentthatpays.com/scrumban)
    