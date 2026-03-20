# How the Web Works

**Q1. What happens when you type google.com in browser?**
> "First the browser checks its local cache for the IP. If not found, it queries the DNS server which resolves google.com to an IP address. Then the browser sends an HTTP request to that IP. Google's server processes the request and sends back HTML, CSS and JavaScript. The browser then renders this into the visible page."

**Q2. What is DNS?**
> "DNS stands for Domain Name System. It acts as the phonebook of the internet — it translates human readable domain names like google.com into IP addresses like 142.250.77.46 that computers use to identify each other."

**Q3. What is the difference between HTTP and HTTPS?**
> "HTTP is HyperText Transfer Protocol — the language used for communication between browser and server. HTTPS is the secure version — it encrypts the data using SSL/TLS so that no one can intercept it in between. Any sensitive site like banking or login pages must use HTTPS."

**Q4. What is an IP address?**
> "An IP address is a unique numerical label assigned to every device on a network. It works like a home address — it tells the internet exactly where to send the data. For example, Google's IP is 142.250.77.46."

**Q5. What is latency in context of web?**
> "Latency is the time taken for a request to travel from the client to the server and back. In web context, it is the delay between typing a URL and the page appearing. High latency means slow page loads. System design techniques like CDN and caching are used to reduce latency."

**Q6. What is rendering?**
> "Rendering is the process where the browser takes the HTML, CSS and JavaScript received from the server and converts it into the visual page that the user sees on screen."