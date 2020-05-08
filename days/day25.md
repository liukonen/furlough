# Day 25

Happy friday


Start of the morning, my network was down partly overnight, which means my chatbot was down. Wrote some code that should fix this, where if there is a network hicup, we try to reconnect after waiting 30 second.

Got back to Web API.

- [Video 5 - Web API Security](https://channel9.msdn.com/Series/Web-API-Design/05)
	- Mostly Authentication, but some cross site 
		- Authentication on the host (default assumtion by web api)
			- None, individual user (other providers), Organizational (Azure active directory), and windows
		-Authentication using message handlers
			- part of the pipeline, override sendasync
			- base function still needs authenitcation
		- Token based authentication
	-Autherization Filters
		- users and roles
		- override the OnAuthorization
	- Cross Site
		- Cookies
		- Token on server (shared key on all servers)
- [Video 6 advanced](https://channel9.msdn.com/Series/Web-API-Design/06)
	- Look into type converters! looks like a handly item to work with (its part of the framework)

Second half of my day, after watching the presidential breafing, was to start reworking my chatbot I have running on slack in a different language, as it is painfully slow, and I know it's the python riverscript aspect that is the painpoint. I downloaded a C# edition, and spent much of the afternoon trying to get it to work... it would not... I mean, I was able to load everything up, but for whatever reason, a simple "hello" would not work. Since there platform isn't offically supported, I might try the Go version, that is, once I learn Go.... which I plan to next week.

