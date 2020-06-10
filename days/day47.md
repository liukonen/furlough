# Day 47
## MongoDB Live Conference Day 2
- Advanced Schema Design Patterns
- Improve Reads in Your Sharded Cluster with Hedged Reads 
    - (and THEY ran into network issues while he was talking about network issues)
- Build an ASP.NET app with the Mongo C SDK
- [Community Cafe] An Introduction to MongoDB
- Client-Side Field Level Encryption: Protecting the Most Sensitive Workloads



## Dev Notes
Spent a GOOD chunck of time on my Nats app, getting indexing to work yesterday... it drove me a bit baty...

Who knew there was a difference between

``` c#
    public class Files
    {
        public Int64 Id;
        public DateTime LastModified;
        public string Name;
    }

```

and 

``` c#
    public class Files
    {
        public Int64 Id { get; set; }
        public DateTime LastModified { get; set; }
        public string Name { get; set; }
    }
```

especially when VS tells you to use the former.