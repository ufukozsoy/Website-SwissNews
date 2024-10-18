<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Swiss News</h1>

    </header>
    <section class="intro-section"><h1>Welcome to Swiss News</h1></section>
    <style>
        


    </style>
  <section class="news-flash">
    <marquee><p>Best Website in the World</p></marquee>
</section>

<main class="article-section">

    <article class="articles">
       <h2>Switzerland’s priciest street makes room for a bakery shop</h2>
       <button class="speak-button" onclick="speakText('Switzerland’s priciest street makes room for a bakery shop')">Listen</button>
       <img src="image1.png" alt="bakery">
       <p>It is one of the most expensive streets for shopping in Switzerland where jewellery, watches and 
        designer clothes worth tens of thousands of Swiss francs can be purchased. You can now also buy a sandwich here thanks to a new bakery.</p>
    </article>

    <article class="articles">
       <h2>Swiss textile heavyweight Rieter plans further job cuts</h2>
       <img src="image2.png" alt="News image 2">
       <p>Textile machinery manufacturer Rieter is to cut more than 10% of its workforce in Switzerland. 
        This latest restructuring is the latest in a long series for the Zurich-based group, 
        which saw its revenues fall by almost half in the first half of 2024.</p>
    </article>

    <article class="articles">
       <h2>Raw milk:Loophole gives Swiss the freedom to skip pasteurisation</h2>
       <img src="image3.png" alt="News image 3">
       <p>Once considered dangerous, raw milk is now back in people’s fridges. 
        Legislation worldwide is adapting. Switzerland relies on labelling and personal responsibility. </p>
    </article>

</main>
    <footer>
        <p>&copy; 2024 Swiss News</p>
    </footer>

    <script>
        // Function to trigger text-to-speech
        function speakText(text) {
            const speech = new SpeechSynthesisUtterance(text);
            speech.lang = 'en-US'; // Set language to English (adjust as necessary)
            speech.rate = 1; // Speed of speech
            window.speechSynthesis.speak(speech);
        }
    </script>
    
</body>
</html>


* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    background-color: rgb(228, 237, 237);
}

body {
    font-family: Arial, sans-serif;
}

header h1 {
    font-size: 30px;
    text-align: center;
    margin-top: 30px;
}

.intro-section {
    font-size: 30px;
    text-align: center;
    margin-top: 30px; 
}

.news-flash {
    margin-top: 30px;
    text-align: center;
    background-color: rgba(255, 255, 255, 0.8);
}

.article-section {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 20px;
    padding: 20px;
    margin: 30px auto;
    max-width: 1200px;
}

.articles {
    background-color: rgba(255, 255, 255, 0.8);
    padding: 20px;
    font-size: 30px;
    text-align: center;
}

.articles img {
    max-width: 100%;
    height: auto;
}

.articles > h2 {
    font-size: 20px;
    text-align: center;
}

.articles > p {
    font-size: 15px;
    text-align: center;
}

footer {
    color: #0f25a1;
    text-align: center;
    padding: 10px;
    margin-top: 30px;
    background-color: rgba(255, 255, 255, 0.8);
}

.news-flash p {
    margin: 0;
    padding: 10px;
}