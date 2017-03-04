# tips_xcConfirm
JS弹窗DEMO

#使用引用
 ><link rel="stylesheet" type="text/css" href="css/xcConfirm.css"/>
		<script src="js/jquery-1.9.1.js" type="text/javascript" charset="utf-8"></script>
		<script src="js/xcConfirm.js" type="text/javascript" charset="utf-8"></script>
    
    
#demo
$("#btn1").click(function(){
					var txt=  "提示文字，提示文字，提示文字，提示文字，提示文字，提示文字";
					window.wxc.xcConfirm(txt, window.wxc.xcConfirm.typeEnum.info);
				});
				
				$("#btn2").click(function(){
					var txt=  "提示文字，提示文字，提示文字，提示文字，提示文字，提示文字";
					window.wxc.xcConfirm(txt, window.wxc.xcConfirm.typeEnum.confirm);

				});
				
				$("#btn3").click(function(){
					var txt=  "提示文字，提示文字，提示文字，提示文字，提示文字，提示文字";
					window.wxc.xcConfirm(txt, window.wxc.xcConfirm.typeEnum.warning);
				});
				
				$("#btn4").click(function(){
					var txt=  "提示文字，提示文字，提示文字，提示文字，提示文字，提示文字";
					window.wxc.xcConfirm(txt, window.wxc.xcConfirm.typeEnum.error);
				});
				
				$("#btn5").click(function(){
					var txt=  "提示文字，提示文字，提示文字，提示文字，提示文字，提示文字";
					window.wxc.xcConfirm(txt, window.wxc.xcConfirm.typeEnum.success);
				});
				
				$("#btn6").click(function(){
					var txt=  "请输入";
					window.wxc.xcConfirm(txt, window.wxc.xcConfirm.typeEnum.input,{
						onOk:function(v){
							console.log(v);
						}
					});
				});
				
				$("#btn7").click(function(){
					var txt=  "自动应以呀";
					var option = {
						title: "自定义",
						btn: parseInt("0011",2),
						onOk: function(){
							console.log("确认啦");
						}
					}
					window.wxc.xcConfirm(txt, "custom", option);
				});
				
				$("#btn8").click(function(){
					var txt=  "默认";
					window.wxc.xcConfirm(txt);
				});
