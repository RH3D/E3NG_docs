---
title: 
layout: default
#parent: Into the project
#has_children: true
#nav_order: 7
---
<!DOCTYPE html>
<html lang="cs">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>E3NG Color Scheme helper</title>
    <style>
        body {
            /*display: flex;
            flex-direction: column;*/
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
        }
        .container {
            position: relative;
            width: 500px; /* Nastavení pevné šířky */
            height: 500px; /* Nastavení pevné výšky */
        }
        .background-image, .foreground-image, .foreground-image-2, .overlay-image {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: contain; /* Zachování poměru stran */
        }
        .background-image {
            z-index: 1;
        }
        .foreground-image {
            z-index: 2;
        }
        .foreground-image-2 {
            z-index: 3;
        }
        .overlay-image {
            z-index: 4; /* Nový obrázek překrývající ostatní */
        }
        .slider-container {
            margin: 10px 0;
            display: flex;
            align-items: center;
        }
        .slider {
            width: 100%;
            margin-left: 10px;
        }
        .number-input {
            width: 40px;
        }
        .sliders-group {
            display: flex;
            justify-content: space-between;
            width: 30%;
            margin-top: 20px; /* Přidání mezery mezi obrázkem a posuvníky */
        }
        .sliders-column {
            display: flex;
            flex-direction: column;
            align-items: right;
            width: 47%; /* Zmenšení šířky sloupců */
        }
    </style>
</head>
<body>
    <h1>E3NG color scheme config</h1>
    <div class="container">
        <img class="background-image" src="background-image.png" alt="Pozadí" onerror="alert('Pozadí se nepodařilo načíst')">
        <img class="foreground-image" id="foreground-image" src="foreground-image.png" alt="Květináč 1" onerror="alert('Květináč 1 se nepodařilo načíst')">
        <img class="foreground-image-2" id="foreground-image-2" src="foreground-image-2.png" alt="Květináč 2" onerror="alert('Květináč 2 se nepodařilo načíst')">
        <img class="overlay-image" id="overlay-image" src="overlay-image.png" alt="Překrývající obrázek" onerror="alert('Překrývající obrázek se nepodařilo načíst')">
    </div>
    <div class="sliders-group">
        <div class="sliders-column">
            <h2>ACCENT COLOR</h2>
            <div class="slider-container">
                <label for="brightness">BRI</label>
                <input type="number" id="brightness-number" class="number-input" min="0" max="100" value="50">
                <input type="range" id="brightness" class="slider" min="0" max="100" value="50">
            </div>
            <div class="slider-container">
                <label for="saturation">SAT</label>
                <input type="number" id="saturation-number" class="number-input" min="0" max="100" value="50">
                <input type="range" id="saturation" class="slider" min="0" max="100" value="50">
            </div>
            <div class="slider-container">
                <label for="hue">HUE</label>
                <input type="number" id="hue-number" class="number-input" min="0" max="100" value="0">
                <input type="range" id="hue" class="slider" min="0" max="100" value="0">
            </div>
        </div>
        <div class="sliders-column">
            <h2>MAIN COLOR</h2>
            <div class="slider-container">
                <label for="brightness-2">BRI</label>
                <input type="number" id="brightness-number-2" class="number-input" min="0" max="100" value="50">
                <input type="range" id="brightness-2" class="slider" min="0" max="100" value="50">
            </div>
            <div class="slider-container">
                <label for="saturation-2">SAT</label>
                <input type="number" id="saturation-number-2" class="number-input" min="0" max="100" value="50">
                <input type="range" id="saturation-2" class="slider" min="0" max="100" value="50">
            </div>
            <div class="slider-container">
                <label for="hue-2">HUE</label>
                <input type="number" id="hue-number-2" class="number-input" min="0" max="100" value="0">
                <input type="range" id="hue-2" class="slider" min="0" max="100" value="0">
            </div>
        </div>
    </div>

    <script>
        const foregroundImage = document.getElementById('foreground-image');
        const brightnessSlider = document.getElementById('brightness');
        const brightnessNumber = document.getElementById('brightness-number');
        const saturationSlider = document.getElementById('saturation');
        const saturationNumber = document.getElementById('saturation-number');
        const hueSlider = document.getElementById('hue');
        const hueNumber = document.getElementById('hue-number');

        const foregroundImage2 = document.getElementById('foreground-image-2');
        const brightnessSlider2 = document.getElementById('brightness-2');
        const brightnessNumber2 = document.getElementById('brightness-number-2');
        const saturationSlider2 = document.getElementById('saturation-2');
        const saturationNumber2 = document.getElementById('saturation-number-2');
        const hueSlider2 = document.getElementById('hue-2');
        const hueNumber2 = document.getElementById('hue-number-2');

        const overlayImage = document.getElementById('overlay-image');

        function updateImage(image, brightness, saturation, hue) {
            image.style.filter = `brightness(${brightness * 2}%) saturate(${saturation * 2}%) hue-rotate(${hue * 3.6}deg)`;
        }

        function syncSlidersAndNumbers(slider, number, image, type, otherSliders) {
            slider.addEventListener('input', () => {
                number.value = slider.value;
                if (type === 'brightness') {
                    updateImage(image, slider.value, otherSliders.saturation.value, otherSliders.hue.value);
                } else if (type === 'saturation') {
                    updateImage(image, otherSliders.brightness.value, slider.value, otherSliders.hue.value);
                } else if (type === 'hue') {
                    updateImage(image, otherSliders.brightness.value, otherSliders.saturation.value, slider.value);
                }
            });
            number.addEventListener('input', () => {
                slider.value = number.value;
                if (type === 'brightness') {
                    updateImage(image, number.value, otherSliders.saturation.value, otherSliders.hue.value);
                } else if (type === 'saturation') {
                    updateImage(image, otherSliders.brightness.value, number.value, otherSliders.hue.value);
                } else if (type === 'hue') {
                    updateImage(image, otherSliders.brightness.value, otherSliders.saturation.value, number.value);
                }
            });
        }

        syncSlidersAndNumbers(brightnessSlider, brightnessNumber, foregroundImage, 'brightness', {saturation: saturationSlider, hue: hueSlider});
        syncSlidersAndNumbers(saturationSlider, saturationNumber, foregroundImage, 'saturation', {brightness: brightnessSlider, hue: hueSlider});
        syncSlidersAndNumbers(hueSlider, hueNumber, foregroundImage, 'hue', {brightness: brightnessSlider, saturation: saturationSlider});

        syncSlidersAndNumbers(brightnessSlider2, brightnessNumber2, foregroundImage2, 'brightness', {saturation: saturationSlider2, hue: hueSlider2});
        syncSlidersAndNumbers(saturationSlider2, saturationNumber2, foregroundImage2, 'saturation', {brightness: brightnessSlider2, hue: hueSlider2});
        syncSlidersAndNumbers(hueSlider2, hueNumber2, foregroundImage2, 'hue', {brightness: brightnessSlider2, saturation: saturationSlider2});
    </script>
</body>
</html>
