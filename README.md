# Hello-lang-ai.github.io
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Movie Selection</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
        }
        .container {
            display: flex;
            flex-direction: column;
            width: 100vw;
            max-width: 1200px;
            margin: 0 auto;
        }
        .nav-container {
            background-color: #fff;
            padding: 1rem;
            border-bottom: 1px solid #cccccc;
            width: 100vw;
        }
        .nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }
        .nav-link {
            font-size: 1.25rem;
            font-weight: bold;
            text-decoration: none;
            color: #333;
            padding: 0.5rem;
            transition: color 0.3s ease;
            border-radius: 0.5rem;
            background-color: transparent;
            margin-right: 1rem;
        }
        .nav-link:hover {
            color: #fff;
            background-color: #333;
        }
        .movie-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            margin: 2rem 0;
        }
        .movie {
            position: relative;
            width: 200px;
            height: 300px;
            margin: 1rem;
            transition: transform 0.3s ease;
            overflow: hidden;
            border-radius: 1rem;
            box-shadow: 0 19px 38px -10px #cccccc, 0 15px 12px 0px #cccccc, 0 8px 20px 5px #cccccc;
            background-color: #fff;
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            border: 1px solid #cccccc;
        }
        .Movie:hover {
            transform: scale(1.1);
        }
        .Movie-img {
            position: absolute;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            object-fit: cover;
            transition: transform 0.3s ease;
        }
        .Movie:hover .Movie-img {
            transform: scale(1.2);
            z-index: 1;
        }
        .Movie-content {
            padding: 1rem;
            z-index: 0;
        }
        .Movie-name {
            font-size: 1.5rem;
            font-weight: bold;
            margin-top: 1rem;
            text-align: center;
            color: #fff;
            background-color: #333;
            padding: 0.5rem 1rem;
            border-radius: 0.5rem;
            position: absolute;
            bottom: 0;
            width: 100vw;
            transform: translateY(100%);
            opacity: 0;
            transition: transform 0.3s ease, opacity 0.3s;
        }
        .Movie:hover .Movie-name {
            transform: translateY(0%);
            opacity: 1;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="nav-container">
            <div class="nav">
                <a href="#" class="nav-link">Home</a>
                <a href="#" class="nav-link">Movies</a>
                <a href="#" class="nav-link">TV Shows</a>
                <a href="#" class="nav-link">Contact</a>
            </div>
        </div>
        <div class="Movie-container">
            <div class="Movie" style="background-image: url(<Movie Poster URL>);">
                <a href="#" class="Movie-img"></a>
                <div class="Movie-content">
                    <h2 class="Movie-name">Movie Name</h2>
                </div>
            </div>
            <!-- Add more Movie containers with unique poster URLs and names -->
        </div>
    </div>
</body>
</html>
