<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Watch Terabox Videos</title>
    <link rel="stylesheet" href="styles.css">
    <script>
        function loadVideo() {
            const videoLink = document.getElementById("videoLink").value;
            const videoContainer = document.getElementById("videoContainer");
            if (videoLink) {
                videoContainer.innerHTML = `<iframe width="600" height="400" src="${videoLink}" frameborder="0" allowfullscreen></iframe>`;
            } else {
                videoContainer.innerHTML = "<p>Please enter a valid Terabox video link.</p>";
            }
        }
    </script>
</head>
<body>
    <header>
        <h1>Watch Terabox Videos</h1>
    </header>
    
    <main>
        <h2>Enter Terabox Video Link</h2>
        <input type="text" id="videoLink" placeholder="Enter Terabox video link here" />
        <button onclick="loadVideo()">Load Video</button>
        
        <div id="videoContainer" style="margin-top: 20px;">
            <p>Your video will be displayed here.</p>
        </div>
    </main>
    
    <footer>
        <p>&copy; 2023 Watch Terabox Videos</p>
    </footer>
</body>
</html>
