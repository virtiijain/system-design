# How the Web Works

## Diagram
```
you type google.com
        │
        ▼
  browser cache ── found? → done ✓
        │ not found
        ▼
  ISP DNS resolver
        │
        ▼
  root nameserver → "go to .com"
        │
        ▼
  .com nameserver → "go to google"
        │
        ▼
  google nameserver → IP = 142.250.77.46
        │
        ▼
  browser sends HTTP request to IP
        │
        ▼
  google server → sends HTML, CSS, JS
        │
        ▼
  browser renders → page appears ✓
```

## Interview Questions

**Q1. What happens when you type google.com in browser?**
> "First the browser checks its local cache for the IP. If not found, it queries the DNS server which resolves google.com to an IP address. Then the browser sends an HTTP request to that IP. Google's server processes the request and sends back HTML, CSS and JavaScript. The browser then renders this into the visible page."

**Q2. What is DNS?**
> "DNS stands for Domain Name System. It acts as the phonebook of the internet — it translates human readable domain names like google.com into IP addresses that computers use to identify each other."

**Q3. What is the difference between HTTP and HTTPS?**
> "HTTP is HyperText Transfer Protocol — the language used for communication between browser and server. HTTPS is the secure version — it encrypts the data using SSL/TLS so that no one can intercept it. Any sensitive site like banking or login pages must use HTTPS."

**Q4. What is an IP address?**
> "An IP address is a unique numerical label assigned to every device on a network. It works like a home address — it tells the internet exactly where to send the data."

**Q5. What is latency in context of web?**
> "Latency is the time taken for a request to travel from the client to the server and back. High latency means slow page loads. System design techniques like CDN and caching are used to reduce latency."

**Q6. What is rendering?**
> "Rendering is the process where the browser takes the HTML, CSS and JavaScript received from the server and converts it into the visual page that the user sees on screen."
