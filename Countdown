Given your birthdate, October 17, 2004, your 25th birthday will be on October 17, 2029. Here’s the HTML code with that date:

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Countdown to 25th Birthday</title>
    <style>
        body { font-family: Arial, sans-serif; display: flex; justify-content: center; align-items: center; height: 100vh; text-align: center; }
        #countdown { font-size: 2rem; }
        #message { display: none; font-size: 1.5rem; color: green; }
    </style>
</head>
<body>
    <div id="countdown"></div>
    <div id="message">I hope it was all worth it.</div>

    <script>
        // Target date: your 25th birthday
        const targetDate = new Date("2029-10-17T00:00:00").getTime();
        
        const countdownElement = document.getElementById('countdown');
        const messageElement = document.getElementById('message');
        
        // Update countdown function
        function updateCountdown() {
            const now = new Date().getTime();
            const timeLeft = targetDate - now;
            
            if (timeLeft <= 0) {
                countdownElement.style.display = 'none';
                messageElement.style.display = 'block';
                clearInterval(interval);
            } else {
                const days = Math.floor(timeLeft / (1000 * 60 * 60 * 24));
                const hours = Math.floor((timeLeft % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
                const minutes = Math.floor((timeLeft % (1000 * 60 * 60)) / (1000 * 60));
                const seconds = Math.floor((timeLeft % (1000 * 60)) / 1000);
                
                countdownElement.innerHTML = `${days} days ${hours} hrs ${minutes} mins ${seconds} secs`;
            }
        }
        
        const interval = setInterval(updateCountdown, 1000);
    </script>
</body>
</html>
