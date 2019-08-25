<template>
  <div class="home">
     <header id="s">
        <el-menu  class="el-menu-demo" mode="horizontal"  background-color='#F5F5F5' text-color='	#696969'>
        <el-submenu index="1">
            <template slot="title">中国大陆</template>
            <el-menu-item index="2-1">选项1</el-menu-item>
            <el-menu-item index="2-2">选项2</el-menu-item>
            <el-menu-item index="2-3">选项3</el-menu-item>
            <el-menu-item index="2-1">选项1</el-menu-item>
            <el-menu-item index="2-2">选项2</el-menu-item>
            <el-menu-item index="2-3">选项3</el-menu-item>
         </el-submenu>
         <el-menu-item index="2" style="color:red">请登录</el-menu-item>
         <el-menu-item index="3">免费注册</el-menu-item>
         <el-menu-item index="4">手机逛淘宝</el-menu-item>

            <el-submenu index="5" style="margin-left:320px">
                <template slot="title" >我的淘宝</template>
                <el-menu-item index="5-1">已买到的宝贝</el-menu-item>
                <el-menu-item index="5-2">我的足迹</el-menu-item>
           </el-submenu>
           <el-menu-item index="6">购物车</el-menu-item>
            <el-submenu index="7" >
                <template slot="title" >收藏夹</template>
                <el-menu-item index="7-1">收藏的宝贝</el-menu-item>
                <el-menu-item index="7-2">收藏的店铺</el-menu-item>
           </el-submenu>
            <el-menu-item index="8">商品分类</el-menu-item>
            <el-submenu index="9" >
                <template slot="title" >千牛卖家中心</template>
                <el-menu-item index="7-1">收藏的宝贝</el-menu-item>
                <el-menu-item index="7-2">收藏的店铺</el-menu-item>
                <el-menu-item index="7-1">收藏的宝贝</el-menu-item>
                <el-menu-item index="7-2">收藏的店铺</el-menu-item>
                <el-menu-item index="7-1">收藏的宝贝</el-menu-item>
                <el-menu-item index="7-2">收藏的店铺</el-menu-item>
           </el-submenu>
             <el-submenu index="10" >
                <template slot="title" >联系客服</template>
                <el-menu-item index="7-1">消费者客服</el-menu-item>
                <el-menu-item index="7-2">卖家客服</el-menu-item>
           </el-submenu>
            <el-menu-item index="11" @click="dh=!dh">网站导航</el-menu-item>
            
          </el-menu>
          <div style="width:1500px;height:352px;;background:white;position: absolute;z-index: 99" v-if="dh">
                   <p>dsbhbnthnbdf</p>
                   <p>dbndfbndffgrfg</p>
            </div>
          <div style="display: flex;">
          <img src="//img.alicdn.com/tfs/TB1_uT8a5ERMeJjSspiXXbZLFXa-143-59.png" alt="" style="margin:40px 140px;display: flex">
          <div style="display: flex;height:50px;margin:auto -60px">
             <input type="text" placeholder="请输入要搜索的物品" style="width:600px;border-radius: 25px 0px 0px 25px; border: 2px orange solid;border-right:none;outline:none">
             <input type="button" value="搜索" style="color:white;background:#FF4200;width:80px;border-radius: 0px 25px 25px 0px; border: 2px orange solid;border-left:none;">
          </div>
          
          </div>
       </header>
      <div class="count">
              <div style="margin:0px auto;display: flex; justify-content: center">
                <el-menu  class="el-menu-demo" mode="horizontal"  background-color='#FF5900' text-color='white' style="display: flex;"  active-text-color='none'>
                <el-menu-item index="1" style="width:200px;text-align:center;background-color:red;margin-left:-20px ;" >主体市场</el-menu-item>
                <el-menu-item index="2" >天猫</el-menu-item>
                <el-menu-item index="3">聚划算</el-menu-item>
                <el-menu-item index="4">天猫超市</el-menu-item>
                <el-menu-item index="5">淘抢购</el-menu-item>
                <el-menu-item index="6">电器城</el-menu-item>
                <el-menu-item index="7">司法拍卖</el-menu-item>
                <el-menu-item index="8">淘宝心选</el-menu-item>
                <el-menu-item index="9">兴农扶贫</el-menu-item>
                <el-menu-item index="10">飞猪旅行</el-menu-item>
                <el-menu-item index="11">智能生活</el-menu-item>
                <el-menu-item index="12">苏宁易购</el-menu-item>
                <el-menu-item index="13">玩转黑科技</el-menu-item>
              </el-menu>
              </div>
      </div>
           <div style="width:1316px;margin:2px auto;display: flex; justify-content: flex-start;">
           <ul style="width:197px;margin-top:-3px;border:1px red solid;height:543px" class="nav">
            <el-col :span='5'>
              <el-menu
                class="el-menu-vertical-demo"  style="width:195px;border-right:none">
                 <el-menu-item index="1"  class="list" @mouseenter="test" @mouseleave="isflag=false" >
                  <span slot="title" >女装/男装/内衣</span>
                </el-menu-item>
                <el-menu-item index="2" class="list" @click="isflag=!isflag" >
                  <span slot="title">鞋靴/箱包/配件</span>
                </el-menu-item>
                <el-menu-item index="3" class="list">
                  <span slot="title" @click="isflag=!isflag">鞋靴/箱包/配件</span>
                </el-menu-item>
                <el-menu-item index="4" class="list"> 
                  <span slot="title" @click="isflag=!isflag">鞋靴/箱包/配件</span>
                </el-menu-item>
                 <el-menu-item index="5" class="list"> 
                  <span slot="title" @mouseover="isshow" @mouseleave="noshow">鞋靴/箱包/配件</span>
                </el-menu-item>
                 <el-menu-item index="6" class="list">
                  <span slot="title" @mouseover="isshow" @mouseleave="noshow">鞋靴/箱包/配件</span>
                </el-menu-item>
                 <el-menu-item index="7" class="list">
                  <span slot="title" @mouseover="isshow" @mouseleave="noshow">鞋靴/箱包/配件</span>
                </el-menu-item>
                 <el-menu-item index="8" class="list">
                  <span slot="title" @mouseover="isshow" @mouseleave="noshow">鞋靴/箱包/配件</span>
                </el-menu-item>
                <el-menu-item index="8" class="list">
                  <span slot="title" @mouseover="isshow" @mouseleave="noshow">鞋靴/箱包/配件</span>
                </el-menu-item>
                <el-menu-item index="8" class="list">
                  <span slot="title" @mousemove="isshow" @mouseleave="noshow">鞋靴/箱包/配件</span>
                </el-menu-item>
                 <el-menu-item index="8" class="list">
                  <span slot="title" @mousemove="isshow" @mouseleave="noshow">鞋靴/箱包/配件</span>
                </el-menu-item>
                 <el-menu-item index="8" class="list">
                  <span slot="title" @mousemove="isshow" @mouseleave="noshow">鞋靴/箱包/配件</span>
                </el-menu-item>


              </el-menu>
           </el-col>
           </ul>
           <!-- 轮播图 -->
           <ul style="height:280px;width:580px;margin-left:10px;position: relative;">

             <!-- 蒙版 -->
             <div style="height:540px;width:770px;background:white; position: absolute;  z-index: 333;margin-left:-9px;margin-top:-2px;border:2px red solid;" v-if="isflag">
              <p>dvfbgdngdgndgndf</p>
             </div>
                <div class="block">
                     <el-carousel height="280px">
                         <el-carousel-item v-for="picture in pictures" :key="picture">
                        <img :src="picture" alt="">
                        </el-carousel-item>
                       </el-carousel>
                </div>
                

                <!-- 轮播图下方 -->
                <div  style="height:40px;background:white;width:760px; display: flex;  justify-content: space-between;">
                 <p  style="height:40px;width:450px; display: flex;line-height:50px;">理想生活上天猫</p>
                 <p  style="height:40px;width:160px; display: flex;line-height:50px">热销商品</p>
                </div>
                <div style="width:760px;height:220px;display: flex;">
                  <!-- 小轮播图 -->
                  <ul style="width:575px;">     
                       <div class="block">
                            <el-carousel height="220px" indicator-position='none'>
                            <el-carousel-item v-for="image in images" :key="image">
                            <img :src="image.tp1" alt="" style="width:282px;height:220px;">
                            <img :src="image.tp2" alt="" style="width:282px;height:220px; margin-left:10px">
                            </el-carousel-item>
                            </el-carousel>
                         </div>  
                  </ul>
                  <ul  style="height:170px;width:160px;margin-left:23px" >
                              <img :src="img" alt="" style="width:160px;height:220px">
                     </ul>
                   
                  
               </div>
           </ul>

           <!-- 轮播图旁边图片 -->
           <ul  style="height:280px;width:160px;margin-left:20px" >
             <img :src="img" alt="">
           </ul>
     
           <ul style="height:543px;width:328px;margin-left:15px;border:1px solid #D3D3D3;background:white">
              <div style="width:100%;height:173px;background:url('https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1566478701193&di=cc2eab8df266ca40425025cc7d35f727&imgtype=0&src=http%3A%2F%2Fimg3.redocn.com%2F20120309%2FRedocn_2012030901590609.jpg');background-size: cover">
                   <img src="https://gw.alicdn.com/tps/i3/TB1yeWeIFXXXXX5XFXXuAZJYXXX-210-210.png_50x50.jpg" alt="" style="border-radius: 50%;margin:5px 140px;">
                   <p style="margin:0px auto;width:48px;font-size:14px">HI!你好</p>
                    <div style=" display: flex; justify-content: space-between;margin:20px auto;width:80%;">
                         <span  class="button">登录</span> 
                         <span   class="button">注册</span> 
                         <span   class="button">开店</span>   
                    </div>
                     <p style="width:100%;height:25px;background:#ffe4dd;text-align:center;color:#f40;font-size:12px;line-height:25px; cursor: pointer;">网上有害信息举报专区 </p>     
              </div>
              <ul style="width:100%;display: flex;justify-content: space-around">
                <li  class="litter-nav"  @mouseover="a" :style="ys">公告</li>
                <li  class="litter-nav"  @mouseover="a2" :style="ys2">规则</li>
                <li  class="litter-nav"  @mouseover="a3" :style="ys3" >论坛</li>
                <li  class="litter-nav"   @mouseover="a4" :style="ys4" >安全</li>
                <li  class="litter-nav"  @mouseover="a5" :style="ys5" >公益</li>
              </ul>
              <!-- 第一个 -->
              <ul  class="cont" v-if="flag">   
               <p v-for="notice in notices" :key='notice'  class="cont-list"  >{{notice}}</p>
              </ul>
              <!-- 第二个 -->
              <ul  class="cont" v-if="flag2">
               <p  v-for="notice2 in notices2" :key='notice2'  class="cont-list" >{{notice2}}</p>
              </ul>
                <!-- 第三个 -->
              <ul  class="cont" v-if="flag3">
               <p>r33333333</p>
              </ul>
                <!-- 第四个 -->
              <ul  class="cont" v-if="flag4">
               <p>44444444444</p>
              </ul>
                <!-- 第五个 -->
              <ul  class="cont" v-if="flag5">
               <p>55555555</p>
              </ul> 
              <ul style="width:100%;height:265px; display: flex; flex-wrap:wrap;  position: relative;">
                <li class="nav-list" @mouseover="navshow" @mouseleave="no" :style="navstyle">充话费</li>
                <ul style="width:100%;height:185px;border:1px red solid;border-top:none;position: absolute;top:89px;background-color:white" v-if="ifnav">
                 <p>1111111111111</p>
                </ul>
                <li class="nav-list"   @mouseover="navshow2" @mouseleave="no" :style="navstyle2" >旅行</li>
                <ul style="width:100%;height:185px;border:1px red solid;border-top:none;position: absolute;top:89px;background-color:white" v-if="ifnav2">
                    <p>22222222222</p>
                </ul>
                <li class="nav-list"  @mouseover="navshow3" @mouseleave="no" :style="navstyle3">车险</li>
                 <ul style="width:100%;height:185px;border:1px red solid;border-top:none;position: absolute;top:89px;background-color:white" v-if="ifnav3">
                    <p>333333333</p>
                </ul>
                <li class="nav-list"  :style="navstyle4">游戏</li>
                <li class="nav-list">充话费</li>
                <li class="nav-list">充话费</li>
                <li class="nav-list">充话费</li>
                <li class="nav-list">充话费</li>
                <li class="nav-list">充话费</li>
                <li class="nav-list">充话费</li>
                <li class="nav-list">充话费</li>
                <li class="nav-list">充话费</li>
              </ul>
           </ul>
         </div>
          
          <!-- 淘宝头条 -->
          <div class="headline">
           <p  class="headline-background" >
           <span style="font-size:14px;color:#B5B5B5;">让你的生活更有趣</span>
           </p>
           <ul style="width:760px ;height:100px;margin-left:10px; background-color: white;">
              <el-carousel height="100px" direction="vertical" :autoplay="false" style="  background-color: #d3dce6;">
                  <el-carousel-item v-for="item in items" :key="item"> 
                   <div style="display: flex;flex-wrap:wrap;height:100px">
                   <img :src="item.tp" alt="" class='headline-img' >
                   <p  class='headline-p'>{{item.bt}}</p>
                   <span class='headline-span'>{{item.nr}}</span>
                    </div>
                  </el-carousel-item>
             </el-carousel>
            </ul>
            <div style="width:330px;height:100px;margin-left:15px;  background-color: #d3dce6;  ">
              <div style="  display: flex;   justify-content: space-between ;"> 
                 <!-- <h4 style=" display: flex;margin-left:10px">阿里APP</h4> -->
                  <el-button style="padding: 3px 0;display: flex;color:black;margin-left:13px" type="text">阿里APP</el-button>
                   <el-button style="padding: 3px 0;display: flex;" type="text">更多></el-button>
               </div>
               <div style="display: flex;flex-wrap: wrap;justify-content: space-around"> 
               <li style="list-style: none;display: flex;margin:3px 15px" v-for="tb in tbs" :key="tb">
               <img :src="tb"  style="width:32px;height:32px;">
               </li>
               </div>
             </div>
            </div>
         
         <div class="main">
         <ul class="main-cont" >
            <el-card class="box-card" v-for="main in mains " :key='main'>
             <div slot="header" class="clearfix">
               <p style="color:red;font-size:20px;font-weight:400px;">{{main.title}} <span style="color:black;font-size:14px;font-weight:400px">{{main.stitle}} </span></p>
               <el-button style="float: right; padding: 3px 0;" type="text">更多</el-button>
               </div>
              <div class="text item">
              <ul style="width:180px;height:240px;border:1px solid #f4f4f4;margin:10px 8px" v-for="tp in 6" :key='tp'>
                  <img :src="main.tp" style="margin:0px ;display: flex;  cursor: pointer;">
               <p style="width:100%;margin:8px 2px;font-size:14px">{{main.ms}}</p>
               <p style="color:skyblue;font-size:16px;margin:0px 10px">{{main.pj}}</p>
              </ul>
               </div>
             </el-card>
         </ul>
         <el-card  style="width:100%;margin-top:20px;">
           <div slot="header" class="clearfix">
              <p style="color:red;font-size:20px;font-weight:400px;">淘抢购<span style="color:black;font-size:14px;font-weight:400px;margin-left:10px">距结束00:00:00 </span></p>
              <div style="float: right;">
                <el-button style="padding: 3px 0" type="text" @click="change">换一换</el-button>
                <el-button style="padding: 3px 0" type="text">更多></el-button>
             </div>

           </div>
           <div style="display: flex;justify-content: space-between;" >
             <div style="width:410px;height:200px;border:1px #f4f4f4 solid;display: flex;" v-for="buy in buys" :key='buy'>
                 <ul style="width:180px ;height:180px;background:#4f4f4f;margin:10px 0px;">
                     <img :src="buy.image" alt="" style=" opacity:0.8 ;">
                   </ul>
                   <div style=" display: flex;flex-wrap: wrap;  align-content:  space-around"> 
                        <p style="word-break: break-all;width:200px;margin-left:10px;"> {{buy.ms}}</p>
                        <p style="word-break: break-all;width:200px;margin-left:10px;">{{buy.yh}}</p>
                        <span style="color:red;font-size:20px;margin-left:10px;font-weight:300px">{{buy.jg}}</span>
                     </div>
                 </div>
            </div>
         </el-card>
         <div style="width:100%;height:300px;margin-top:0px;background:#f4f4f4;">
           <p style="margin:0px 500px;padding:20px 0px;font-size:20px; opacity: 0.2">-------------- END------------------</p>
           <div style=" display: flex; justify-content: space-around;">
             <ul  class="end" v-for="end in ends" :key='end'>
               <p class="end-main" >{{end.title}}</p>
               <p style="width:260px;display: flex; flex-wrap: wrap;margin-top:10px">
                  <span  class="spans" v-for="span in end.spans" :key='span'>{{span}}</span> 
                </p>
             </ul>
           </div>
         </div>
    
        </div>
          <div style="width:100%;background:white;margin-top:-20px">
            <ul style="width:1320px;height:300px;margin:0px auto;display: flex; flex-wrap: wrap;  justify-content: space-around">
             <div style="height:60px;">
              <el-link href="https://element.eleme.io" target="_blank" v-for="lj in ljs" :key='lj' class='ljs'>{{lj}}</el-link>
            </div>
            <div style="width:100%;height:60px;border-top:1px black solid;margin-top:-123px;display: flex;flex-wrap: wrap;">
                 <div style="height:60px;width:840px;">
                 <el-link href="https://element.eleme.io" target="_blank" v-for="message in messages" :key='message' style="margin:5px 6px">{{message}}</el-link>
                </div>
                 <div style="height:60px;font-size:14px;color:#9c9c9c;">
                  <p style="margin:5px 80px">© 2003-现在 Taobao.com 版权所有</p>
                  <p style="margin:10px 0px">浙江省网络食品销售第三方平台提供者备案：浙网食A33010001</p>
                 </div>
                 <ul style="width:1316px ;height:100px;">
                  <div style="height:80px;">
                 <el-link href="https://element.eleme.io" target="_blank" v-for="message2 in messages2" :key='message2' style="margin:5px 8px;font-size:14px">{{message2}}</el-link>
                 <img src="https://img.alicdn.com/tfs/TB1EPnIQXXXXXaSXpXXXXXXXXXX-1133-35.jpg" alt="" style="height:60px;width:1316px;margin-top:10px">
                </div>
                 </ul>
                 
            </div>
            

           </ul>
           <a href="#s"> <img src="http://pic.51yuansu.com/pic3/cover/00/65/15/5895b559e9620_610.jpg" alt="" style="width:60px; position: fixed;right:10px;top:600px"></a>
         
         </div>
      
  

  
 
 
  </div>
</template>

<script>
export default {
  data(){
   

  
     return{
        flag:true,
        flag2:false,
        flag3:false,
        flag4:false,
        flag5:false,
        isflag:false,
        ifnav:false,
        ifnav2:false,
        ifnav3:false,
        dh:false,
       pictures:[
       "https://img.alicdn.com/tps/i4/TB1tktbdND1gK0jSZFySuwiOVXa.jpg",
       "https://img.alicdn.com/tfs/TB1JrZkdAL0gK0jSZFtXXXQCXXa-520-280.jpg",
       "https://img.alicdn.com/tps/i4/TB1tktbdND1gK0jSZFySuwiOVXa.jpg",
       "https://img.alicdn.com/tfs/TB1JrZkdAL0gK0jSZFtXXXQCXXa-520-280.jpg",
       ],
       img:[
         "https://img.alicdn.com/imgextra/i1/56/O1CN01sUaK5p1CHgjVPHwB0_!!56-0-lubanu.jpg_290x290q90.jpg_.webp",
       ],
       images:[
         {
           tp1:'https://img.alicdn.com/tps/i4/TB1gWzQda67gK0jSZFHSuu9jVXa.jpg_240x240q90.jpg',
           tp2:'https://aecpm.alicdn.com/simba/img/TB13xKuLVXXXXcHapXXSutbFXXX.jpg'
         },
            {
           tp1:'//img.alicdn.com/tps/i4/TB1Ar8Kblv0gK0jSZKbSuvK2FXa.jpg_240x240q90.jpg',
           tp2:'//img.alicdn.com/tps/i4/TB1Sa_HbEH1gK0jSZSySuttlpXa.jpg_240x240q90.jpg'
         },
         {
      tp1:"//img.alicdn.com/tps/i4/TB1Ar8Kblv0gK0jSZKbSuvK2FXa.jpg_240x240q90.jpg",
      tp2:"//img.alicdn.com/tps/i4/TB1G1ESaBv0gK0jSZKbSuvK2FXa.jpg_240x240q90.jpg",
         }
        
       ],
       items:[
         {
           tp:'//img.alicdn.com/mt/TB1AlqoeGWs3KVjSZFxXXaWUXXa-640-360.jpg_120x120q90.jpg_.webp',
           bt:'糖酥饼真香警告',
           nr:'就是这样充满烟火气的食物，总是深深虏获了大人小孩的心。。'
         },
         {
           tp:"//img.alicdn.com/mt/TB1qv5geRWD3KVjSZFsXXcqkpXa-640-398.jpg_120x120q90.jpg_.webp",
           bt:"扦插花卉不生根？教你3分钟学“高压”",
           nr:'喜欢养花的人越来越多，想必很多花友经常会去花店或者花卉市场买一些绿植盆栽养在家里，当然随着养花的经验越来越足，很多花友也会通过播种繁殖、扦插繁殖、分株繁殖和高压繁殖来获得大量花卉盆栽。'
         },
          {
           tp:'//img.alicdn.com/mt/TB1TgefeLWG3KVjSZFgXXbTspXa-790-552.jpg_120x120q90.jpg_.webp',
           bt:'糖酥饼真香警告',
           nr:'就是这样充满烟火气的食物，总是深深虏获了大人小孩的心。。'
         },
               {
           tp:"//img.alicdn.com/mt/TB1qv5geRWD3KVjSZFsXXcqkpXa-640-398.jpg_120x120q90.jpg_.webp",
           bt:"夏日降温偏方，北欧风清新卫浴这般造”",
           nr:'比起大动干戈的客厅打造，独爱那温馨的卫浴空间，任由安静的色泽与各好物发光发热，由此打造远离尘世的北欧空间，上演一出以无胜多的神奇逆袭，将清新感贯穿于细节之中，从此解禁夏日凉爽，get全新的降温时光。'
         },

 
       ],
       tbs:[
           '//img.alicdn.com/tfs/TB1qpwlQXXXXXcCXXXXXXXXXXXX-256-256.png_60x60.jpg',
           '//img.alicdn.com/tps/i3/TB1DGkJJFXXXXaZXFXX07tlTXXX-200-200.png_60x60.jpg',
           "//img.alicdn.com/tps/i4/TB1CKSgIpXXXXccXXXX07tlTXXX-200-200.png_60x60.jpg",
           '//img.alicdn.com/tps/i4/TB1zkDeIFXXXXXrXVXX07tlTXXX-200-200.png_60x60.jpg',
           '//img.alicdn.com/tps/i4/TB1zkDeIFXXXXXrXVXX07tlTXXX-200-200.png_60x60.jpg',
          '//img.alicdn.com/tps/i4/TB1zkDeIFXXXXXrXVXX07tlTXXX-200-200.png_60x60.jpg',
          '//img.alicdn.com/tps/i3/TB1DGkJJFXXXXaZXFXX07tlTXXX-200-200.png_60x60.jpg',
            '//img.alicdn.com/tfs/TB1qpwlQXXXXXcCXXXXXXXXXXXX-256-256.png_60x60.jpg', 
           "//img.alicdn.com/tps/i4/TB1CKSgIpXXXXccXXXX07tlTXXX-200-200.png_60x60.jpg",
           '//img.alicdn.com/tps/i4/TB1zkDeIFXXXXXrXVXX07tlTXXX-200-200.png_60x60.jpg',
       ],
       notices:[
         '聚划算效应全面爆发 ',
          '天天都是品牌双11',
          '聚划算效应全面爆发 ',
          '天天都是品牌双11',
       ],
        notices2:[
         '新增《淘宝网汽配行业 ',
          '《淘宝网区域零售服务',

       ],
       mains:[
         {
           title:'有好货',
           stitle:'与品质生活不期而遇',
            tp:'//img.alicdn.com/tfscom/i2/33889958/TB2SlTgeheK.eBjSZFuXXcT4FXa_!!33889958.jpg_180x180xzq90.jpg_.webp',
            ms:'粉格小地毯 满足你的少女心',
            pj:'67人说好',
         },
          {
           title:'爱逛街',
           stitle:'献给聪明可爱的你',
            tp:'//img.alicdn.com/imgextra/i4/128864177/TB2E8HiaPv85uJjSZFNXXcJApXa_!!128864177-0-beehive-scenes.jpg_180x180xzq90.jpg_.webp',
            ms:'"可外穿的森系风家居服"',
            pj:"67人说好",
         },
                {
           title:'有好货',
           stitle:'与品质生活不期而遇',
            tp:'//img.alicdn.com/tfscom/i2/33889958/TB2SlTgeheK.eBjSZFuXXcT4FXa_!!33889958.jpg_180x180xzq90.jpg_.webp',
            ms:'粉格小地毯 满足你的少女心',
            pj:'67人说好',
         },
          {
           title:'爱逛街',
           stitle:'献给聪明可爱的你',
            tp:'//img.alicdn.com/imgextra/i4/128864177/TB2E8HiaPv85uJjSZFNXXcJApXa_!!128864177-0-beehive-scenes.jpg_180x180xzq90.jpg_.webp',
            ms:'"可外穿的森系风家居服"',
            pj:"67人说好",
         },
  
       ],
       buys:[
        {
          image:"//img.alicdn.com/tps/i4/O1CN01eMfSlY1qK3PPoI9Fh_!!0-juitemmedia.jpg_180x180q90.jpg_.webp",
          ms:'【反季清仓】儿童轻薄羽绒服',
          yh:'前500名卷后价39.9',
          jg:'￥269.00',
        },
        {
          image:"//img.alicdn.com/tps/i3/1048605002402100672/TB2DmoTdYJmpuFjSZFBXXXaZXXa_!!2-juitemmedia.png_180x180q90.jpg_.webp",
          ms:'康佳电烤箱迷你家用烘焙12L',
          yh:'前200名领券减20',
          jg:'￥199.00',
        },
        {
          image:"//img.alicdn.com/tps/TB1ZV9TQ9rqK1RjSZK9SutyypXa.jpg_180x180q90.jpg_.webp",
          ms:'必抢/新款天鹅镂空机械女表',
          yh:'直降300 送手镯',
          jg:'￥1399.00',
        },
       ],
       ends:[
           {
             title:'消费者保障',
             spans:[
               '保障范围',
                '退货退款流程',
                '服务中心',
                '更多特色服务',
             ]
           },
             {
             title:'新手上路',
             spans:[
               '新手专区',
               '消费警示', 
               '交易安全', 
               '24小时在线帮助', 
               '免费开店',
             ]
           },
             {
             title:'付款方式',
             spans:[
               '快捷支付',
                '信用卡', 
                '余额宝', 
                '蚂蚁花呗', 
                '货到付款'
             ]
           },
             {
             title:'淘宝特色',
             spans:[
               '手机淘宝',
                '旺旺/旺信',
                '大众评审'
             ]
           },
       ],
       ljs:[
            '阿里巴巴集团',
            '淘宝网',
            '天猫',
            '聚划算',
            '全球速卖通',
            '阿里巴巴国际交易市场',
            '1688',
            '阿里妈妈',
            '飞猪',
            '阿里云计算',
            'AliOS',
            '阿里通信',
            '一淘',
            '万网',
            '高德',
            'UC',
            '友盟',
            '虾米',
            '大麦网',
            '钉钉',
            '支付宝',
            '优酷',
            '土豆',
            '阿里健康',
            '阿里影业',
            '阿里体育',
            '网商银行',
       ],
       messages:[
      '关于淘宝',
      '合作伙伴',
      '营销中心',
      '廉正举报',
      '联系客服',
      '开放平台',
      '诚征英才',
      '联系我们',
      '网站地图',
      '隐私权政策',
      '法律声明',
      '知识产权 ',
'增值电信业务经营许可证：浙B2-20080224',
'增值电信业务经营许可证（跨地区）： B2-20150210',
'浙网文（2019）1033-086号',
       ],
       messages2:[
'互联网药品信息服务资格证书（浙）-经营性-2018-0010',
'短消息类服务接入代码使用证书：号【2016】00154-A01',
'信息网络传播视听许可证：1109364号',
'出版物网络交易平台服务经营备案号：新出发浙备字第002号',
'浙公网安备 33010002000078号 ',
 '广播电视节目制作经营许可证（浙）字第01012号|市场名称登记证：工商网市字3301004120号',
 '医疗器械网络交易服务第三方平台备案：（浙）网械平台备字[2018]第00004号',
       ],
     }
  },
    methods: {
   test(e){
     const a = 1
        alert('fdg')
   },
          a(){
          this.flag=true;
          this.flag2=false;
          this.flag3=false;
          this.flag4=false;
          this.flag5=false;
          this.ys={
            "border-bottom":'2px red solid'
          }
           this.ys2={
            "border-bottom":'none'
          }
            this.ys3={
            "border-bottom":'none'
          }
              this.ys4={
            "border-bottom":'none'
          }
            this.ys5={
            "border-bottom":'none'
          }
           },
           a2(){
          this.flag2=true;
          this.flag=false;
          this.flag3=false;
          this.flag4=false;
          this.flag5=false;
               this.ys2={
            "border-bottom":'2px red solid'
          }
           this.ys={
            "border-bottom":'none'
          }
            this.ys3={
            "border-bottom":'none'
          }
              this.ys4={
            "border-bottom":'none'
          }
            this.ys5={
            "border-bottom":'none'
          }


           },
             a3(){
          this.flag3=true;
          this.flag=false;
          this.flag2=false;
          this.flag4=false;
          this.flag5=false;
               this.ys3={
            "border-bottom":'2px red solid'
          }
           this.ys2={
            "border-bottom":'none'
          }
            this.ys={
            "border-bottom":'none'
          }
              this.ys4={
            "border-bottom":'none'
          }
            this.ys5={
            "border-bottom":'none'
          }
           },
                   a4(){
          this.flag4=true;
          this.flag=false;
          this.flag2=false;
          this.flag3=false;
          this.flag5=false;
               this.ys4={
            "border-bottom":'2px red solid'
          }
           this.ys2={
            "border-bottom":'none'
          }
            this.ys={
            "border-bottom":'none'
          }
              this.ys3={
            "border-bottom":'none'
          }
            this.ys5={
            "border-bottom":'none'
          }
           },
                   a5(){
          this.flag5=true;
          this.flag=false;
          this.flag2=false;
          this.flag4=false;
          this.flag3=false;
               this.ys5={
            "border-bottom":'2px red solid'
          }
           this.ys2={
            "border-bottom":'none'
          }
            this.ys={
            "border-bottom":'none'
          }
              this.ys4={
            "border-bottom":'none'
          }
            this.ys3={
            "border-bottom":'none'
          }
           },
           isshow(){
             this.isflag=true;
           },
           noshow(){
             this.isflag=false;
            //  this.navstyle={
            //    'border':'1px red solid',
            //  }
           },
           no(){
              this.ifnav=false;
              this.ifnav2=false;
              this.ifnav3=false;
                    this.navstyle={
               'border': '1px #D3D3D3 solid'
             };
                  this.navstyle2={
               'border': '1px #D3D3D3 solid'
             }
                    this.navstyle3={
               'border': '1px #D3D3D3 solid'
             }
                         this.navstyle4={
               'border': '1px #D3D3D3 solid'
             }
           },
           navshow(){
             this.ifnav=true;
             this.ifnav2=false;
             this.ifnav3=false;
             this.navstyle={
               'border':'1px red solid',
               'border-bottom':"none"
             }
                  this.navstyle2={
         'border': '1px #D3D3D3 solid',
         'border-bottom': '1px red solid'
             }
                       this.navstyle3={
         'border': '1px #D3D3D3 solid',
          'border-bottom': '1px red solid'
             }
                             this.navstyle4={
         'border': '1px #D3D3D3 solid',
          'border-bottom': '1px red solid'
             }
           },
           navshow2(){
             this.ifnav2=true;
             this.ifnav=false;
             this.ifnav3=false;
             this.navstyle2={
               'border':'1px red solid',
               'border-bottom':"none"
             }
             this.navstyle3={
         'border': '1px #D3D3D3 solid',
          'border-bottom': '1px red solid'
             }
                this.navstyle={
         'border': '1px #D3D3D3 solid',
          'border-bottom': '1px red solid'
             }
                    this.navstyle4={
         'border': '1px #D3D3D3 solid',
          'border-bottom': '1px red solid'
             }
           },
              navshow3(){
             this.ifnav3=true;
             this.ifnav=false;
              this.ifnav2=false;
             this.navstyle3={
               'border':'1px red solid',
               'border-bottom':"none"
             }
                    this.navstyle={
         'border': '1px #D3D3D3 solid',
          'border-bottom': '1px red solid'
             }
                  this.navstyle2={
         'border': '1px #D3D3D3 solid',
          'border-bottom': '1px red solid'
             }
                        this.navstyle4={
         'border': '1px #D3D3D3 solid',
          'border-bottom': '1px red solid'
             }
           },


           
    }
      
  }
</script>

<style >
*{
  padding: 0px;
  margin: 0px;

}
.home{
  width:100%;
  background: #f4f4f4;
}
header{
  width:1500px;
  margin:0px auto ;
  
  
 


  

  
 
  
}
.count{
  width:100%;
  margin:0px auto ;
  background: #FF5900;

  


  
  
 
}
.nav li{
  text-align: center;
  list-style: none;
  width:193px;
  height:30px;
  line-height: 30px;
  margin: 5px 0px;
  color: gray;
  



}
  .el-menu-vertical-demo:not(.el-menu--collapse) {
    width: 200px;
    min-height: 400px;
  }
  .list{
    height:45px !important;
    line-height: 45px !important;
    margin:0px !important;
    width:197px !important;
  }
  .el-carousel__item img {
     width: 580px;
     height:280px;
   
  }

  .button{
  text-decoration: none;
   width:80px;
   height:25px;
   line-height: 25px;
   text-align: center;
   background:#FF5900;
   border-radius: 5px;
   font-size: 12px;
  font-weight: 400px;
   color:white;
   cursor: pointer;
   
  }
  .litter-nav{
    list-style: none;
    width:60px;
    text-align: center;
    height:21px;
    cursor: pointer;
  }
  .cont{
    width:100%;
    height:80px;
    display: flex;
    flex-wrap:wrap
  }
  .cont-list{
   margin:10px 20px;
   font-size:14px;
   font-weight:400px; 
   display:flex;
   cursor: pointer;
  }
  .nav-list{
    list-style: none;
    line-height: 87px;
    width:80px;
    height:87px;
    border: 1px #D3D3D3 solid;
    display: flex;
    cursor: pointer; 
    align-content: center;
    justify-content: center;
  }
  .headline{
    width:1316px;
    height:100px;
    background: white;
    margin:10px auto;
     display: flex;
      background-color: #d3dce6;
    
     
     
    
  }
  .headline-background{
     width:198px;
     height:100px;
     background:url('//img.alicdn.com/tfs/TB1KbhkbUgQMeJjy0FeXXXOEVXa-129-26.png') no-repeat;
     background-position: 50%;
      display: flex;  
      align-items: flex-end;
  }
 .headline  .headline-img{
   height:80px;
   width:120px;
   margin:10px 0px;
   display: flex;
  }
  .headline .headline-p{
    display: flex;
    margin:10px 20px;
    color:#333;
    font-weight:500px;
    height:20px;
    font-size:16px;
      cursor: pointer;
  }
  .headline .headline-span{
    width:593px;
    color:#999;
    height:67px; 
     position: absolute; 
     top: 36px; 
     left: 141px; 
     overflow: hidden;
     font-size:14px;  
    cursor: pointer;
  }
  .main{
    width:1320px;

    background: white;
    margin:20px auto;

  }
  .main-cont{
    width:100%;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;


  }
  .text {
    font-size: 14px;
  }

  .item {
    margin-bottom: 18px;
   display: flex;
   flex-wrap: wrap;
   
  }
.clearfix{
  display: flex;
  justify-content: space-between;
}
  .box-card {
    width: 645px;
    margin-top: 20px; 
  }
  .end{
width:260px;
height:140px;
margin-top:20px;
color:black;
  }
  .end-main{
 font-size:18px;
 text-align:left;
 margin-top: 10px;
 margin-left:12px;

  }
  .spans{
font-size: 14px;
margin:5px 10px;
color:#4f4f4f;

  }
.ljs{
  margin-right:15px;
}
</style>