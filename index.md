
THIS IS A TEST ONLY

<video controls width="400" autoplay="true">
    <source src="https://tst.dynamsoft.com/public/docs/dbr/javascript/How%20to%20Use%20Dynamsoft%20Barcode%20Reader%20JavaScript%20SDK%20v1.1.mp4">
</video>

<script>
    // Check if autoplay flag exists in sessionStorage
    const autoplayFlag = sessionStorage.getItem('autoplay');

    if (!autoplayFlag) {
        // Autoplay the video if the flag doesn't exist
        const videoElement = document.getElementById('myVideo');
        videoElement.autoplay = true;

        // Set the autoplay flag in sessionStorage
        sessionStorage.setItem('autoplay', 'true');
    }
</script>

# Welcome to My Website

Please select an option:

- [About](about.md)
- [Contact](contact.md)


