![[Pasted image 20231004161127.png]]
> One of the oldest ways of rendering content. » The server will generate the full HTML page and return this as the response. » Data from a database or external APl may be included in the page generated. The db connection / API fetch are handled on the server. » No rendering is required on the client. » Every request is handled independently and the server will generate a new response each time » The server processing power is shared by all active users at a given time.

# Diagram
---
![[Pasted image 20231004161228.png]]
> Data Sources Web Server = Database API = 1| Generated ———— = 1| HT™ML Response — L Clent Advantages: Disadvantages: SEO, page linkability, instant first page load. Not good with heavy server requests — slow rendering SSR works if JS is disabled on client Poor user experience All processing on server, no specific requirements Suitable for a straightforward website for the browser easier to deal with errors