<!DOCTYPE html>
<html>
<head>
    <title>Cek Bilangan Ganjil atau Genap</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
        }

        input[type="number"] {
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            width: 200px;
        }

        button {
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        #hasil {
            font-size: 20px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>Cek Bilangan Ganjil atau Genap</h1>
    <input type="number" id="bilangan" placeholder="Masukkan bilangan">
    <button onclick="cekBilangan()">Cek</button>
    <p id="hasil"></p>

    <script>
        function cekBilangan() {
            const bilangan = document.getElementById('bilangan').value;
            const hasil = document.getElementById('hasil');

            if (bilangan % 2 === 0) {
                hasil.textContent = bilangan + " adalah bilangan genap.";
            } else {
                hasil.textContent = bilangan + " adalah bilangan ganjil.";
            }
        }
    </script>
</body>
</html>
