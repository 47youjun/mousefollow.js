# mousefollow.js


#默认参数：

			className: 'js-follow',  // 插入的div的class
			html: '',                // 插入的html
			speed: 200,              // 淡出速度
			x: 20,                   // 距离鼠标的水平距离
			y: 20                    // 距离鼠标的垂直距离

#使用demo：
![image](https://github.com/YuTingtao/mousefollow.js/blob/master/images/eg-1.gif)

html：

	<ul class="imglist eg-2">
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
	</ul>
  
	<ul class="imglist eg-2">
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
		<li><a href="#"></a></li>
	</ul>
  
  js：
  
	<script src="js/jquery-1.8.3.min.js"></script>
	<script src="js/jquery.mousefollow.js"></script>
	<script tpye="text/javascript">
    $(function(){
      $('.eg-1 li').each(function(index, el) {
        var imgUrl = $(el).data('imgurl');
        $(el).mousefollow({
          html: '<img src="'+imgUrl+'" alt="">'
        });
      });

      $('.eg-2 li').mousefollow({
        html: '<div class="hidden-box"><img src="images/2.jpg" alt=""><p>图片1</p></div>',
        speed: 0
      });
    });
	</script>
  
