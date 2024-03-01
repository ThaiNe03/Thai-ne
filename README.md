<!DOCTYPE html>
<html>
<head>
    <title>Thái nèee</title>
    <link rel="stylesheet" href="tet.css">
    <style>
        #yesButton,#noButton {
            width: fit-content;
            height: fit-content;
        }
        h1{
            color: red;
        }
        .hienthi {
            display: none;
        }
        .active {
            display: inline;
        }
        .img{
            height: 350px;
            width: 350px;
        }
        .img1{
            height: 350px;
            width: 350px;
        }
    </style>
</head>
<body>
        <div class="hienthi">
            <form action="">
                <h2>Chuẩn chuẩn ròi đó</h2>
                <h3>Cảm ơn em nha</h3>
                <img class="img" src="https://i.pinimg.com/originals/17/87/f6/1787f6dcd793e1221f3ea874835b1764.gif" alt="">
            </form>
        </div>
        <div class="home">
            <div>
                <h1>Thấy giỏi khong nè 😊</h1>
                <img class="img1" src="https://i.pinimg.com/originals/dc/b9/6f/dcb96f174bb3e9615a4f7d5e9e161f14.gif" alt="Your GIF">
            </div>
            <div class="footer">
                <button id="yesButton">Chắc chắn là có</button>
                <button id="noButton">Không nha</button>
            </div>
        </div>
    <script>
        document.getElementById('noButton').addEventListener('click', function() {
            var yesButton = document.getElementById('yesButton');
            var style = window.getComputedStyle(yesButton);
            yesButton.style.width = (parseInt(style.width) * 1.5) + 'px';
            yesButton.style.height = (parseInt(style.height) * 1.5) + 'px';
            var hienthi = document.querySelector('.hienthi');
            hienthi.classList.remove('active');
        });
        document.getElementById('yesButton').addEventListener('click', function() {
            var hienthi = document.querySelector('.hienthi');
            var home = document.querySelector('.home');
            hienthi.classList.add('active');
            home.classList.add('hienthi');
        });
    </script>
</body>
</html>
