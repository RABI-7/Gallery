# Ex.08 Design of Interactive Image Gallery
# Date:06/05/2025
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Photo Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #000000;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            padding: 20px;
        }

        .gallery-item {
            position: relative;
            overflow: hidden;
            border-radius: 10px;
            cursor: pointer;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.3s ease;
        }

        .gallery-item:hover img {
            transform: scale(1.5);
        }
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .modal img {
            max-width: 90%;
            max-height: 90%;
            border: 4px solid white;
            border-radius: 10px;
        }

        .modal span {
            position: absolute;
            top: 20px;
            right: 40px;
            font-size: 30px;
            color: white;
            cursor: pointer;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <br>
    <br>
    <br>

    <h1 style="text-align: center; margin-top: 20px; color: #fff;">Interactive Photo Gallery</h1>
    <h3 style="text-align: center; margin-top: 20px; color: #fff;">RABI BASKAR PRABURAJAN(24001812)</h3>
     <br>
     <br>
     <br>
     <br>
     <br>

    <div class="gallery">
        <div class="gallery-item" data-image="image1.jpg">
            <img src="hector fort.jpg" alt="Photo 1" onclick="openModal(this)">
        </div>
        <div class="gallery-item" data-image="image2.jpg">
            <img src="jude bellingham.jpg" alt="Photo 2" onclick="openModal(this)">
        </div>
        <div class="gallery-item" data-image="image3.jpg">
            <img src="Ronaldo.jpg" alt="Photo 3" onclick="openModal(this)">
        </div>
        <div class="gallery-item" data-image="image3.jpg">
          <img src="neymar.jpg" alt="Photo 3" onclick="openModal(this)">
      </div>
      <div class="gallery-item" data-image="image3.jpg">
        <img src="Lamine yamal.jpg" alt="Photo 3" onclick="openModal(this)">
    </div>
    <div class="gallery-item" data-image="image3.jpg">
      <img src="mbappe.jpg" alt="Photo 3" onclick="openModal(this)">
  </div>
        
    </div>

    <div class="modal" id="imageModal">
        <span onclick="closeModal()">&times;</span>
        <img id="modalImage" src="" alt="">
    </div>

    <script>
        function openModal(image) 
        {
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImage');
            modal.style.display = 'flex';
            modalImg.src = image.src;
        }
        function closeModal() 
        {
            const modal = document.getElementById('imageModal');
            modal.style.display = 'none';
        }
    </script>

</body>
</html>

```
# OUTPUT:
![Screenshot (94)](https://github.com/user-attachments/assets/8f9575c4-42c6-48b5-8c87-44c26fda88b2)
![Screenshot (95)](https://github.com/user-attachments/assets/2dedb180-b24e-44d6-bb88-dbcb463b8e68)
![Screenshot (96)](https://github.com/user-attachments/assets/17bbc164-a1c3-4244-a2ec-f13b622ca77c)
![Screenshot (97)](https://github.com/user-attachments/assets/5c40d54b-163f-4b10-bdf3-c42a645f2993)
![Screenshot (98)](https://github.com/user-attachments/assets/2d2f39fa-cc53-4552-bdf6-9d03b02892b9)
![Screenshot (99)](https://github.com/user-attachments/assets/3673bed2-a39e-4bf1-9f74-753fd98b9a89)
![Screenshot (100)](https://github.com/user-attachments/assets/4e199035-f30c-483e-b81e-8f377bf39308)



# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
