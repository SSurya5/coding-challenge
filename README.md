
## Setup
Forked the repository to my GitHub profile.
Then cloned the repository to my Visual Studio and started my development.
In the new folder, I installed the npm.
Then started the development server.


 ## Building the PDP

1. Reviewed the existing files and planned what has to be built on top of it.
2. I decided to use a Bootstrap 5 template and downloaded it to commence the development. As this will allow easy customization and it has a mobile-first approach. The enhanced components allow us to reuse the code avoiding redundancy and being more efficient. Eg: Toast component used for notification
3. First I built the layout of the page using the “template.liquid” file with a ‘Header (with Nav bar and Cart Icon)’, ‘Body, and ‘Footer’. 
   - Included the Shop Name and a dummy Nav bar to give a proper look and feel.
   - The cart icon on the right of the header is used to display the number of items in the cart. I used JS to get the number of items in the cart, the value of the cart will keep on increasing as the item is successfully added to the cart.
   - I have kept the footer very simple with just copyright details to focus on the design and functionality of the PDP section.

https://github.com/SSurya5/coding-challenge/blob/main/Screenshot%202024-09-09%20at%207.35.46%20PM.png



4. Then, in the “product.liquid”, I started the PDP page by developing its layout with 2 columns, one to display the image, and the other to display the details like Product Title, Price, Stock Status, Description, Variants as Dropdown, Quantity box, and Add to cart button.

    - I used liquid syntax to display the information correctly/dynamically by grabbing the details from the “product.json” file.
    - Included a badge to display the availability of the product, so that the customer is aware of it.
    - The variant (Size) is displayed using the dropdown element. The active element is passed to the server via the “add to cart()” to send the correct details.

https://github.com/SSurya5/coding-challenge/blob/main/Screenshot%202024-09-09%20at%207.36.13%20PM.png

https://github.com/SSurya5/coding-challenge/blob/main/Screenshot%202024-09-09%20at%207.36.30%20PM.png


    - In the “Add to Cart” button, I have included a function via which the selected product details are extracted and used fetch API to make POST request to cart/add.js.

5. If the data is sent successfully, the success message is displayed to the customer. I have used “Toast” plugin from bootstrap to display this message and the message will automatically fade after few seconds avoiding interference with the user experience.

https://github.com/SSurya5/coding-challenge/blob/main/Screenshot%202024-09-09%20at%207.37.12%20PM.png

https://github.com/SSurya5/coding-challenge/blob/main/Screenshot%202024-09-09%20at%207.42.01%20PM.png


6. If there is any error it is rendered in the user console for debugging purposes.

7. All the default CSS are used from the bootstrap to make the styles and responsiveness. The custom CSS is used at places and the class is prefixed with “c-” for easy recognition.


## Improvisation

If I were to improve the current project in a proper Shopify way, I prefer to do the following:

1. I will use separate css file and js file and render them in the liquid file. This is a proper method to maintain the code and avoid any redundancies.
2. Right now, I have included only one image from the JSON file. I would like to include all the images give them a zoom-in option and change the image based on the variant chosen.

## Final Note

I am attaching the screenshot of every step for your easy reference. Please don’t hesitate to reach out to me for the explanation and I would like to explain everything in detail. I am attaching the link to my repository and have also sent a PR.

Thank you so much Rocco and Gabriel for your explanations. I am glad that I was given a chance to come so far.

