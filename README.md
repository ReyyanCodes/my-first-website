 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>ZT Ultra 2 - Online Store</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background: #f4f6f8;
            color: #222;
        }

        /* Header */
        header {
            background: #111827;
            color: white;
            padding: 18px 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        header h1 {
            font-size: 25px;
        }

        header span {
            color: #38bdf8;
        }

        /* Product */
        .container {
            max-width: 1000px;
            margin: 50px auto;
            padding: 20px;
        }

        .product {
            background: white;
            border-radius: 18px;
            padding: 30px;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            box-shadow: 0 8px 30px rgba(0,0,0,0.1);
        }

        /* Image */
        .product-image {
            text-align: center;
        }

        .product-image img {
            width: 100%;
            max-width: 420px;
            height: 420px;
            object-fit: contain;
            border-radius: 15px;
            background: #f1f5f9;
        }

        .upload-label {
            display: inline-block;
            margin-top: 15px;
            background: #e5e7eb;
            padding: 10px 15px;
            border-radius: 8px;
            cursor: pointer;
        }

        #imageUpload {
            display: none;
        }

        /* Details */
        .details h2 {
            font-size: 36px;
            margin-bottom: 10px;
        }

        .rating {
            color: #f59e0b;
            margin-bottom: 20px;
        }

        .price {
            font-size: 30px;
            font-weight: bold;
            color: #16a34a;
            margin: 20px 0;
        }

        .description {
            color: #555;
            line-height: 1.6;
            margin-bottom: 25px;
        }

        /* Colors */
        .option-title {
            font-weight: bold;
            margin-bottom: 10px;
        }

        .colors {
            display: flex;
            gap: 12px;
            margin-bottom: 25px;
        }

        .color {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            border: 3px solid white;
            box-shadow: 0 0 0 1px #aaa;
            cursor: pointer;
        }

        .color.selected {
            box-shadow: 0 0 0 3px #2563eb;
        }

        .black {
            background: black;
        }

        .silver {
            background: silver;
        }

        .blue {
            background: #2563eb;
        }

        .gold {
            background: #eab308;
        }

        /* Quantity */
        .quantity {
            display: flex;
            align-items: center;
            gap: 15px;
            margin-bottom: 25px;
        }

        .quantity button {
            width: 35px;
            height: 35px;
            border: none;
            background: #e5e7eb;
            font-size: 20px;
            cursor: pointer;
            border-radius: 5px;
        }

        #quantity {
            font-size: 18px;
            font-weight: bold;
        }

        /* Buy Button */
        .buy-btn {
            width: 100%;
            padding: 16px;
            border: none;
            border-radius: 10px;
            background: #2563eb;
            color: white;
            font-size: 18px;
            font-weight: bold;
            cursor: pointer;
            transition: 0.3s;
        }

        .buy-btn:hover {
            background: #1d4ed8;
            transform: translateY(-2px);
        }

        /* Payment Box */
        .payment {
            display: none;
            margin-top: 25px;
            padding: 20px;
            border-radius: 12px;
            background: #ecfdf5;
            border: 1px solid #86efac;
        }

        .payment h3 {
            margin-bottom: 12px;
            color: #15803d;
        }

        .easypaisa {
            font-size: 20px;
            font-weight: bold;
            margin: 10px 0;
        }

        .payment input {
            width: 100%;
            padding: 12px;
            margin-top: 10px;
            border: 1px solid #ccc;
            border-radius: 7px;
        }

        .confirm-btn {
            margin-top: 12px;
            width: 100%;
            padding: 12px;
            border: none;
            border-radius: 7px;
            background: #16a34a;
            color: white;
            cursor: pointer;
            font-weight: bold;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 25px;
            background: #111827;
            color: white;
            margin-top: 50px;
        }

        /* Mobile */
        @media (max-width: 750px) {
            .product {
                grid-template-columns: 1fr;
            }

            .details h2 {
                font-size: 28px;
            }

            .product-image img {
                height: 300px;
            }
        }
    </style>
</head>

<body>

    <header>
        <h1>ZT <span>STORE</span></h1>
        <p>Online Shopping</p>
    </header>

    <div class="container">

        <div class="product">

            <!-- Product Image -->
            <div class="product-image">

                <!-- Change this image URL to your own product picture -->
                <img
                    id="productImage"
                    src="https://via.placeholder.com/500x500.png?text=ZT+Ultra+2"
                    alt="ZT Ultra 2"
                >

                <label class="upload-label">
                    📷 Choose Product Picture
                    <input type="file" id="imageUpload" accept="image/*">
                </label>

            </div>


            <!-- Product Details -->
            <div class="details">

                <h2>ZT Ultra 2</h2>

                <div class="rating">
                    ★★★★★ <span style="color:#555;">4.8/5</span>
                </div>

                <div class="price">
                    Rs. 1,500
                </div>

                <p class="description">
                    Experience the ZT Ultra 2 with a stylish design
                    and modern look. Choose your favorite color and
                    place your order easily.
                </p>


                <!-- Colors -->
                <p class="option-title">Choose Color:</p>

                <div class="colors">

                    <div
                        class="color black selected"
                        data-color="Black"
                        title="Black">
                    </div>

                    <div
                        class="color silver"
                        data-color="Silver"
                        title="Silver">
                    </div>

                    <div
                        class="color blue"
                        data-color="Blue"
                        title="Blue">
                    </div>

                    <div
                        class="color gold"
                        data-color="Gold"
                        title="Gold">
                    </div>

                </div>

                <p>
                    Selected Color:
                    <strong id="selectedColor">Black</strong>
                </p>

                <br>


                <!-- Quantity -->
                <p class="option-title">Quantity:</p>

                <div class="quantity">

                    <button onclick="changeQuantity(-1)">
                        −
                    </button>

                    <span id="quantity">1</span>

                    <button onclick="changeQuantity(1)">
                        +
                    </button>

                </div>


                <!-- Buy Button -->
                <button class="buy-btn" onclick="showPayment()">
                    🛒 Buy Now
                </button>


                <!-- Payment -->
                <div class="payment" id="paymentBox">

                    <h3>💳 EasyPaisa Payment</h3>

                    <p>
                        Send your payment to:
                    </p>

                    <div class="easypaisa">
                        📱 03339059199
                    </div>

                    <p>
                        Total Amount:
                        <strong id="totalPrice">Rs. 1,500</strong>
                    </p>

                    <p>
                        After sending the payment, enter your
                        name and contact number below.
                    </p>

                    <input
                        type="text"
                        id="customerName"
                        placeholder="Your Name"
                    >

                    <input
                        type="text"
                        id="customerPhone"
                        placeholder="Your Phone Number"
                    >

                    <button
                        class="confirm-btn"
                        onclick="confirmOrder()">
                        Confirm Order
                    </button>

                </div>

            </div>

        </div>

    </div>


    <footer>
        © 2026 ZT Store | All Rights Reserved
    </footer>


    <script>

        /* Quantity */
        let quantity = 1;

        function changeQuantity(amount) {

            quantity += amount;

            if (quantity < 1) {
                quantity = 1;
            }

            document.getElementById("quantity").innerText = quantity;

            updatePrice();
        }


        /* Update price */
        function updatePrice() {

            let price = 1500;

            let total = price * quantity;

            document.getElementById("totalPrice").innerText =
                "Rs. " + total.toLocaleString();
        }


        /* Color selection */
        const colors = document.querySelectorAll(".color");

        colors.forEach(function(color) {

            color.addEventListener("click", function() {

                colors.forEach(function(item) {
                    item.classList.remove("selected");
                });

                this.classList.add("selected");

                document.getElementById("selectedColor").innerText =
                    this.dataset.color;

            });

        });


        /* Upload product picture */
        document.getElementById("imageUpload")
        .addEventListener("change", function(event) {

            const file = event.target.files[0];

            if (file) {

                const imageURL = URL.createObjectURL(file);

                document.getElementById("productImage").src =
                    imageURL;
            }

        });


        /* Show payment */
        function showPayment() {

            document.getElementById("paymentBox").style.display =
                "block";

            document.getElementById("paymentBox")
                .scrollIntoView({
                    behavior: "smooth"
                });
        }


        /* Confirm order */
        function confirmOrder() {

            const name =
                document.getElementById("customerName").value;

            const phone =
                document.getElementById("customerPhone").value;

            const color =
                document.getElementById("selectedColor").innerText;

            if (name === "" || phone === "") {

                alert("Please enter your name and phone number.");

                return;
            }

            alert(
                "Order details:\n\n" +
                "Product: ZT Ultra 2\n" +
                "Color: " + color + "\n" +
                "Quantity: " + quantity + "\n" +
                "Total: Rs. " + (1500 * quantity) +
                "\n\nThank you, " + name + "!"
            );

        }

    </script>

</body>
</html>