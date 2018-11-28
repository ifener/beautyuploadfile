# beautyuploadfile

![Image text](https://raw.githubusercontent.com/ifener/beautyuploadfile/master/images/2018-11-28_16-32-43.jpg)

一个将上传组件美化的JQuery插件,用法(how to use)：
<pre>
    $("#file").beautyfileupload({});
</pre>
可限制文件的类型及回调：
<pre>
$("#file").beautyfileupload({
     allowExtensions:[".zip"],
     allowExtensionErrorHandler:function(){
        $(this).val('');
        alert("文件格式不正确");
    },
    okHandler:function(e){
       alert("ok"+this)
    }
 });
</pre>
