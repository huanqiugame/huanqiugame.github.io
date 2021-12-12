# 欢迎

欢迎来到我的博客！我是浣秋，一位在校学生。在这里，我会书写我的感受与想法，以及我认为值得记录的、发生在我身边的每一件事。

因为学业关系，我不可能做到每日更新，但会尽量做到至少每周都能更新。

**请看好现在地址栏中的网址！**我有时也会在这里发布一些我感兴趣的内容，有可能是陈述，也有可能是教程。总之，**如果你想要转载（引用除外）此网站上的任何内容，请注明出处。**

> 让我们开始吧：
>
>  [阅读我的日记体博客](Daily/Daily.md) 
>
>  [阅读其他类型文章](杂项/杂项.md) 

# 关于我自己

这个网站是我在不久前（2021年11月初）建立的，因此内容非常非常少。以后我会尽力扩充内容。

如果你有任何意见或建议，欢迎给我的邮箱（huanqiu_myworld@163.com）发送邮件，也可以通过下面的表单给我发送消息。

<form id="my-form" action="https://formspree.io/f/mdoyqljy" method="POST">
  <label>您的电子邮件地址，以便我们联系您：</label>
  <br />
  <textarea rows="1" cols="50" style="font-size:20px" name="email" placeholder="非必填"></textarea>
  <br />
  <label>您的建议或意见：</label>
  <br />
  <textarea rows="10" cols="50" style="font-size:20px" name="message" required="required"></textarea>
  <button id="my-form-button" style="font-size:20">提交</button>
  <p id="my-form-status"></p>
</form>
<script>
    var form = document.getElementById("my-form");
  async function handleSubmit(event) {
  event.preventDefault();
  var status = document.getElementById("my-form-status");
  var data = new FormData(event.target);
  fetch(event.target.action, {
    method: form.method,
    body: data,
    headers: {
        'Accept': 'application/json'
    }
  }).then(response => {
    status.innerHTML = "感谢您的建议！";
    form.reset()
  }).catch(error => {
    status.innerHTML = "Oh, no！你的建议提交失败，请稍后再试。"
  });
}
form.addEventListener("submit", handleSubmit)
</script>




# 友情链接

- [macwk.com](https://macwk.com) - 提供各种macOS软件的破解版
- [macloudtv.com](https://macloudtv.com) - 休康，多年Mac教学经验，各类macOS使用上的疑难解答
- [616.sb](https://616.sb) - 小型音游的下载站，原[konmai.cn](https://konmai.cn)
- [PojavLauncher](https://github.com/PojavLauncherTeam/PojavLauncher/) - 一款可以在手机上运行Minecraft Java版的软件，没有防沉迷限制。

<p style="color:gray"><code>Version 0.0.2</code></p>
