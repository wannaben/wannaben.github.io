# Welcome to My Website

Please select an option:

- [Homepage](index.md)
- [Contact](contact.md)

<a href="https://www.dynamsoft.com/barcode-reader/downloads">Dynamsoft website</a> == $0
<a href="https://www.dynamsoft.com/barcode-reader/docs/web/programming/javascript/api-reference/BarcodeScanner.html?ver=9.6.20&amp;utm_source=guide#singleframemode">Single Frame Mode</a> == $0

<video id="myVideo" controls width="400" autoplay="true">
    <source src="https://tst.dynamsoft.com/public/docs/dbr/javascript/How%20to%20Use%20Dynamsoft%20Barcode%20Reader%20JavaScript%20SDK%20v1.1.mp4">
</video>

<script>
    const autoplayFlag = localStorage.getItem('autoplay');
    const expirationKey = 'expiration';

    if (!autoplayFlag) {
        // Autoplay the video if the flag doesn't exist
        const videoElement = document.getElementById('myVideo');
        videoElement.autoplay = true;

        // Set the autoplay flag and expiration time in localStorage
        localStorage.setItem('autoplay', 'true');
        const expirationTime = new Date().getTime() + 24 * 60 * 60 * 1000; // 24 hours
        localStorage.setItem(expirationKey, expirationTime);
    } else {
        // Check if the expiration time has passed
        const expirationTime = localStorage.getItem(expirationKey);
        const currentTime = new Date().getTime();

        if (expirationTime && currentTime > parseInt(expirationTime)) {
            // Remove the expired flag and expiration time
            localStorage.removeItem('autoplay');
            localStorage.removeItem(expirationKey);

            // Autoplay the video for the current visit
            const videoElement = document.getElementById('myVideo');
            videoElement.autoplay = true;

            // Set the new autoplay flag and expiration time
            localStorage.setItem('autoplay', 'true');
            const newExpirationTime = new Date().getTime() + 24 * 60 * 60 * 1000; // 24 hours
            localStorage.setItem(expirationKey, newExpirationTime);
        } else {
            // Video autoplay is disabled for subsequent visits
            const videoElement = document.getElementById('myVideo');
            videoElement.autoplay = false;
        }
    }
</script>

