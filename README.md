<!DOCTYPE html>
<!--[if lt IE 7]>      <html class="no-js lt-ie9 lt-ie8 lt-ie7"> <![endif]-->
<!--[if IE 7]>         <html class="no-js lt-ie9 lt-ie8"> <![endif]-->
<!--[if IE 8]>         <html class="no-js lt-ie9"> <![endif]-->
<!--[if gt IE 8]>      <html class="no-js"> <!--<![endif]-->
<html>
	<head>
		<meta charset="utf-8">
		<meta http-equiv="X-UA-Compatible" content="IE=edge">
		<link rel="stylesheet" href="styles.css">
	
		<style>
		.slideshow-container {
            max-width: 1200px;
            position: relative;
            margin: auto;
        }

        /* Ẩn tất cả ảnh mặc định */
        .mySlides {
			display: none;
    		width: 100%;
    		max-width: 600px; /* Giới hạn chiều rộng */
    		margin: auto; /* Căn giữa theo chiều ngang */
		}
			.active {
				display: block
			}
		/* Tăng kích thước ảnh */

img {
    width: 100%;
    border-radius: 10px;
}

/* Nút điều hướng */
.prev, .next {
    position: absolute;
    top: 20%;
    transform: translateY(-50%);
    background-color: rgba(0, 0, 0, 0.5);
    color: white;
    border: none;
    padding: 10px;
    cursor: pointer;
}

.prev { left: 10px; }
.next { right: 10px; }

.prev:hover, .next:hover {
    background-color: rgba(0, 0, 0, 0.8);
}
		</style>
		<title>trang web kĩ thuật</title>
		<meta name="description" content="">
		<meta name="viewport" content="width=device-width, initial-scale=1">
		<link rel="icon" href="picture/462891570_4074011672884558_6889142999978527665_n.jpg">
		<link rel="stylesheet" href="style.css">
		<style>
			.nut-dieu-huong {
				position: fixed;
				top: 20px;
				left: 20px;
				z-index: 1000;
			}
		</style>
	</head>
	<body>
		<header>
        <ul>
            <li class="logo">
                <img  src="picture/pngtree-industrial-factory-factory-line-icon-vector-png-image_13120016.png" alt="Logo Doanh Nghiệp" width=200px height=10px>
				<h1>Chào mừng đến với Cửa Hàng Xe Máy</h1>
				<nav class="navbar">
					<ul class="nav-links">
						<li><a href="index.html">Trang chủ</a></li>
						<li><a href="about.html">Giới thiệu</a></li>
						<li>
							<a href="#">Sản phẩm ▼</a>
							<ul class="dropdown-menu">
								<li><a href="xe-so.html">Xe số</a></li>
								<li><a href="xe-tay-ga.html">Xe tay ga</a></li>
								<li><a href="xe-con-tay.html">Xe côn tay</a></li>
							</ul>
						</li>
						<li><a href="contact.html">Liên hệ</a></li>
						<li><a href="store.html" target="_blank">Cửa hàng</a></li>
					</ul>
				</nav>
			</header>
			
			<section>
				<h2>Sản phẩm nổi bật</h2>
				<p>Danh sách xe máy đang bán...</p>
				<!-- Bạn có thể thêm hình ảnh sản phẩm ở đây -->
			</section>
    </nav>
		</header>
	
		<!-- Banner -->
		<header class="hero">
			<h1 >Cửa hàng xe Duy Nhất kính chào quý khách</h1>
			<p>Chất lượng - Uy tín - Giá tốt nhất</p>
			<a href="#" class="btn">Khám phá ngay</a>
		</header>
		<div class="slideshow-container">
			<div class="swiper-wrapper">
			<img class="mySlides" src="picture/474146112_4157643974521327_908606949127112153_n.jpg" alt= ảnh 1>
			<img class="mySlides" src="picture/474364831_4157642524521472_7494803716688900304_n.jpg" alt=ảnh 2>
			<img class="mySlides" src="picture/474459857_4157643871188004_7842900903028145483_n.jpg" alt="ảnh 3">
			<button class="prev" onclick="plusSlides(-1)">❮</button>
			<button class="next" onclick="plusSlides(1)">❯</button>
		</div>
		
		<div class="container">
			<h2>Danh sách sản phẩm</h2>
			<div class="product-grid">
				<div class="product">
					<img src="picture về sản phẩm/474068627_4157646707854387_1024257364806248234_n.jpg" alt="giá hàng gọn nhẹ">
					<h3>giá hàng nhỏ</h3>
					<p>Giá: 500.000 VNĐ</p>
				</div>
				<div class="product">
					<img src="picture về sản phẩm/474214578_4156950381257353_4833224894200174572_n.jpg" alt="spa lại tất cả các dòng Xe">
					<h3>spa lại các dòng xe</h3>
					<p>Giá: 500.000 VNĐ- 1.500.000 VNĐ</p>
				</div>
				<div class="product">
					<img src="picture về sản phẩm/474572572_4157646744521050_681079070720934943_n.jpg" alt="giá hàng to">
					<h3>giá hàng cỡ lớn</h3>
					<p>Giá: 1.000.000 VNĐ</p>
				</div>
			</div>
		</div>
		<script>
			let slideIndex = 0; // Chỉ số ảnh hiện tại
			showSlides(slideIndex);
	
			function plusSlides(n) {
				showSlides(slideIndex += n);
			}
	
			function showSlides(n) {
				let slides = document.getElementsByClassName("mySlides");
	
				if (n >= slides.length) { slideIndex = 0; } // Nếu vượt quá ảnh cuối, quay lại ảnh đầu
				if (n < 0) { slideIndex = slides.length - 1; } // Nếu nhỏ hơn ảnh đầu, quay lại ảnh cuối
	
				for (let i = 0; i < slides.length; i++) {
					slides[i].style.display = "none"; // Ẩn tất cả ảnh
				}
	
				slides[slideIndex].style.display = "block"; // Hiển thị ảnh hiện tại
			}
		</script>
	</body>
</html>
