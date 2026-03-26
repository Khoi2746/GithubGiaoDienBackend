    <template>
        <div class="container mt-5">
            <h1 class="text-center">Kiến thức sức khỏe cộng đồng</h1>
            <div class="row">
                <div class="col-sm-4">
                    <div class="card">
                        <img :src="item[0].image" alt="Hình ảnh"/>
                        <div class="card-body">
                            <h3 class="card-title">{{  item[0].title }} </h3>
                            <p class="card-text"> {{ item[0].content }}</p>
                            <button class="btn btn-info">Xem chi tiết</button>
                        </div>
                    </div>
                </div>
                <div class="col-sm-4">
                    <div class="card">
                        <img :src="item[1].image" alt="Hình ảnh"/>
                        <div class="card-body">
                            <h3 class="card-title">{{ item[1].title }}</h3>
                            <p class="card-text">{{ item[1].content }}</p>
                            <button class="btn btn-info">Xem chi tiết</button>
                        </div>
                    </div>
                </div>
            <div class="col-sm-4">
                    <div class="card">
                        <img :src="item[2].image" alt="Hình ảnh"/>
                        <div class="card-body">
                            <h3 class="card-title">{{ item[2].title }}</h3>
                            <p class="card-text">{{ item[2].content }}</p>
                            <button class="btn btn-info">Xem chi tiết</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </template>

    <script setup>
    import img1 from '../assets/images/img1.jpg';
    import img2 from '../assets/images/img2.jpg';
    import img3 from '../assets/images/img3.jpg';

    const item = ([
        { title: '8 loại rau củ giàu canxi', content: 'Canxi là khoảng chất cần thiết đối với cơ thể người. Có nhiều cách để bổ sung canxi, trong đó bổ sung qua đường ăn uống là cách tốt nhất. Có 8 loại rau củ giàu canxi...', image: img1 },
        { title: 'Các loại gia vị tốt cho sức khỏe', content: 'Một số loại gia vị cung cấp nhiều polyphenol chống oxy hóa cao hơn các loại gia vị quen thuộc khác. Với một lượng nhỏ các món ăn đã thêm hương thơm và vị hấp dẫn...', image: img2 },
        { title: '9 loại đậu bổ dưỡng nên dùng nhiều', content: 'Đầu làng, đậu nành, đậu phộng, đậu Hà Lan giàu chất xơ, protein cùng nhiều vitamin và khoáng chất giúp giảm lượng đường trong máu, rất tốt cho tim mạch...', image: img3 },
    ]);

    </script>

    <style>
    .card img {
    height: 200px;     
    object-fit: cover; 
    }
    </style>