<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="FastSave - Download Instagram Reels, YouTube Shorts, and more in HD for free!">
    <title>FastSave - Download Reels & Shorts Instantly</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f5f5f5;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            text-align: center;
        }
        .container {
            background: white;
            border-radius: 15px;
            padding: 30px;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
            max-width: 500px;
            width: 90%;
        }
        h1 {
            color: #ff4d8d;
            font-size: 2.5rem;
            margin-bottom: 10px;
        }
        .tagline {
            color: #666;
            font-size: 1.1rem;
            margin-bottom: 30px;
        }
        .btn {
            display: block;
            width: 100%;
            padding: 15px;
            margin: 15px 0;
            border: none;
            border-radius: 8px;
            font-size: 1.1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        #reel-btn {
            background-color: #ff4d8d;
            color: white;
        }
        #shorts-btn {
            background-color: #ff0000;
            color: white;
        }
        #others-btn {
            background-color: #000000;
            color: white;
        }
        .features {
            margin-top: 30px;
            text-align: left;
            font-size: 0.95rem;
            color: #555;
        }
        .features h2 {
            color: #333;
            font-size: 1.3rem;
            margin-bottom: 10px;
        }
        .features ul {
            padding-left: 20px;
        }
        .features li {
            margin-bottom: 8px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>FastSave</h1>
        <p class="tagline">Download Instagram Reels, YouTube Shorts & More in One Click!</p>
        
        <button id="reel-btn" class="btn" onclick="window.open('https://fastvideosave.net/', '_blank')">Reel Downloader</button>
        <button id="shorts-btn" class="btn" onclick="window.open('https://yt.savetube.me/1kejjj1', '_blank')">Shorts Downloader</button>
        <button id="others-btn" class="btn" onclick="alert('Server is busy. Please try again later.')">Others</button>
        
        <div class="features">
            <h2>Why Choose FastSave?</h2>
            <ul>
                <li>🚀 <strong>Super Fast</strong> - Download videos in seconds.</li>
                <li>🔒 <strong>100% Free</strong> - No hidden charges.</li>
                <li>📱 <strong>No App Needed</strong> - Works directly in your browser.</li>
                <li>💡 <strong>Easy to Use</strong> - Just paste the link and download!</li>
            </ul>
        </div>
    </div>
</body>
</html>
