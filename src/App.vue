<template>
  <div id="app">
     <div class="full">
        <div class="header">
            <div class="header__navbar">
                <div >
                    <ul class="header__navbar-list">
                        <li class="header__navbar-item header__navbar-item-qr header__navbar-item-separate">
                            Vào cửa hàng trên ứng dụng F8-shop
                            <div class="header__qr">
                                    <img src="https://deo.shopeemobile.com/shopee/shopee-pcmall-live-sg/assets/d91264e165ed6facc6178994d5afae79.png" 
                                        alt="QR code" class="qr__code">
                                
                                    <div class="header__app">
                                    <img src="https://deo.shopeemobile.com/shopee/shopee-pcmall-live-sg/assets/f4f5426ce757aea491dce94201560583.png" 
                                        alt="png" class="qr__code-app">
                                    <img src="https://deo.shopeemobile.com/shopee/shopee-pcmall-live-sg/assets/39f189e19764dab688d3850742f13718.png" 
                                        alt="ios" class="qr__code-app">
                                </div>
                            </div>
                        </li>
                        <li class="header__navbar-item ">
                            <span class="header__navaritem-ket-noi"> Kết nối</span>
                        </li>

                        <a href="" class="navbar_con-link">
                            <i class="fab navbar_icon fa-facebook"></i>
                        </a>

                        <a href="" class="navbar_con-link">
                            <i class="fab navbar_icon fa-instagram"></i>
                        </a>
                        
                    </ul>
                </div>
                <div >
                    <ul  class="header__navbar-list">
                        <li class="header__navbar-item header__navbar-item-thongbao">
                            <a href="" class="navbar_con-link navbar_con-link-thongbao">
                                <i class="far navbar_icon fa-bell"></i>
                                    Thông báo 
                            </a>
                            <div class="header__thongbao">
                                <h3 class="header__thongbao--header">Thông báo mới nhận</h3>
                                <ul class="header__thongbao-tp">
                                    <li class="header__thongbao-item">
                                        <a href="" class="header__thongbao-item_link">
                                            <img class="header__thongbao-item_link-sanpham" src="data:image/jpeg;base64,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" alt="">
                                            <div class="header__thongbao-item-link-info">
                                                <h4 class="ten__sanpham">Sữa tươi 100% Vinamilk có đường hoặc không đường</h4>
                                                <p class="chuc__nang">Sữa tươi là các loại sữa động vật chưa qua chế biến hoặc chỉ mới qua sơ chế và chưa được tiệt trùng hay khử trùng </p>
                                            </div>
                                        </a>
                                    </li>
                                    <li class="header__thongbao-item">
                                        <a href="" class="header__thongbao-item_link">
                                            <img class="header__thongbao-item_link-sanpham" src="https://product.hstatic.net/1000003969/product/den_tt03029_1_3f3d996d8d69420a80823f793b46746a_master.jpg" alt="">
                                            <div class="header__thongbao-item-link-info">
                                                <h4 class="ten__sanpham"> Giày Comfy Moon Walk</h4>
                                                <p class="chuc__nang">Đổi trả dễ dàng Đổi trả 30 ngày cho Giày và Túi; 7 ngày cho Phụ kiện nếu lỗi nhà sản xuất</p>
                                            </div>
                                        </a>
                                    </li>
                                    <li class=" header__thongbao-item_link-end">
                                        <a href="" class="header__thongbao-item_link header__thongbao-item_link-t ">Xem tất cả</a>
                                    </li>
                                </ul>
                            </div>
                               
                             
                        </li>
                        <li class="header__navbar-item">
                            <a href="" class="navbar_con-link">
                                <i class="far navbar_icon fa-question-circle"> Trợ giúp</i>
                            </a>
                        </li>
                        <li class="header__navbar-item header__navbar-item-separate header__navbar-item-bold">Đăng kí</li>
                        <li class="header__navbar-item header__navbar-item-bold">Đăng nhập</li>
                    </ul>
                </div>
                
            </div>
            <div class="header__search">
                <div class="header__search-logo">
                    <img src="http://vietnam.lgcare.com/brand/ohui/resources/images/common/h1_logo.png" 
                    alt="" class="search__logo">
                </div>
                <div class="header__search-search">
                    <div class="search__search-wrap">
                        <input type="text" class="search__search" placeholder="Nhập tên mặt hàng">
                        <div class="search__search-history">
                            <p class="search__search-header">Lịch sử tìm kiếm</p>
                            <ul class="search__search-history2" >
                                <li class="search__search-list-li">
                                    <a class="search__search-list-item" href="" >Kem dưỡng da</a>
                                </li>
                                <li class="search__search-list-li">
                                     <a class="search__search-list-item" href="" >Sửa rửa mặt</a>
                                </li>
                            </ul>
                        </div>
                            
                    </div>
                    <div class="search__kick">
                        <span class="search__luachon">Trong shop</span>
                        <i class="fas fa-chevron-down"></i>
                        <div class="search__daluachon">
                        <span class="search__daluachon-text">Trong shop</span>
                        <i class="fas search__daluachon-dow fa-check"></i>
                        </div>  
                    </div>
                    <div class="header__search-btn">
                        <button class="header__search-btn-btn">
                            <i class="fas fa-search"></i>
                        </button>
                    </div>
                        
                    
                </div>
                <div class="header__search-cart">
                    <a href="show.html">
                        <i class="fas header__search-car--icon fa-cart-plus" style="color: white;">
                            <p id="number__incart">{{quantity}}</p>
                        </i>
                    </a>
                </div>
            </div>
        </div>
        <div class="container">
            <div class="grid">
                <div class="grid__row">
                    <div class="grid__column-2">
                        <h3 class="category__header">
                            <i class="fas fa-list" style="padding-right: 10px;"></i>
                            Danh mục
                        </h3>
                        <ul class="category__list">
                            <li class="category__list-item category__list-item-header">Sản phẩm</li>
                            <li class="category__list-item">
                                <a href="" class="category__list-item-link"> Quần âu</a>
                            </li>
                            <li class="category__list-item">
                                <a href="" class="category__list-item-link"> Quần bò</a>
                            </li>
                            <li class="category__list-item">
                                <a href="" class="category__list-item-link">Giày nam</a>
                            </li>
                        </ul>
                    </div>
                    <div class="grid__column-10">
                        <div class="home__fillter">
                            <div class="home__fillter-left">
                                <label for="" class="home__fillter-lable">Sắp xếp theo</label>
                                <button class="home__fillter-btn home__fillter-btn-1">Phổ biến</button>
                                <button class="home__fillter-btn">Mới nhất</button>
                                <button class="home__fillter-btn">Bán chạy</button>
                                
                                <div class="home__fillter-select-price">
                                    <span class="home__fillter-select-label">Giá</span>
                                    <i class="fas home__fillter-select-icon fa-chevron-down"></i>
                                
                                    <div class="home__fillter-select-price-selec">
                                        <a href="" class="home__fillter-select-price-selec1">Giá: Từ thấp đến cao</a>
                                        <a href="" class="home__fillter-select-price-selec1">Giá: Từ cao đến thấp</a>
                                    </div>
                             </div>
                                    
                            </div>
                            <div class="home__fillter-right">
                                <div class="home__fillter-right-number">
                                    <p class="home__fillter-right-number1">1</p>/10
                                </div>
                                
                                <div class="home__fillter-right-icon">
                                    <i class="fas home__fillter-right-icon-list fa-angle-left" 
                                        style=" font-weight: 300;"></i>
                                    <i class="fas home__fillter-right-icon-list home__fillter-right-icon-list-right fa-angle-right"  
                                        style=" font-weight: 300;"></i>
                                </div>
                            </div>
                            
                            
                        </div>
                        <div class="grid__column-10-2">
                          <a class="home__product" v-for="(item, index ) in listItems" :key="index"  >
                            <div class="home__product-img home__product-img--shose" 
                                :style="{backgroundImage: `url(${listItems[index].img})`}">
                            </div> 
                            <h4 class=" home_product-name home_product-name--shose">{{listItems[index].name}}</h4>
                            <div class="home__product-price">
                                <p class="home__product-price-old">
                                    {{listItems[index].price.toLocaleString('us-US', { style: 'currency', currency: 'VND' })}}
                                </p>
                                <p class="home__product-price-new home__product-price--shose">
                                    {{(listItems[index].price / 10 * 7).toLocaleString('us-US', { style: 'currency', currency: 'VND' })}}
                                </p>
                            </div>
                            <div class="home__product-icon">
                                <div class="home__product-icon-like ">
                                    <i class="far home__product-icon-like-no fa-heart"></i>
                                    <i class="fas home__product-icon-like-like fa-heart"></i>
                                </div>
                                
                                <div class="home__product-icon-star">
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="far home__product-icon-star-item1 fa-star"></i>
                                    
                                    <span class="home__product-icon-solded">Đã bán 20 </span>
                                </div>
                                
                            </div>
                            <div class="home__produce-adress">
                                <i class="fas fa-cart-plus" @click="quantity++"></i>
                                <p>Hà nội</p>
                            </div>
                            <div class="home__produce-favorite">
                                <i class="fas home__produce-favorite-check fa-check" style="font-weight: 400;"></i>
                                Yêu thích
                            </div>
                            <div class="home__product-sale">
                                <p class="home__product-sale-ratio">30%</p>
                                GIẢM
                            </div>
                        </a>
                        <!-- <a class="home__product">
                            <div class="home__product-img" style="background-image: url(data:image/jpeg;base64,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)">
    
                            </div> 
                            <h4 class="home_product-name">Áo thun nam</h4>
                            <div class="home__product-price">
                                <p class="home__product-price-old">500000đ</p>
                                <p class="home__product-price-new">399000đ</p>
                            </div>
                            <div class="home__product-icon">
                                <div class="home__product-icon-like ">
                                    <i class="far home__product-icon-like-no fa-heart"></i>
                                    <i class="fas home__product-icon-like-like fa-heart"></i>
                                </div>
                                
                                <div class="home__product-icon-star">
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="far home__product-icon-star-item1 fa-star"></i>
                                    
                                    <span class="home__product-icon-solded">Đã bán 20 </span>
                                </div>
                                
                            </div>
                            <div class="home__produce-adress">
                                <i class="fas hihi fa-cart-plus" onclick="addCartTshirt()"></i>
                                <p>Hà nội</p>
                            </div>
                            <div class="home__produce-favorite">
                                <i class="fas home__produce-favorite-check fa-check" style="font-weight: 400;"></i>
                                Yêu thích
                            </div>
                            <div class="home__product-sale">
                                <p class="home__product-sale-ratio">30%</p>
                                GIẢM
                            </div>
                        </a>
                        <a class="home__product">
                            <div class="home__product-img" style="background-image: url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRUN5Qh8qRXAdptglK57Gq2Ul3VigPNp56aOw&usqp=CAU)">
    
                            </div> 
                            <h4 class="home_product-name">Áo sơ mi trắng</h4>
                            <div class="home__product-price">
                                <p class="home__product-price-old">1500000đ</p>
                                <p class="home__product-price-new">888000đ</p>
                            </div>
                            <div class="home__product-icon">
                                <div class="home__product-icon-like ">
                                    <i class="far home__product-icon-like-no fa-heart"></i>
                                    <i class="fas home__product-icon-like-like fa-heart"></i>
                                </div>
                                
                                <div class="home__product-icon-star">
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="far home__product-icon-star-item1 fa-star"></i>
                                    
                                    <span class="home__product-icon-solded">Đã bán 20 </span>
                                </div>
                                
                            </div>
                            <div class="home__produce-adress">
                                <i class="fas fa-cart-plus" onclick="addCartShirt()"></i>
                                <p>Hà nội</p>
                            </div>
                            <div class="home__produce-favorite">
                                <i class="fas home__produce-favorite-check fa-check" style="font-weight: 400;"></i>
                                Yêu thích
                            </div>
                            <div class="home__product-sale">
                                <p class="home__product-sale-ratio">30%</p>
                                GIẢM
                            </div>
                        </a>
                        <a class="home__product">
                            <div class="home__product-img" style="background-image: url(data:image/jpeg;base64,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)">
    
                            </div> 
                            <h4 class="home_product-name">Giày đạp gót sục NY</h4>
                            <div class="home__product-price">
                                <p class="home__product-price-old">1200000đ</p>
                                <p class="home__product-price-new">999000đ</p>
                            </div>
                            <div class="home__product-icon">
                                <div class="home__product-icon-like ">
                                    <i class="far home__product-icon-like-no fa-heart"></i>
                                    <i class="fas home__product-icon-like-like fa-heart"></i>
                                </div>
                                
                                <div class="home__product-icon-star">
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="far home__product-icon-star-item1 fa-star"></i>
                                    
                                    <span class="home__product-icon-solded">Đã bán 20 </span>
                                </div>
                                
                            </div>
                            <div class="home__produce-adress">
                                <i class="fas fa-cart-plus"></i>
                                <p>Hà nội</p>
                            </div>
                            <div class="home__produce-favorite">
                                <i class="fas home__produce-favorite-check fa-check" style="font-weight: 400;"></i>
                                Yêu thích
                            </div>
                            <div class="home__product-sale">
                                <p class="home__product-sale-ratio">30%</p>
                                GIẢM
                            </div>
                        </a>
                        <a class="home__product">
                            <div class="home__product-img" style="background-image: url(data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAoHCBISERERERESEREREQ8RERESERERERIRGBQZGRgUGBgcIS4lHB4rIRgYJjgmLC8xNTc1GiQ7QDs2Py40NTEBDAwMEA8PGBISGjEhISE0MTE0NDQ0NDQ0NDQxNDQxNDE0MTQ0NDQ0NDQ0NDQxMTQ0NDE0NDQxNDQ0MTQ0MTQ0NP/AABEIAOEA4QMBIgACEQEDEQH/xAAcAAACAgMBAQAAAAAAAAAAAAAAAQIFAwQGBwj/xABAEAACAgEDAQQGBwUHBAMAAAABAgADEQQSIQUGMUFRExQiYXGRMkJSgaGx0Qdik8HwFSNTcpLC4TOCorIkVIP/xAAXAQEBAQEAAAAAAAAAAAAAAAAAAQID/8QAHREBAQEAAwEBAQEAAAAAAAAAAAERAhIhMVFBYf/aAAwDAQACEQMRAD8AuRMgmNZkEiHCEIUSSyMYhEoQhCiRjzIwJZgYoQh5hmKPMB5jEUYgSjEUcAjEUIEgYEyMcAhFCFEWYExQAxZiYxZgShI5igYVk5BZMTIccQjmgRiKMQCEUIBCEIBCEIBCEIRICPMiJKBIRyMBAlCKEB5hFFmBLMUUWYVKRzAmLMAYyJMZMjCiEMQg1jWTEiscyiUciI5pDjEUJkEIQgEIQmgQhCAQhAQGJKRhAlHFCA4ZihAMwzCLMAzDMjCA4oQhRFHImA4SMICEcQjmQ4ZikkQsQqgkk4AHeTNIBHLZOguU5cB8EhcZU+7d5yqK4JBGCCQR5HymVKEIQgijMU0CKZtJpjY+0cDvY+Q/WdB/ZNTIEC4b7YPtfE+cmrjmoxNzW9Lsrycb0+0ufxHhNMgjg8Ed4PBlQRwEBAlCIRwHImORMB5kYQgEIRQHFCKAZhFFCnCKEAEcITKAy66HpsA2HvPCe4eJlRp6jY6oPrH5DxM6mtQoCjgAAD4CLWuMZtx4PkR+krerVh1Zse2nIbxK+IMtQmQfcM/KamoTLMPtDHzGJm3GnMRx4xwfDiOdHNEyBkzLLoukDsXYZVDhR5v/AMQNzo+kNaFmGGfBC/ZGOMy0rfbnHJ8SfD4zDdaEVnOOATycDj3+AnjnWu0Fvr1Nuk1bf3prDvX9DLWsCrIRyVXaPPAHMzPb43fI9qe7GDnd5+E19RVTd9JRk8BuA33Gc3X16+lmTV0ekqGP/lUAEFT9unJZT8Aw98vtC9T4srctkcAkH/k/ONTFXq+jWVgsuHUd236WPPbK3M6xtbtYqw4HPvx5++Q1HTa7gWKlHPO8H5ZEusuXzHmbOo6ZdWTlCwH1k9oEeeByJp5lEjFDMWYDhFmEAhCIwCIxxGAoQhCiEIQhwhJVoWZVHexAmYqy6VpWx6XzyF+Hn8/yltW+e8YxMiKFUKOAoAHwExuZi1uRsVXYMldWGwR4dxHJA8iPL3zQLSaagiTtPlXFT1HQujkqpZGOQR7WD4g47pp7T5H5GdSus8+ZL1weQ+U3OTOOZr0lj/RrY+/GB8zxOh6dpWrrCvgHLHjnvMm2t8phfUk+cXlCcVN2l7RU6e+jTOSDeGIfAKqQQAHOfHJx8DPLO0dtbdUpqqVVRH0larWqoq5KvwBx9bwnQdtusaVrhTqKzqNzAKiKrOveuVOQRkgjgzmdVRoxX6zpUeqyi+sGtndLAd/tAqxODgMOMdx8prj+59StvWdQubWdRf1u1Bp0dkFbgB2AAVWVsgquMHjn3ZlbZ2p1Jeu2pjRatYSw17WS0hiQxrPA78fp3TW6N0t9frWB4V3e65gPoIWyQD5nIUfPwkesaMVXaha63SpLPRjLknxIyT35CmayfKzr17sz2nts01V2qrUhwxDorMoAYgMVOSpOPf8AGdQmsFi7qnD9/wBEgn3zzTsni7pppp1NiWc7nIDPQ5xhVAAwhxkc+J5GMTQ6TbYnWnrFzLu3hyvsq7rVwzKSQTle/v475nL6uvZNPYx5PHhyCM/cZX9T6SthL1FVf6w7lY/yM5jRdv6N7137wtbqjXit/RZJwGLfUBION3znV6RlfDV2hkPPH0iO/v8A5iNMc3dprK/p1so8ypx85izOzfUKTsZAVIwcjIx75X29CrfmslCeQD7S/I8j5ypjnRHNvWdOsq5dcr9pTlf+PvmoIBCOKAjIycRECMI8QxAUI4QHibnS1zYD9lSf5fzmmJudOsVGdnO1VQknnuBBMxfla4/VzqNVXXW1lrrXWgJZ2IAA+JnLa3t/pK1qdBlLt2x3VyWAON2wDIBOMZAnO9r9TrOo1ldPSr6SwUvQfSBLMY3lnVsAk5GBnjB85ztmor0t/T7GQsKdIwsUKm/eC6HvODhgec+JknHWrXZ9U7fNVXXYldNtbl1yu4e0FJAyp4yRjkcTH0X9oo1AtL6N0FNbWOyWq42jwAYLyecDPgZ5W1rgbSzqpy4VtxX2gPbAPnxz48TuexZo9TuB9llFj2sVYKa/aAO48HgMOPKavGSJOV12HT+3fTriqi/0bsQAttbpyT3bsFc/fOiW9D3Mpz5Mp58u+eAdWop9LTXp2ZqSlaIzAhjudsk8DnJPh906E62yqm/T61W2il1qtCOyOCh25KgjOfE4meXH8Wcv17H9x+Upe0XVXrpcacI+oZSK1LDCsRwzHkDHBA8T5DmeS9Fez1HqIrcgr6J+SwITJDAc8HHukqup3aSvS3C1tQtyWF67H3KpDbdqnkg4yOc+Pul6J2Y+qa1kt0FqkOyUI7ByrMTubdnvwTzz7xKjX1WbvTPWyLe1liEjhgWOcHxGfyi0qLZbWh3LXZZWhx3KrOAcc8cGeg9qOhi5KXBVU09VuU5GVVWKKuMY5A+6dNyyM/VP+ztrBfeFrdkasB3LhdmCxXKnO/J493JmftrqndGV9K9ATUv/AHhAVb/7tlDA4G7gLzyMDv4lH2euvqa7U0AOtGDdWfrVnOSDg4xjP4y17X9f0+roo9C3tAuzVke0h2AYbHGe/nuj+p/F10zoZSvSarR2rTc+nr9Ij7nquJQd6hgV+j3jy+OcWn6bqtPrRrtT6J0LkOtLuSDYfRr7LheAzDPPcPGVXaPadN0pXcqjVIHCgHGFTLqcd43H+jK/rGsFVmq01DJZpXKja7tYoxghlbdnOQPHwiQZjq3J12krRbfWdXmso+SHW0kbcAhlYDzGO+a9HUNVo7X2PZU9bbHVXWxCy4UhkPDfRxnOe4Aze7BKG14Lr7XobTX9EhXJC5B552lhx5y17b9Mqr9Ncrg3PZQzV8Zrr2OCeORuZc84+jxNeW5U/wBdxo+0Nnq9F12mssWzYDtrDWJuzhigZvYOO8En2hkDwudB1/S6nctdyF1+khO105x7SnleQRyB3Tzzsv1DV0UadnVtTpLBhGqR7btMwJBV1UElODgjyHnNTpZA6ncGFldOqW+tXsrNZBc70I3r7JzwMic+v1rXsGm3fWIKgcEHOZg1WlpsJDptb6rrw3wPnPI9F2iv0ulatbrRq6tQU/vFttS1DldoyMrhgOMg/HuHonZrq76zTpYwzch9HfWQUZLAOQM4IByCM+B88iLvH6s9a2s0jVuVPK5O1scMJrzrHsUrsetguMYKkj5/zmkekUufYd1PfjvwPvETlDHPmEubOgt9SxT7mBX8szSu6banfWSPNfa/LmaTGnCPEIRHEJLEIEZJqDYltYUvvqsTA4zkYkZc9J0Lgek+juGFXzHmZjlPGp9eRauy/Sf3rNbXZWenolT7669nq/tgpnDe0ME+BHhKPp6etaupH4WywlhuZxsyWKDxA4x98+iHdgMOuR71DCaFmh0bsHfS6ZnHIc01q4PmGxkSTlItjybtj0tzZZqQFFa1Vrjge0HVAuPLBz901eyfWDTWK9QMaS1nWuxgNi2fWVj4A+/8u71zWdntDeGFlBYMoVlXU6lVIDBh7KuBnIHOMzAnYzpwqNAosFTNuKeldwT8WJx92JZymZTPXkXayhK9XTsVETZQdqKqqBvPOB98v7ev3Jqn0tenFmxNxJc1EgKCXyQRt8OBOo1v7MunuQyPqqiuMAOlijHcMMp490jq+wivqDqV1NiuU2EBE2Fdu3BA/riW2GVw3Vuv1ugeoKDqNPZVam4b1YlCrMMANjDYJ8z3eNd2e6J60l9jk7KK32KpClrSuVX3Djn4iddb+ys4wmqP/fUG/Jh5CWfQOyF+jSyvelgd9+4IUI9kDuJPkI2SeGXfXkyLg1s4fYzKxAOCUD8lOe/hh4cz0vV6avU112V32IK6WKMjg7l2lSj5yD7QwcjOeJp9f7Ia2yyuyvTVbURUNVT+AsLErlVB4M2m7M6vTtc2kBSq1W3UW12Om443FWXkH54/JbuVJK5zsTq/RDW2nG1K0cggfabA5HjxLjT9pNLcFF2mbbY/ow1tavTv4O0HJ8B9nxErND0yzRjVJqFVBfp7Qh52ttRiVO7GOCMcShXUvfp6NKlW81vaylcEkMGJDceGSc5lyWp8Z+0GqyzUqiqlV+oKbCAhDEcKoHsgBQJaa/oPo+nUuKw172I1hx7Y3rhVHPdkquPMzk2AxnG3gnI5GMCer2a/Vppa3q0wN2QGqNm/CYI3BhgEkBTjPifKW3MHCdF1Vej1itaiutZZHO3fsION6gjvBH4ztO1Wl076S3V1Kju5qzaDuLKXVeDjHcRyMZ985ns/WG6qyOvDvq1ZTgj6xIPge78J0R7PaMCytNVqEViC9VWpr9FvzyNhUjPC9/dgeUW5YmeNTpXX7NL0euytQzpqLKyXDMiqTvwwUg+OBLHrfaayuuzT6tEqtsprtpspax1V8hkDBl8CAT4cEcyl6wtWl02q0Nbs4YafUILCjWF2dldRgAEAID3fWEqNNpdRrK7bnsLJpKQo3ICTtBIrGMdy8knPgPhZlK2+yti29Sraxy26x7i3B32qrOCRjPfzPTekaP0Gtvu9IoTVLWTXzkWBmy3Pnu4/zHyE8T0d4rsqdmcIrgk1+xZsyQ21hyCRunqWsoqvVNdUS9lNdr1PW7hGKjcAwUHI3KOPnJyI9L9NIG3H9f1zNHTakWVpYpyrojqfNSAQfxkms/oTGtt82Rb5orbxA3y6F1LQpYpZQBYBkEfW9x/Wc3idRUHf6IOPPuHzlDr9L6NyudwPtA+4+EsqVrYik4Sso6Vdz1qeQWXI92eZ1q3jxE5fpK5uX3Bj+GP5zoGE58q3xjZ9Kp8YFVPkflNUiRxJq42X0qH6omI6NfDI++QDHzPzjFjecbAxpf3m+ci2nYdzN85MXt/QkhqG93yjwa4Lr4n7+ZIWn3fITP6x5qIekXxQSYaxCz3D8pJbfiPvjIrP1SPgZA1L4MR8RAym44wSSPIgETTfQaZm3tptMz4I3mmsPg943Yz4CZ/RHwYflGNMx8V+cvo5+/sP0t+/Rqh5/wClddX+Cvj8JtafsxpK0WtDeqLnaDYtmB9nLLnHuzLc6RvdI+qv54+8y7UyORq/Z7RXqzq01doYvY5R6kZfbDAqCCOPa/CV4/ZgmNQW1dd1loIrZ6WHoyWyWPtnJ98771az7X84jRZ5g/ES9qmR5prf2c9QsCB9fpbNi7ELixWC5zjIQk/Eky77OdjNRpdO1LvpX3M7Nssch9wA53J5AD7p2HobP3fxkBp7T3Mg58VaLyv4TjHm3Wv2caovT6qtJrqRVK2XjJYOWP1eQcyxXsBqarLG0eoXS12Ltal9t6DuycFvcMZyRzzg4ndDT2faTHwbMl6tZ9pP9LfrHblf4vWK/s70i3TaWnT22I7Ups3q2AyDOzjwwMD7pZHS+boPhkyJ0tngy/6TGNE573I+CjiT38ULVWPpOW8to/WMXVr9CvJ9+XPymROnj67Fv8xwPwmUGtO7HwUS4jGGsfv9kf14TF1DSp6J93LKpZW+tnEzNqj9UYmnr7MVuWPeCo+J4lgoYSOY5plcaHpLUuXLqw2lcLnPJHP4TdMnqqHdcK22VLnWVd9a6hPNG22Y/I/Kcq3xnixIimvXrCRl6NRX7mqZvxTMG19Q+k6ofJzsPybEyrYhMS6qs91lZ+Dof5zKGB7iD8CJQ8QAgMef5QyPP8v1hBiPEjuHmPwj3jzHzEB4jiz/AFxHiUERjx/XMJCEHI8TJC5h4mKECY1Te75R+tN5CYiIsS7TGf1s/ZEfrn7o+c18RYEbRseufuiHrp+yJr4hiNoznWN7vlMbalz4yIWa2q1tNX/UtrT3O6qT8B3mNGxuJ7yYwko7+1FC8VrZafMKUT5tz+E1H6vqLeFGxT9WsHP3t3/LEmmOmexVO3Kl/BdwB+/ymjqdBqLTkhMD6Khxgf8AMrtJoLTztYe88ToNHS6AAmb41LFX/Y932V/1rCdBkwmtZxEGMGKEy2mGj3TGIQJFVPeAfiAZjOmqPfXWfiifpJQhNQOkqPfVWfjWn6Reo0f4FX8Ov9JkJhGQ1j9Ro/wKf4SfpD1Kj/Ap/hV/pMsUZE1j9R0//wBen+FX+kj/AGdp/wDArHwrUflM0eYyGsH9n1eCuv8AlttUfINA6Cvwe1f/ANXb/wBszPmGY6xdap6f5X3D+EfzSI6Gzwvb/urRvyxNvMlmOsNaPql3+NWfjQw/3wOlv8HqPxrsH+8zd3QDR1hrR9Wv+3T/AKH/AFkX0up8LKB8a7D/AL5Y7pHMdYar00OpP0tRWP8AJQ2f/JzCzpdhGPW7VPmldC/mhliHgWjqaoH7KpYc26vWWfunUMiH4qmBNzSdnNHUMJp6/eWG9ifMkyyzHujIawjQVDgVVjHd7C/pMiIq9ygfAARkxZlxWTEUhmG+VEt0IswgKHEWYTKnCKPMAhFHCDMIQgwQzCEJghCEGCEIQYMwiMMwYcIZhmaMGYRZjgwGIGERhUooAwMB5hIwzAlERDMcCOD5xxwhEY4oTLQhCEBwhCEEIQEAhCBgOEQjMBQizGTAUIQmgRxQMBwihAcIo4ETGDHIQJxQBkjAjCPEJNCzCPMI0KRjMUgYkooQAwEjJTQIQIkYExEDASMCRhmRhAkIjHIwmCMQEUGJQxEBJSaDEMQhGrhYjxCGY0AgRDMJBEiPMcREuhwxEI5AsQjhCIRiKECUjCEAhCEqiEISoIzFCAQhCAxFCEAkoQkBHCEhBCEIUQhCEKOEIUjHCEIRjEIQohCEI//Z)">
    
                            </div> 
                            <h4 class="home_product-name">Giày đạp gót sục NY</h4>
                            <div class="home__product-price">
                                <p class="home__product-price-old">1200000đ</p>
                                <p class="home__product-price-new">999000đ</p>
                            </div>
                            <div class="home__product-icon">
                                <div class="home__product-icon-like ">
                                    <i class="far home__product-icon-like-no fa-heart"></i>
                                    <i class="fas home__product-icon-like-like fa-heart"></i>
                                </div>
                                
                                <div class="home__product-icon-star">
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="fas home__product-icon-star-item fa-star"></i>
                                    <i class="far home__product-icon-star-item1 fa-star"></i>
                                    
                                    <span class="home__product-icon-solded">Đã bán 20 </span>
                                </div>
                                
                            </div>
                            <div class="home__produce-adress">
                                <i class="fas fa-cart-plus"></i>
                                <p>Hà nội</p>
                            </div>
                            <div class="home__produce-favorite">
                                <i class="fas home__produce-favorite-check fa-check" style="font-weight: 400;"></i>
                                Yêu thích
                            </div>
                            <div class="home__product-sale">
                                <p class="home__product-sale-ratio">30%</p>
                                GIẢM
                            </div>
                        </a> -->
                        
                    </div>
                </div>
                </div>
                
            </div>
        </div>
        <div class="footer">
            
        </div>
    </div>
  </div>
</template>

<script>
import axios from 'axios'
export default {
  name: 'app',
  data () {
     
    return {
        listItems : [],
        quantity : 0
    }
  },
  computed: {
    
  },

  created() {
     axios
    .get('https://60c81d59afc88600179f62c1.mockapi.io/items')
    .then((response) => {
      console.log(response);
      this.listItems = response.data;
  })
  }
  
}
</script>

<style>

</style>
