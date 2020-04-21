<!--
 * @Description: 
 * @Date: 2020-04-21 10:31:49
 * @LastEditors: Astronautics across the sea of stars
 * @LastEditTime: 2020-04-21 15:25:23
 -->
# vue-parallax-image

一个根据鼠标移动，图层视差效果vue组件
未做测试，请谨慎使用！

 ## demo演示
 [demo](http://www.jq22.com/yanshi4800)


 ## 安装
 
 ```JS
 npm install vue-parallax-image --save
 ```
 
 ## 使用
 
 ```js
    <ParallaxImage :config='config' />

    import ParallaxImage from 'vue-parallax-image'
    
    components: { ParallaxImage },

    data () {
           return {
               config:{
                    width:'100%', // 底图的宽度
                    height: '500px', // 底图的高度
                    basemap: require('../../assets/img/0.jpg'), // 底图相对路径
                    imgList:[ // 视差图片的列表 （建议最少1张最多5张）
                        {
                            img: require('../../assets/img/1.png'), // 图片路径
                            width:  '200px', // 图片的宽度
                            height: '200px', // 图片的高度
                            left:   '60%', // 图片的位置 - left
                            top:    '25%'  // 图片的位置 - top
                        },
                        {
                            img: require('../../assets/img/2.png'),
                            width:  '200px',
                            height: '100px',
                            left:'40%',
                            top: '45%'
                        },
                        {
                            img: require('../../assets/img/3.png'),
                            width:  '100%',
                            height: '100%',
                            left:'0%',
                            top: '0%'
                        },
                        {
                            img: require('../../assets/img/4.png'),
                            width:  '',
                            height: '',
                            left:'5%',
                            top: '0%'
                        }
                    ]
                }
           }
       }

       

 ```

