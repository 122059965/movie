<template>
    <div>
        <h1>豆瓣电影排行榜</h1>
        <h2>豆瓣新片榜· · · · · ·</h2>
        <div style="border-top:1px dashed #cccccc;height: 1px;overflow:hidden"></div>


        <div id="app">
            <div v-for="movie in mlvieList">
                <img v-bind:src="movie.src"/>
                <h1>{{movie.title}}</h1>
                <p>{{movie.text}}</p>
                <h4>{{movie.score}}</h4>
                <span></span>
            </div>
        </div>
    </div>


</template>

<script>
    var app = new Vue({
        el: "app",
        data: {
            movieList: [
                {
                    src: "../assets/6.jpg",
                    title: "爱尔兰人 / 爱尔兰杀手(港) / 听说你刷房子了",
                    text: "2019-09-27(纽约电影节) / 2019-11-01(美国点映) / 2019-11-27(美国网络) / 罗伯特·德尼罗 / 阿尔·帕西诺 / 乔·佩西 / 安娜·帕奎因 / 杰西·普莱蒙 / 哈威·凯特尔 / 斯蒂芬·格拉汉姆 / 鲍比·坎纳瓦尔 / 杰克·休斯顿 / 阿莱卡萨·帕拉迪诺 / 凯瑟琳·纳杜奇...",
                    scoring: {
                        score: 9.1,
                        amount: 46180,
                        star: 4.5
                    }
                },
                {
                    src: "../assets/1.jpg",
                    title: "小丑 / 小丑起源电影：罗密欧 / Romeo",
                    text: "2019-08-31(威尼斯电影节) / 2019-10-04(美国) / 杰昆·菲尼克斯 / 罗伯特·德尼罗 / 马克·马龙 / 莎姬·贝兹 / 谢伊·惠格姆 / 弗兰西丝·康罗伊 / 布莱恩·考伦 / 布莱恩·泰里·亨利 / 布莱特·卡伦 / 道格拉斯·霍奇斯 / 格伦·弗莱施勒 / 比尔·坎普...",
                    scoring: {
                        score: 8.8,
                        amount: 378978,
                        star: 4.5
                    }
                },
                {
                    src: "../assets/2.jpg",
                    title: "好莱坞往事 / 从前，有个荷里活(港) / 从前，有个好莱坞...(台)",
                    text: " 2019-05-21(戛纳电影节) / 2019-07-26(美国) / 2019(中国大陆) / 莱昂纳多·迪卡普里奥 / 布拉德·皮特 / 玛格特·罗比 / 埃米尔·赫斯基 / 玛格丽特·库里 / 蒂莫西·奥利芬特 / 茱莉亚·巴特斯 / 奥斯汀·巴特勒 / 达科塔·范宁 / 布鲁斯·邓恩 /...",
                    scoring: {
                        score: 7.3,
                        amount: 73598,
                        star: 3.5
                    }
                },
            ]
        }
    })
</script>


<style scoped>
    h1 {
        margin-top: 50px;
        word-wrap: break-word;
        display: block;
        font-size: 30px;
        font-weight: bold;
        color: #494949;
        padding: 0 0 15px 0;
        line-height: 1.1;
        text-align: left;
    }

    h2 {
        font-size: 20px;
        color: #072;
        margin: 0 0 12px 0;
        line-height: 150%;
        text-align: left;
    }
</style>