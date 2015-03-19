协议和技术细节

[原网站](http://developer.wandoujia.com/search/details/)


目录：

[第一步：使 App 支持外部调起](#standard)

[第二步：描述 App 内容](#process)

[第三步：提交 AppURL 和 App 内容等信息](#promotion)

[豌豆荚支持的其他标准](#otherstandard)

# <a name="standard"></a>**第一步：使 App 支持外部调起**

为了使用户能够从豌豆荚的搜索结果中打开应用内容，开发者需要使 App 支持外部调用。豌豆荚使用 AppURL 来指向一个可以在 App 中展现的资源，AppURL 的格式：

**_{scheme}://{host_path}_**

### 制定统一的 URI 指向 App 的内容

我们推荐开发者将 scheme 设为 app_name，将 host_path 设为 page/type/id，也就是使用 app_name://page/type/id 的方式来指向 App 的内容。例如，一个优酷的视频播放页可以被描述为：youku://play/video/12321；一个多看的电子书详情页可以被描述为：duokan://detail/ebook/21312。

### 在 Android Manifest 文件中注册 intent-filter

对于一个可以展示 **_{app_name}://{page}/{type}/{id}_** 所指向资源的 activity 添加如下 intent-filter：
<!-- Crayon Syntax Highlighter v2.5.0 -->

		<div id="crayon-550a253e5503b634868329" class="crayon-syntax crayon-theme-arduino-ide crayon-font-monaco crayon-os-pc print-yes notranslate" data-settings=" minimize scroll-mouseover" style=" margin-top: 12px; margin-bottom: 12px; float: none; clear: both; font-size: 12px !important; line-height: 15px !important;">

			<div class="crayon-toolbar" data-settings=" mouseover overlay hide delay" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><span class="crayon-title"></span>
			<div class="crayon-tools" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><div class="crayon-button crayon-nums-button" title="Toggle Line Numbers"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-plain-button" title="Toggle Plain Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-wrap-button" title="Toggle Line Wrap"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-expand-button" title="Expand Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-copy-button" title="Copy"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-popup-button" title="Open Code In New Window"><div class="crayon-button-icon"></div></div><span class="crayon-language">XHTML</span></div></div>
			<div class="crayon-info" style="min-height: 16.8px !important; line-height: 16.8px !important;"></div>
			<div class="crayon-plain-wrap"><textarea wrap="soft" class="crayon-plain print-no" data-settings="dblclick" readonly style="-moz-tab-size:4; -o-tab-size:4; -webkit-tab-size:4; tab-size:4; font-size: 12px !important; line-height: 15px !important;">
&lt;intent-filter&gt;
    &lt;action android:name="android.intent.action.VIEW" /&gt;
    &lt;category android:name="android.intent.category.DEFAULT" /&gt;
    &lt;!-- 处理以"app_name://page/type"开头的 URI --&gt;
    &lt;data android:scheme="app_name" /&gt;
    &lt;data android:host="detail" /&gt;
    &lt;data android:path="/type" /&gt;
&lt;/intent-filter&gt;</textarea></div>
			<div class="crayon-main" style="">
				<table class="crayon-table">
					<tr class="crayon-row">
				<td class="crayon-nums " data-settings="hide">
					<div class="crayon-nums-content" style="font-size: 12px !important; line-height: 15px !important;"><div class="crayon-num" data-line="crayon-550a253e5503b634868329-1">1</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e5503b634868329-2">2</div><div class="crayon-num" data-line="crayon-550a253e5503b634868329-3">3</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e5503b634868329-4">4</div><div class="crayon-num" data-line="crayon-550a253e5503b634868329-5">5</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e5503b634868329-6">6</div><div class="crayon-num" data-line="crayon-550a253e5503b634868329-7">7</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e5503b634868329-8">8</div></div>
				</td>
						<td class="crayon-code"><div class="crayon-pre" style="font-size: 12px !important; line-height: 15px !important;"><div class="crayon-line" id="crayon-550a253e5503b634868329-1"><span class="crayon-r ">&lt;intent-filter&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e5503b634868329-2"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;action </span>android<span class="crayon-o">:</span><span class="crayon-e ">name</span><span class="crayon-o">=</span><span class="crayon-s ">"android.intent.action.VIEW"</span><span class="crayon-r "> /&gt;</span></div><div class="crayon-line" id="crayon-550a253e5503b634868329-3"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;category </span>android<span class="crayon-o">:</span><span class="crayon-e ">name</span><span class="crayon-o">=</span><span class="crayon-s ">"android.intent.category.DEFAULT"</span><span class="crayon-r "> /&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e5503b634868329-4"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-c">&lt;!-- 处理以"app_name://page/type"开头的 URI --&gt;</span></div><div class="crayon-line" id="crayon-550a253e5503b634868329-5"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;data </span>android<span class="crayon-o">:</span><span class="crayon-e ">scheme</span><span class="crayon-o">=</span><span class="crayon-s ">"app_name"</span><span class="crayon-r "> /&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e5503b634868329-6"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;data </span>android<span class="crayon-o">:</span><span class="crayon-e ">host</span><span class="crayon-o">=</span><span class="crayon-s ">"detail"</span><span class="crayon-r "> /&gt;</span></div><div class="crayon-line" id="crayon-550a253e5503b634868329-7"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;data </span>android<span class="crayon-o">:</span><span class="crayon-e ">path</span><span class="crayon-o">=</span><span class="crayon-s ">"/type"</span><span class="crayon-r "> /&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e5503b634868329-8"><span class="crayon-r ">&lt;/intent-filter&gt;</span></div></div></td>
					</tr>
				</table>
			</div>
		</div>
<!-- [Format Time: 0.0022 seconds] -->

### 使用 am 指令进行测试

通过如下指令测试调起，如果能够正确地调起页面展示数据则说明 intent-filter 设置成功。
<!-- Crayon Syntax Highlighter v2.5.0 -->

		<div id="crayon-550a253e5504c391056927" class="crayon-syntax crayon-theme-arduino-ide crayon-font-monaco crayon-os-pc print-yes notranslate" data-settings=" minimize scroll-mouseover" style=" margin-top: 12px; margin-bottom: 12px; float: none; clear: both; font-size: 12px !important; line-height: 15px !important;">

			<div class="crayon-toolbar" data-settings=" mouseover overlay hide delay" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><span class="crayon-title"></span>
			<div class="crayon-tools" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><div class="crayon-button crayon-nums-button" title="Toggle Line Numbers"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-plain-button" title="Toggle Plain Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-wrap-button" title="Toggle Line Wrap"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-expand-button" title="Expand Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-copy-button" title="Copy"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-popup-button" title="Open Code In New Window"><div class="crayon-button-icon"></div></div></div></div>
			<div class="crayon-info" style="min-height: 16.8px !important; line-height: 16.8px !important;"></div>
			<div class="crayon-plain-wrap"><textarea wrap="soft" class="crayon-plain print-no" data-settings="dblclick" readonly style="-moz-tab-size:4; -o-tab-size:4; -webkit-tab-size:4; tab-size:4; font-size: 12px !important; line-height: 15px !important;">
adb shell am start -W -a "android.intent.action.VIEW" -d "yourUri" yourPackageName</textarea></div>
			<div class="crayon-main" style="">
				<table class="crayon-table">
					<tr class="crayon-row">
				<td class="crayon-nums " data-settings="hide">
					<div class="crayon-nums-content" style="font-size: 12px !important; line-height: 15px !important;"><div class="crayon-num" data-line="crayon-550a253e5504c391056927-1">1</div></div>
				</td>
						<td class="crayon-code"><div class="crayon-pre" style="font-size: 12px !important; line-height: 15px !important;"><div class="crayon-line" id="crayon-550a253e5504c391056927-1"><span class="crayon-e">adb </span><span class="crayon-e">shell </span><span class="crayon-e">am </span><span class="crayon-i">start</span><span class="crayon-h"> </span><span class="crayon-o">-</span><span class="crayon-i">W</span><span class="crayon-h"> </span><span class="crayon-o">-</span><span class="crayon-i">a</span><span class="crayon-h"> </span><span class="crayon-s">"android.intent.action.VIEW"</span><span class="crayon-h"> </span><span class="crayon-o">-</span><span class="crayon-i">d</span><span class="crayon-h"> </span><span class="crayon-s">"yourUri"</span><span class="crayon-h"> </span><span class="crayon-i">yourPackageName</span></div></div></td>
					</tr>
				</table>
			</div>
		</div>
<!-- [Format Time: 0.0012 seconds] -->

## <a name="process"></a>**第二步：描述 App 内容**

内容是指 IAS(In App Search, 应用内搜索) 检索和展现的内容对象，同时，也是各个 App 提供给用户消费的对象。例如某一个视频就是一个典型的内容。我们将内容称为 Item，这两个概念可以互换。

一个 Item 通常包含一系列的属性，例如一部电影至少有标题、导演、演员、电影简介等等属性。而对于一部电子书或者一张图片，其包含的属性则不尽相同。

### 如何描述 App 内容

豌豆荚 IAS 使用 [Microdata](http://www.w3.org/TR/microdata/) 标准来描述一个 Item。Microdata 是 Google、Bing 和 Yahoo 都支持的结构化数据标注方案，也是 HTML5 的标准，同时也可以用 XML 来表示。下面的例子我们用 XML 来描述电影《环太平洋》：
<!-- Crayon Syntax Highlighter v2.5.0 -->

		<div id="crayon-550a253e55056136927125" class="crayon-syntax crayon-theme-arduino-ide crayon-font-monaco crayon-os-pc print-yes notranslate" data-settings=" minimize scroll-mouseover" style=" margin-top: 12px; margin-bottom: 12px; float: none; clear: both; font-size: 12px !important; line-height: 15px !important;">

			<div class="crayon-toolbar" data-settings=" mouseover overlay hide delay" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><span class="crayon-title"></span>
			<div class="crayon-tools" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><div class="crayon-button crayon-nums-button" title="Toggle Line Numbers"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-plain-button" title="Toggle Plain Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-wrap-button" title="Toggle Line Wrap"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-expand-button" title="Expand Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-copy-button" title="Copy"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-popup-button" title="Open Code In New Window"><div class="crayon-button-icon"></div></div><span class="crayon-language">XHTML</span></div></div>
			<div class="crayon-info" style="min-height: 16.8px !important; line-height: 16.8px !important;"></div>
			<div class="crayon-plain-wrap"><textarea wrap="soft" class="crayon-plain print-no" data-settings="dblclick" readonly style="-moz-tab-size:4; -o-tab-size:4; -webkit-tab-size:4; tab-size:4; font-size: 12px !important; line-height: 15px !important;">
&lt;xhtml:span itemscope="true" itemtype="http://schema.org/Movie"&gt;
    &lt;xhtml:span itemprop="name"&gt;环太平洋&lt;/xhtml:span&gt;
    &lt;xhtml:span itemprop="description"&gt;有一个名叫"凯由"的滔天外来生物从海上崛起，并且引起一场战争，这场浩劫将威胁到数百万计的人类的生命和...&lt;/xhtml:span&gt;
    &lt;xhtml:span itemprop="director" itemscope="true" itemtype="http://schema.org/Person"&gt;
        &lt;xhtml:span itemprop="name"&gt;吉尔莫·德尔·托罗&lt;/xhtml:span&gt;
    &lt;/xhtml:span&gt; 
    &lt;xhtml:span itemprop="actor" itemscope="true" itemtype="http://schema.org/Person"&gt;
        &lt;xhtml:span itemprop="name"&gt;朗·普尔曼&lt;/xhtml:span&gt;
    &lt;/xhtml:span&gt;
    &lt;xhtml:span itemprop="aggregateRating" itemscope="true" itemtype="http://schema.org/AggregateRating"&gt;
        &lt;xhtml:span itemprop="ratingValue"&gt;8&lt;/xhtml:span&gt;
        &lt;xhtml:span itemprop="bestRating"&gt;10&lt;/xhtml:span&gt;
        &lt;xhtml:span itemprop="ratingCount"&gt;200&lt;/xhtml:span&gt;
        &lt;xhtml:span itemprop="reviewCount"&gt;50&lt;/xhtml:span&gt;
    &lt;/xhtml:span&gt;
&lt;/xhtml:span&gt;</textarea></div>
			<div class="crayon-main" style="">
				<table class="crayon-table">
					<tr class="crayon-row">
				<td class="crayon-nums " data-settings="hide">
					<div class="crayon-nums-content" style="font-size: 12px !important; line-height: 15px !important;"><div class="crayon-num" data-line="crayon-550a253e55056136927125-1">1</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55056136927125-2">2</div><div class="crayon-num" data-line="crayon-550a253e55056136927125-3">3</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55056136927125-4">4</div><div class="crayon-num" data-line="crayon-550a253e55056136927125-5">5</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55056136927125-6">6</div><div class="crayon-num" data-line="crayon-550a253e55056136927125-7">7</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55056136927125-8">8</div><div class="crayon-num" data-line="crayon-550a253e55056136927125-9">9</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55056136927125-10">10</div><div class="crayon-num" data-line="crayon-550a253e55056136927125-11">11</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55056136927125-12">12</div><div class="crayon-num" data-line="crayon-550a253e55056136927125-13">13</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55056136927125-14">14</div><div class="crayon-num" data-line="crayon-550a253e55056136927125-15">15</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55056136927125-16">16</div></div>
				</td>
						<td class="crayon-code"><div class="crayon-pre" style="font-size: 12px !important; line-height: 15px !important;"><div class="crayon-line" id="crayon-550a253e55056136927125-1"><span class="crayon-r ">&lt;xhtml:span </span><span class="crayon-e ">itemscope</span><span class="crayon-o">=</span><span class="crayon-s ">"true"</span><span class="crayon-h"> </span><span class="crayon-e ">itemtype</span><span class="crayon-o">=</span><span class="crayon-s ">"http://schema.org/Movie"</span><span class="crayon-r ">&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55056136927125-2"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;xhtml:span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"name"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">环太平洋</span><span class="crayon-r ">&lt;/xhtml:span&gt;</span></div><div class="crayon-line" id="crayon-550a253e55056136927125-3"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;xhtml:span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"description"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">有一个名叫"凯由"的滔天外来生物从海上崛起，并且引起一场战争，这场浩劫将威胁到数百万计的人类的生命和...</span><span class="crayon-r ">&lt;/xhtml:span&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55056136927125-4"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;xhtml:span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"director"</span><span class="crayon-h"> </span><span class="crayon-e ">itemscope</span><span class="crayon-o">=</span><span class="crayon-s ">"true"</span><span class="crayon-h"> </span><span class="crayon-e ">itemtype</span><span class="crayon-o">=</span><span class="crayon-s ">"http://schema.org/Person"</span><span class="crayon-r ">&gt;</span></div><div class="crayon-line" id="crayon-550a253e55056136927125-5"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;xhtml:span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"name"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">吉尔莫·德尔·托罗</span><span class="crayon-r ">&lt;/xhtml:span&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55056136927125-6"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;/xhtml:span&gt;</span><span class="crayon-i "> </span></div><div class="crayon-line" id="crayon-550a253e55056136927125-7"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;xhtml:span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"actor"</span><span class="crayon-h"> </span><span class="crayon-e ">itemscope</span><span class="crayon-o">=</span><span class="crayon-s ">"true"</span><span class="crayon-h"> </span><span class="crayon-e ">itemtype</span><span class="crayon-o">=</span><span class="crayon-s ">"http://schema.org/Person"</span><span class="crayon-r ">&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55056136927125-8"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;xhtml:span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"name"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">朗·普尔曼</span><span class="crayon-r ">&lt;/xhtml:span&gt;</span></div><div class="crayon-line" id="crayon-550a253e55056136927125-9"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;/xhtml:span&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55056136927125-10"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;xhtml:span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"aggregateRating"</span><span class="crayon-h"> </span><span class="crayon-e ">itemscope</span><span class="crayon-o">=</span><span class="crayon-s ">"true"</span><span class="crayon-h"> </span><span class="crayon-e ">itemtype</span><span class="crayon-o">=</span><span class="crayon-s ">"http://schema.org/AggregateRating"</span><span class="crayon-r ">&gt;</span></div><div class="crayon-line" id="crayon-550a253e55056136927125-11"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;xhtml:span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"ratingValue"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">8</span><span class="crayon-r ">&lt;/xhtml:span&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55056136927125-12"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;xhtml:span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"bestRating"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">10</span><span class="crayon-r ">&lt;/xhtml:span&gt;</span></div><div class="crayon-line" id="crayon-550a253e55056136927125-13"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;xhtml:span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"ratingCount"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">200</span><span class="crayon-r ">&lt;/xhtml:span&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55056136927125-14"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;xhtml:span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"reviewCount"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">50</span><span class="crayon-r ">&lt;/xhtml:span&gt;</span></div><div class="crayon-line" id="crayon-550a253e55056136927125-15"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;/xhtml:span&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55056136927125-16"><span class="crayon-r ">&lt;/xhtml:span&gt;</span></div></div></td>
					</tr>
				</table>
			</div>
		</div>
<!-- [Format Time: 0.0075 seconds] -->

下面是几个属性的说明：

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th  style="text-align:left" >属性</th>
<th  style="text-align:left" >描述</th>
<th style="text-align:left;width:50px">是否必须</th>
<th  style="text-align:left" >说明</th>
</tr>
</thead>
<tbody>
<tr><td  style="text-align:left" >itemprop</td>
<td  style="text-align:left" >属性名</td>
<td  style="text-align:left" >必须</td>
<td  style="text-align:left" >属性的名字</td>
</tr>

<tr><td  style="text-align:left" >itemscope</td>
<td  style="text-align:left" >取值为 true 或者 false</td>
<td  style="text-align:left" >可选</td>
<td  style="text-align:left" >带有 itemscope 的属性是特殊类型（有自己的属性），例如 Person</td>
</tr>

<tr><td  style="text-align:left" >itemtype</td>
<td  style="text-align:left" >属性的类型</td>
<td  style="text-align:left" ></td>
<td  style="text-align:left" >只有在 itemscope 出现的时候需要指定。itemtype 的值为 “http://schema.org/{type}”，其中 {type} 是该属性的类型。例如，actor 属性的类型是 Person，那么 actor 对应的 itemtype="http://schema.org/Person"</td>
</tr>
</tbody></table>

为了方便各类内容顺利接入 IAS，豌豆荚对一些特定种类的内容会给出明确的数据组织标准，也就是定义其应该包含哪些属性。对于其余类别，豌豆荚提供了一个通用的数据组织标准。具体细节请阅读[豌豆荚应用内搜索 Item 数据标准](http://developer.wandoujia.com/search/details/items/)以及[说明](http://developer.wandoujia.com/search/details/items/#explain)。

[这里](http://developer.wandoujia.com/search/details/examples/#common)列出了不同种类的 Item 分别用 XML 格式表示的示例。

# <a name="promotion"></a>**第三步：提交 AppURL 和 App 内容等信息**

在完成了上述步骤后，开发者需要通过[开发者中心](http://open.wandoujia.com/ias)将以下信息提交给豌豆荚：

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th  style="text-align:left" >需要提交的信息</th>
<th  style="text-align:left" >描述</th>
</tr>
</thead>
<tbody>
<tr><td  style="text-align:left" >AppURL</td>
<td  style="text-align:left" >App 内容的 URI</td>
</tr>

<tr><td  style="text-align:left" >Item</td>
<td  style="text-align:left" >App 内容</td>
</tr>

<tr><td  style="text-align:left" >packageName</td>
<td  style="text-align:left" >应用的包名</td>
</tr>

<tr><td  style="text-align:left" >minVersion</td>
<td  style="text-align:left" >支持从外部调用的最小版本号</td>
</tr>
</tbody></table>

我们提供了一种扩展的 [Sitemap 协议](http://www.sitemaps.org/)让开发者提交这些信息。下面是一个例子：

<!-- Crayon Syntax Highlighter v2.5.0 -->

		<div id="crayon-550a253e55071949960445" class="crayon-syntax crayon-theme-arduino-ide crayon-font-monaco crayon-os-pc print-yes notranslate" data-settings=" minimize scroll-mouseover" style=" margin-top: 12px; margin-bottom: 12px; float: none; clear: both; font-size: 12px !important; line-height: 15px !important;">

			<div class="crayon-toolbar" data-settings=" mouseover overlay hide delay" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><span class="crayon-title"></span>
			<div class="crayon-tools" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><span class="crayon-mixed-highlight" title="Contains Mixed Languages"></span><div class="crayon-button crayon-nums-button" title="Toggle Line Numbers"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-plain-button" title="Toggle Plain Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-wrap-button" title="Toggle Line Wrap"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-expand-button" title="Expand Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-copy-button" title="Copy"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-popup-button" title="Open Code In New Window"><div class="crayon-button-icon"></div></div><span class="crayon-language">XHTML</span></div></div>
			<div class="crayon-info" style="min-height: 16.8px !important; line-height: 16.8px !important;"></div>
			<div class="crayon-plain-wrap"><textarea wrap="soft" class="crayon-plain print-no" data-settings="dblclick" readonly style="-moz-tab-size:4; -o-tab-size:4; -webkit-tab-size:4; tab-size:4; font-size: 12px !important; line-height: 15px !important;">
&lt;?xml version="1.0" encoding="UTF-8"?&gt;
&lt;urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9" xmlns:ias="http://www.wandoujia.com/ias/schemas/1.0" xmlns:xhtml="http://www.w3.org/1999/xhtml"&gt;
    &lt;ias:app minVersion="489" packageName="com.example.android"/&gt;
    &lt;url&gt;
        &lt;loc&gt;http://v.example.com/xxx.html&lt;/loc&gt;
        &lt;lastmod&gt;2013-10-1&lt;/lastmod&gt;
        &lt;xhtml:link href="example://play/movie/xxx" rel="alternate"/&gt;
        &lt;xhtml:span itemscope="true" itemtype="http://schema.org/Movie"&gt;
            &lt;xhtml:span itemprop="name"&gt;环太平洋&lt;/xhtml:span&gt;
            &lt;xhtml:span itemprop="description"&gt;有一个名叫&amp;quot;凯由&amp;quot;的滔天外来生物从海上崛起...&lt;/xhtml:span&gt;
        &lt;/xhtml:span&gt;
    &lt;/url&gt;
&lt;/urlset&gt;</textarea></div>
			<div class="crayon-main" style="">
				<table class="crayon-table">
					<tr class="crayon-row">
				<td class="crayon-nums " data-settings="hide">
					<div class="crayon-nums-content" style="font-size: 12px !important; line-height: 15px !important;"><div class="crayon-num" data-line="crayon-550a253e55071949960445-1">1</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55071949960445-2">2</div><div class="crayon-num" data-line="crayon-550a253e55071949960445-3">3</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55071949960445-4">4</div><div class="crayon-num" data-line="crayon-550a253e55071949960445-5">5</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55071949960445-6">6</div><div class="crayon-num" data-line="crayon-550a253e55071949960445-7">7</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55071949960445-8">8</div><div class="crayon-num" data-line="crayon-550a253e55071949960445-9">9</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55071949960445-10">10</div><div class="crayon-num" data-line="crayon-550a253e55071949960445-11">11</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55071949960445-12">12</div><div class="crayon-num" data-line="crayon-550a253e55071949960445-13">13</div></div>
				</td>
						<td class="crayon-code"><div class="crayon-pre" style="font-size: 12px !important; line-height: 15px !important;"><div class="crayon-line" id="crayon-550a253e55071949960445-1"><span class="crayon-ta">&lt;?</span><span class="crayon-e">xml </span><span class="crayon-i">version</span><span class="crayon-o">=</span><span class="crayon-s">"1.0"</span><span class="crayon-h"> </span><span class="crayon-i">encoding</span><span class="crayon-o">=</span><span class="crayon-s">"UTF-8"</span><span class="crayon-ta">?&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55071949960445-2"><span class="crayon-r ">&lt;urlset </span><span class="crayon-e ">xmlns</span><span class="crayon-o">=</span><span class="crayon-s ">"http://www.sitemaps.org/schemas/sitemap/0.9"</span><span class="crayon-h"> </span>xmlns<span class="crayon-o">:</span><span class="crayon-e ">ias</span><span class="crayon-o">=</span><span class="crayon-s ">"http://www.wandoujia.com/ias/schemas/1.0"</span><span class="crayon-h"> </span>xmlns<span class="crayon-o">:</span><span class="crayon-e ">xhtml</span><span class="crayon-o">=</span><span class="crayon-s ">"http://www.w3.org/1999/xhtml"</span><span class="crayon-r ">&gt;</span></div><div class="crayon-line" id="crayon-550a253e55071949960445-3"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;ias:app </span><span class="crayon-e ">minVersion</span><span class="crayon-o">=</span><span class="crayon-s ">"489"</span><span class="crayon-h"> </span><span class="crayon-e ">packageName</span><span class="crayon-o">=</span><span class="crayon-s ">"com.example.android"</span><span class="crayon-r ">/&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55071949960445-4"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;url&gt;</span></div><div class="crayon-line" id="crayon-550a253e55071949960445-5"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;loc&gt;</span><span class="crayon-i ">http://v.example.com/xxx.html</span><span class="crayon-r ">&lt;/loc&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55071949960445-6"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;lastmod&gt;</span><span class="crayon-i ">2013-10-1</span><span class="crayon-r ">&lt;/lastmod&gt;</span></div><div class="crayon-line" id="crayon-550a253e55071949960445-7"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;xhtml:link </span><span class="crayon-e ">href</span><span class="crayon-o">=</span><span class="crayon-s ">"example://play/movie/xxx"</span><span class="crayon-h"> </span><span class="crayon-e ">rel</span><span class="crayon-o">=</span><span class="crayon-s ">"alternate"</span><span class="crayon-r ">/&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55071949960445-8"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;xhtml:span </span><span class="crayon-e ">itemscope</span><span class="crayon-o">=</span><span class="crayon-s ">"true"</span><span class="crayon-h"> </span><span class="crayon-e ">itemtype</span><span class="crayon-o">=</span><span class="crayon-s ">"http://schema.org/Movie"</span><span class="crayon-r ">&gt;</span></div><div class="crayon-line" id="crayon-550a253e55071949960445-9"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;xhtml:span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"name"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">环太平洋</span><span class="crayon-r ">&lt;/xhtml:span&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55071949960445-10"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;xhtml:span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"description"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">有一个名叫&amp;quot;凯由&amp;quot;的滔天外来生物从海上崛起...</span><span class="crayon-r ">&lt;/xhtml:span&gt;</span></div><div class="crayon-line" id="crayon-550a253e55071949960445-11"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;/xhtml:span&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55071949960445-12"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;/url&gt;</span></div><div class="crayon-line" id="crayon-550a253e55071949960445-13"><span class="crayon-r ">&lt;/urlset&gt;</span></div></div></td>
					</tr>
				</table>
			</div>
		</div>
<!-- [Format Time: 0.0083 seconds] -->

下面是几个标签的说明：

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th  style="text-align:left" >标签</th>
<th  style="text-align:left" >描述</th>
<th style="text-align:left;width:50px">是否必须</th>
<th  style="text-align:left" >说明</th>
</tr>
</thead>
<tbody>
<tr><td  style="text-align:left" >ias:app</td>
<td  style="text-align:left" >描述包名和支持从外部调用的最小版本</td>
<td  style="text-align:left" >必须</td>
<td  style="text-align:left" >属于扩展协议，豌豆荚自定义的标签。packageName 描述包名，minVersion 描述支持从外部调用的最小版本。如果应用有多个版本，比如非 HD 版和 HD 版，可以用多个 ias:app 标签来表示</td>
</tr>

<tr><td  style="text-align:left" >url</td>
<td  style="text-align:left" >包含 AppURL 和 Item 内容</td>
<td  style="text-align:left" >必须</td>
<td  style="text-align:left" >属于标准的 Sitemap 协议，可重复</td>
</tr>

<tr><td  style="text-align:left" >loc</td>
<td  style="text-align:left" >描述的是 WebURL 地址，也就是一个 web 页面的地址</td>
<td  style="text-align:left" >可选</td>
<td  style="text-align:left" >属于标准的 Sitemap 协议</td>
</tr>

<tr><td  style="text-align:left" >lastmod</td>
<td  style="text-align:left" >描述的是 App 内容最后一次修改的时间</td>
<td  style="text-align:left" >可选</td>
<td  style="text-align:left" >属于标准的 Sitemap 协议</td>
</tr>

<tr><td  style="text-align:left" >xhtml:link</td>
<td  style="text-align:left" >描述的是 WebURL 对应的 AppURL</td>
<td  style="text-align:left" >必须</td>
<td  style="text-align:left" >属于扩展协议，使用了标准的 XHTML 协议</td>
</tr>

<tr><td  style="text-align:left" >xhtml:span</td>
<td  style="text-align:left" >描述的是一个 Item</td>
<td  style="text-align:left" >必须</td>
<td  style="text-align:left" >属于扩展协议，使用了标准的 XHTML 协议</td>
</tr>
</tbody></table>

一个 Sitemap 文件中可以描述多个 Item，具体请参考 [Sitemap 文件示例](http://developer.wandoujia.com/search/details/examples/#sitemap)。Sitemap 文件的大小建议不超过 30MB。

如果应用内的内容不多，开发者可以使用一个 Sitemap 文件描述所有的内容，然后提供该 Sitemap 文件的 url 给豌豆荚即可。

如果 App 内容较多，导致单个 Sitemap 文件过大；或者每天更新的数据量比较大，App 内容提供方希望把更新的数据单独列出来，那么开发者可以将 App 内容用多个 Sitemap 文件描述，然后将这些 Sitemap 文件的地址保存在一个 [Sitemap 索引文件](http://developer.wandoujia.com/search/details/examples/#index)中。这样开发者只需要提供该 Sitemap 索引文件的 url，不再需要单独提供 Sitemap 文件的 url。

## <a name="otherstandard"></a>**豌豆荚支持的其他标准**

同时我们也支持 Google 的 App Indexing 标准和 Quixey 的 AppURL 标准。

### Google 的 App Indexing 标准

豌豆荚的标准基本上兼容 Google 的 App Indexing 标准，区别在于：Google 的 App Indexing 标准对 AppURL 的定义是：

**_android-app://{package_name}/{scheme}/{host_path}_**

同时还支持开发者在一个 Web 页面使用 link 标签来标识此 Web 页面对应的 AppURL。例如：
<!-- Crayon Syntax Highlighter v2.5.0 -->

		<div id="crayon-550a253e55083765481262" class="crayon-syntax crayon-theme-arduino-ide crayon-font-monaco crayon-os-pc print-yes notranslate" data-settings=" minimize scroll-mouseover" style=" margin-top: 12px; margin-bottom: 12px; float: none; clear: both; font-size: 12px !important; line-height: 15px !important;">

			<div class="crayon-toolbar" data-settings=" mouseover overlay hide delay" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><span class="crayon-title"></span>
			<div class="crayon-tools" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><div class="crayon-button crayon-nums-button" title="Toggle Line Numbers"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-plain-button" title="Toggle Plain Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-wrap-button" title="Toggle Line Wrap"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-expand-button" title="Expand Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-copy-button" title="Copy"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-popup-button" title="Open Code In New Window"><div class="crayon-button-icon"></div></div><span class="crayon-language">XHTML</span></div></div>
			<div class="crayon-info" style="min-height: 16.8px !important; line-height: 16.8px !important;"></div>
			<div class="crayon-plain-wrap"><textarea wrap="soft" class="crayon-plain print-no" data-settings="dblclick" readonly style="-moz-tab-size:4; -o-tab-size:4; -webkit-tab-size:4; tab-size:4; font-size: 12px !important; line-height: 15px !important;">
&lt;html&gt;
&lt;head&gt;
  ...
  &lt;link rel="alternate" href="android-app://com.dianping/shop/11566327" /&gt;
  ...
&lt;/head&gt;
&lt;body&gt; … &lt;/body&gt;</textarea></div>
			<div class="crayon-main" style="">
				<table class="crayon-table">
					<tr class="crayon-row">
				<td class="crayon-nums " data-settings="hide">
					<div class="crayon-nums-content" style="font-size: 12px !important; line-height: 15px !important;"><div class="crayon-num" data-line="crayon-550a253e55083765481262-1">1</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55083765481262-2">2</div><div class="crayon-num" data-line="crayon-550a253e55083765481262-3">3</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55083765481262-4">4</div><div class="crayon-num" data-line="crayon-550a253e55083765481262-5">5</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55083765481262-6">6</div><div class="crayon-num" data-line="crayon-550a253e55083765481262-7">7</div></div>
				</td>
						<td class="crayon-code"><div class="crayon-pre" style="font-size: 12px !important; line-height: 15px !important;"><div class="crayon-line" id="crayon-550a253e55083765481262-1"><span class="crayon-r ">&lt;html&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55083765481262-2"><span class="crayon-r ">&lt;head&gt;</span></div><div class="crayon-line" id="crayon-550a253e55083765481262-3"><span class="crayon-i ">&nbsp;&nbsp;...</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55083765481262-4"><span class="crayon-i ">&nbsp;&nbsp;</span><span class="crayon-r ">&lt;link </span><span class="crayon-e ">rel</span><span class="crayon-o">=</span><span class="crayon-s ">"alternate"</span><span class="crayon-h"> </span><span class="crayon-e ">href</span><span class="crayon-o">=</span><span class="crayon-s ">"android-app://com.dianping/shop/11566327"</span><span class="crayon-r "> /&gt;</span></div><div class="crayon-line" id="crayon-550a253e55083765481262-5"><span class="crayon-i ">&nbsp;&nbsp;...</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55083765481262-6"><span class="crayon-r ">&lt;/head&gt;</span></div><div class="crayon-line" id="crayon-550a253e55083765481262-7"><span class="crayon-r ">&lt;body&gt;</span><span class="crayon-i "> … </span><span class="crayon-r ">&lt;/body&gt;</span></div></div></td>
					</tr>
				</table>
			</div>
		</div>
<!-- [Format Time: 0.0010 seconds] -->

这样就通过 link 标签定义了此 Web 页面对应的 AppURL。然后开发者可以在此页面中加入 Microdata 的标签来描述对应的 Item。这种方式要求 App 的所有内容都必须有对应的 Web 页面，好处是不再需要提交另外的数据。

详细信息请阅读：[https://developers.google.com/app-indexing/](https://developers.google.com/app-indexing/)

### Quixey 的 AppURL 标准

Quixey 的 AppURL 是一个跨平台的描述应用内资源的方案，跟 Google 的 App Indexing 类似，AppURL 也是建立了 Web 地址和 App 内容之间的对应关系，只是描述方式不一样而已。

开发者需要在自己的网站下面放置一个 appurl.json 文件，这个文件描述了 Web 地址和 AppURL 的对应规则，以及在不同平台上应用的版本信息等等。例如：你有一个域名为 http://example.com 的网站，你需要将以 http://example.com 开头的 URL 映射成移动应用中的内容。你需要做的就是在网站根目录下放置一个名为 appurl.json 的文件。文件内容是：
<!-- Crayon Syntax Highlighter v2.5.0 -->

		<div id="crayon-550a253e55089026389633" class="crayon-syntax crayon-theme-arduino-ide crayon-font-monaco crayon-os-pc print-yes notranslate" data-settings=" minimize scroll-mouseover" style=" margin-top: 12px; margin-bottom: 12px; float: none; clear: both; font-size: 12px !important; line-height: 15px !important;">

			<div class="crayon-toolbar" data-settings=" mouseover overlay hide delay" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><span class="crayon-title"></span>
			<div class="crayon-tools" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><div class="crayon-button crayon-nums-button" title="Toggle Line Numbers"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-plain-button" title="Toggle Plain Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-wrap-button" title="Toggle Line Wrap"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-expand-button" title="Expand Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-copy-button" title="Copy"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-popup-button" title="Open Code In New Window"><div class="crayon-button-icon"></div></div></div></div>
			<div class="crayon-info" style="min-height: 16.8px !important; line-height: 16.8px !important;"></div>
			<div class="crayon-plain-wrap"><textarea wrap="soft" class="crayon-plain print-no" data-settings="dblclick" readonly style="-moz-tab-size:4; -o-tab-size:4; -webkit-tab-size:4; tab-size:4; font-size: 12px !important; line-height: 15px !important;">
{
    "name": "Example",
    "webPrefix": "example.com",
    "nativePrefix": "custom:///",
    "transforms": [
        {
            "web": "search?find_doc={query}",
            "native": "search?terms={query}"
        }
    ]
}</textarea></div>
			<div class="crayon-main" style="">
				<table class="crayon-table">
					<tr class="crayon-row">
				<td class="crayon-nums " data-settings="hide">
					<div class="crayon-nums-content" style="font-size: 12px !important; line-height: 15px !important;"><div class="crayon-num" data-line="crayon-550a253e55089026389633-1">1</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55089026389633-2">2</div><div class="crayon-num" data-line="crayon-550a253e55089026389633-3">3</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55089026389633-4">4</div><div class="crayon-num" data-line="crayon-550a253e55089026389633-5">5</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55089026389633-6">6</div><div class="crayon-num" data-line="crayon-550a253e55089026389633-7">7</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55089026389633-8">8</div><div class="crayon-num" data-line="crayon-550a253e55089026389633-9">9</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55089026389633-10">10</div><div class="crayon-num" data-line="crayon-550a253e55089026389633-11">11</div></div>
				</td>
						<td class="crayon-code"><div class="crayon-pre" style="font-size: 12px !important; line-height: 15px !important;"><div class="crayon-line" id="crayon-550a253e55089026389633-1"><span class="crayon-sy">{</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55089026389633-2"><span class="crayon-h">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-s">"name"</span><span class="crayon-o">:</span><span class="crayon-h"> </span><span class="crayon-s">"Example"</span><span class="crayon-sy">,</span></div><div class="crayon-line" id="crayon-550a253e55089026389633-3"><span class="crayon-h">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-s">"webPrefix"</span><span class="crayon-o">:</span><span class="crayon-h"> </span><span class="crayon-s">"example.com"</span><span class="crayon-sy">,</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55089026389633-4"><span class="crayon-h">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-s">"nativePrefix"</span><span class="crayon-o">:</span><span class="crayon-h"> </span><span class="crayon-s">"custom:///"</span><span class="crayon-sy">,</span></div><div class="crayon-line" id="crayon-550a253e55089026389633-5"><span class="crayon-h">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-s">"transforms"</span><span class="crayon-o">:</span><span class="crayon-h"> </span><span class="crayon-sy">[</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55089026389633-6"><span class="crayon-h">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-sy">{</span></div><div class="crayon-line" id="crayon-550a253e55089026389633-7"><span class="crayon-h">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-s">"web"</span><span class="crayon-o">:</span><span class="crayon-h"> </span><span class="crayon-s">"search?find_doc={query}"</span><span class="crayon-sy">,</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55089026389633-8"><span class="crayon-h">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-s">"native"</span><span class="crayon-o">:</span><span class="crayon-h"> </span><span class="crayon-s">"search?terms={query}"</span></div><div class="crayon-line" id="crayon-550a253e55089026389633-9"><span class="crayon-h">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-sy">}</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55089026389633-10"><span class="crayon-h">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-sy">]</span></div><div class="crayon-line" id="crayon-550a253e55089026389633-11"><span class="crayon-sy">}</span></div></div></td>
					</tr>
				</table>
			</div>
		</div>
<!-- [Format Time: 0.0022 seconds] -->

详细信息请阅读：[http://appurl.org/](http://appurl.org/)

采用这两种标准的开发者，我们建议其使用 Microdata 对 Web 页面进行描述，这样可以帮助豌豆荚更好地检索和展现内容。由于 Microdata 可以直接使用  HTML 属性来标注，因此对于有 Web 站点的开发者，只需要在原有网页上进行少量修改就可以达到结构化数据标注的效果。

假设有一个电影网站，电影《环太平洋》详情页的部分 HTML 代码如下：
<!-- Crayon Syntax Highlighter v2.5.0 -->

		<div id="crayon-550a253e55092514209046" class="crayon-syntax crayon-theme-arduino-ide crayon-font-monaco crayon-os-pc print-yes notranslate" data-settings=" minimize scroll-mouseover" style=" margin-top: 12px; margin-bottom: 12px; float: none; clear: both; font-size: 12px !important; line-height: 15px !important;">

			<div class="crayon-toolbar" data-settings=" mouseover overlay hide delay" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><span class="crayon-title"></span>
			<div class="crayon-tools" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><div class="crayon-button crayon-nums-button" title="Toggle Line Numbers"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-plain-button" title="Toggle Plain Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-wrap-button" title="Toggle Line Wrap"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-expand-button" title="Expand Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-copy-button" title="Copy"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-popup-button" title="Open Code In New Window"><div class="crayon-button-icon"></div></div><span class="crayon-language">XHTML</span></div></div>
			<div class="crayon-info" style="min-height: 16.8px !important; line-height: 16.8px !important;"></div>
			<div class="crayon-plain-wrap"><textarea wrap="soft" class="crayon-plain print-no" data-settings="dblclick" readonly style="-moz-tab-size:4; -o-tab-size:4; -webkit-tab-size:4; tab-size:4; font-size: 12px !important; line-height: 15px !important;">
&lt;h1&gt;环太平洋&lt;/h1&gt;
&lt;div&gt;
有一个名叫"凯由"的滔天外来生物从海上崛起，并且引起一场战争，这场浩劫将威胁到数百万计的人类的生命和...
&lt;/div&gt;
&lt;div&gt;导演: 吉尔莫·德尔·托罗&lt;/div&gt;
&lt;div&gt;主演: 朗·普尔曼&lt;/div&gt;
&lt;div&gt;来自200个用户的评分: 8/10 总评论数: 50&lt;/div&gt;</textarea></div>
			<div class="crayon-main" style="">
				<table class="crayon-table">
					<tr class="crayon-row">
				<td class="crayon-nums " data-settings="hide">
					<div class="crayon-nums-content" style="font-size: 12px !important; line-height: 15px !important;"><div class="crayon-num" data-line="crayon-550a253e55092514209046-1">1</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55092514209046-2">2</div><div class="crayon-num" data-line="crayon-550a253e55092514209046-3">3</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55092514209046-4">4</div><div class="crayon-num" data-line="crayon-550a253e55092514209046-5">5</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55092514209046-6">6</div><div class="crayon-num" data-line="crayon-550a253e55092514209046-7">7</div></div>
				</td>
						<td class="crayon-code"><div class="crayon-pre" style="font-size: 12px !important; line-height: 15px !important;"><div class="crayon-line" id="crayon-550a253e55092514209046-1"><span class="crayon-r ">&lt;h1&gt;</span><span class="crayon-i ">环太平洋</span><span class="crayon-r ">&lt;/h1&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55092514209046-2"><span class="crayon-r ">&lt;div&gt;</span></div><div class="crayon-line" id="crayon-550a253e55092514209046-3"><span class="crayon-i ">有一个名叫"凯由"的滔天外来生物从海上崛起，并且引起一场战争，这场浩劫将威胁到数百万计的人类的生命和...</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55092514209046-4"><span class="crayon-r ">&lt;/div&gt;</span></div><div class="crayon-line" id="crayon-550a253e55092514209046-5"><span class="crayon-r ">&lt;div&gt;</span><span class="crayon-i ">导演: 吉尔莫·德尔·托罗</span><span class="crayon-r ">&lt;/div&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55092514209046-6"><span class="crayon-r ">&lt;div&gt;</span><span class="crayon-i ">主演: 朗·普尔曼</span><span class="crayon-r ">&lt;/div&gt;</span></div><div class="crayon-line" id="crayon-550a253e55092514209046-7"><span class="crayon-r ">&lt;div&gt;</span><span class="crayon-i ">来自200个用户的评分: 8/10 总评论数: 50</span><span class="crayon-r ">&lt;/div&gt;</span></div></div></td>
					</tr>
				</table>
			</div>
		</div>
<!-- [Format Time: 0.0011 seconds] -->

我们加入相关的 Microdata 标签来对这个电影进行描述：
<!-- Crayon Syntax Highlighter v2.5.0 -->

		<div id="crayon-550a253e55099304705834" class="crayon-syntax crayon-theme-arduino-ide crayon-font-monaco crayon-os-pc print-yes notranslate" data-settings=" minimize scroll-mouseover" style=" margin-top: 12px; margin-bottom: 12px; float: none; clear: both; font-size: 12px !important; line-height: 15px !important;">

			<div class="crayon-toolbar" data-settings=" mouseover overlay hide delay" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><span class="crayon-title"></span>
			<div class="crayon-tools" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><div class="crayon-button crayon-nums-button" title="Toggle Line Numbers"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-plain-button" title="Toggle Plain Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-wrap-button" title="Toggle Line Wrap"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-expand-button" title="Expand Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-copy-button" title="Copy"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-popup-button" title="Open Code In New Window"><div class="crayon-button-icon"></div></div><span class="crayon-language">XHTML</span></div></div>
			<div class="crayon-info" style="min-height: 16.8px !important; line-height: 16.8px !important;"></div>
			<div class="crayon-plain-wrap"><textarea wrap="soft" class="crayon-plain print-no" data-settings="dblclick" readonly style="-moz-tab-size:4; -o-tab-size:4; -webkit-tab-size:4; tab-size:4; font-size: 12px !important; line-height: 15px !important;">
&lt;div itemscope itemtype="http://schema.org/Movie"&gt;
  &lt;h1 itemprop="name"&gt;环太平洋&lt;/h1&gt;
  &lt;span itemprop="description"&gt;有一个名叫"凯由"的滔天外来生物从海上崛起，并且引起一场战争，这场浩劫将威胁到数百万计的人类的生命和...&lt;/span&gt;
  导演:
  &lt;div itemprop="director" itemscope itemtype="http://schema.org/Person"&gt;
    &lt;span itemprop="name"&gt;吉尔莫·德尔·托罗&lt;/span&gt;
  &lt;/div&gt;
  主演:
  &lt;div itemprop="actor" itemscope itemtype="http://schema.org/Person"&gt;
    &lt;span itemprop="name"&gt;朗·普尔曼&lt;/span&gt;
  &lt;/div&gt;
  &lt;div itemprop="aggregateRating" itemscope itemtype="http://schema.org/AggregateRating"&gt;
    来自&lt;span itemprop="ratingCount"&gt;200&lt;/span&gt; 个用户.
    的评分：&lt;span itemprop="ratingValue"&gt;8&lt;/span&gt;/&lt;span itemprop="bestRating"&gt;10&lt;/span&gt;
    总评论数: &lt;span itemprop="reviewCount"&gt;50&lt;/span&gt;.
  &lt;/div&gt;
&lt;/div&gt;</textarea></div>
			<div class="crayon-main" style="">
				<table class="crayon-table">
					<tr class="crayon-row">
				<td class="crayon-nums " data-settings="hide">
					<div class="crayon-nums-content" style="font-size: 12px !important; line-height: 15px !important;"><div class="crayon-num" data-line="crayon-550a253e55099304705834-1">1</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55099304705834-2">2</div><div class="crayon-num" data-line="crayon-550a253e55099304705834-3">3</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55099304705834-4">4</div><div class="crayon-num" data-line="crayon-550a253e55099304705834-5">5</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55099304705834-6">6</div><div class="crayon-num" data-line="crayon-550a253e55099304705834-7">7</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55099304705834-8">8</div><div class="crayon-num" data-line="crayon-550a253e55099304705834-9">9</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55099304705834-10">10</div><div class="crayon-num" data-line="crayon-550a253e55099304705834-11">11</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55099304705834-12">12</div><div class="crayon-num" data-line="crayon-550a253e55099304705834-13">13</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55099304705834-14">14</div><div class="crayon-num" data-line="crayon-550a253e55099304705834-15">15</div><div class="crayon-num crayon-striped-num" data-line="crayon-550a253e55099304705834-16">16</div><div class="crayon-num" data-line="crayon-550a253e55099304705834-17">17</div></div>
				</td>
						<td class="crayon-code"><div class="crayon-pre" style="font-size: 12px !important; line-height: 15px !important;"><div class="crayon-line" id="crayon-550a253e55099304705834-1"><span class="crayon-r ">&lt;div </span>itemscope<span class="crayon-h"> </span><span class="crayon-e ">itemtype</span><span class="crayon-o">=</span><span class="crayon-s ">"http://schema.org/Movie"</span><span class="crayon-r ">&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55099304705834-2"><span class="crayon-i ">&nbsp;&nbsp;</span><span class="crayon-r ">&lt;h1 </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"name"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">环太平洋</span><span class="crayon-r ">&lt;/h1&gt;</span></div><div class="crayon-line" id="crayon-550a253e55099304705834-3"><span class="crayon-i ">&nbsp;&nbsp;</span><span class="crayon-r ">&lt;span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"description"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">有一个名叫"凯由"的滔天外来生物从海上崛起，并且引起一场战争，这场浩劫将威胁到数百万计的人类的生命和...</span><span class="crayon-r ">&lt;/span&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55099304705834-4"><span class="crayon-i ">&nbsp;&nbsp;导演:</span></div><div class="crayon-line" id="crayon-550a253e55099304705834-5"><span class="crayon-i ">&nbsp;&nbsp;</span><span class="crayon-r ">&lt;div </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"director"</span><span class="crayon-h"> </span>itemscope<span class="crayon-h"> </span><span class="crayon-e ">itemtype</span><span class="crayon-o">=</span><span class="crayon-s ">"http://schema.org/Person"</span><span class="crayon-r ">&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55099304705834-6"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"name"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">吉尔莫·德尔·托罗</span><span class="crayon-r ">&lt;/span&gt;</span></div><div class="crayon-line" id="crayon-550a253e55099304705834-7"><span class="crayon-i ">&nbsp;&nbsp;</span><span class="crayon-r ">&lt;/div&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55099304705834-8"><span class="crayon-i ">&nbsp;&nbsp;主演:</span></div><div class="crayon-line" id="crayon-550a253e55099304705834-9"><span class="crayon-i ">&nbsp;&nbsp;</span><span class="crayon-r ">&lt;div </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"actor"</span><span class="crayon-h"> </span>itemscope<span class="crayon-h"> </span><span class="crayon-e ">itemtype</span><span class="crayon-o">=</span><span class="crayon-s ">"http://schema.org/Person"</span><span class="crayon-r ">&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55099304705834-10"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="crayon-r ">&lt;span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"name"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">朗·普尔曼</span><span class="crayon-r ">&lt;/span&gt;</span></div><div class="crayon-line" id="crayon-550a253e55099304705834-11"><span class="crayon-i ">&nbsp;&nbsp;</span><span class="crayon-r ">&lt;/div&gt;</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55099304705834-12"><span class="crayon-i ">&nbsp;&nbsp;</span><span class="crayon-r ">&lt;div </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"aggregateRating"</span><span class="crayon-h"> </span>itemscope<span class="crayon-h"> </span><span class="crayon-e ">itemtype</span><span class="crayon-o">=</span><span class="crayon-s ">"http://schema.org/AggregateRating"</span><span class="crayon-r ">&gt;</span></div><div class="crayon-line" id="crayon-550a253e55099304705834-13"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;来自</span><span class="crayon-r ">&lt;span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"ratingCount"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">200</span><span class="crayon-r ">&lt;/span&gt;</span><span class="crayon-i "> 个用户.</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55099304705834-14"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;的评分：</span><span class="crayon-r ">&lt;span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"ratingValue"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">8</span><span class="crayon-r ">&lt;/span&gt;</span><span class="crayon-i ">/</span><span class="crayon-r ">&lt;span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"bestRating"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">10</span><span class="crayon-r ">&lt;/span&gt;</span></div><div class="crayon-line" id="crayon-550a253e55099304705834-15"><span class="crayon-i ">&nbsp;&nbsp;&nbsp;&nbsp;总评论数: </span><span class="crayon-r ">&lt;span </span><span class="crayon-e ">itemprop</span><span class="crayon-o">=</span><span class="crayon-s ">"reviewCount"</span><span class="crayon-r ">&gt;</span><span class="crayon-i ">50</span><span class="crayon-r ">&lt;/span&gt;</span><span class="crayon-i ">.</span></div><div class="crayon-line crayon-striped-line" id="crayon-550a253e55099304705834-16"><span class="crayon-i ">&nbsp;&nbsp;</span><span class="crayon-r ">&lt;/div&gt;</span></div><div class="crayon-line" id="crayon-550a253e55099304705834-17"><span class="crayon-r ">&lt;/div&gt;</span></div></div></td>
					</tr>
				</table>
			</div>
		</div>
<!-- [Format Time: 0.0049 seconds] -->

这样只要稍作修改，就可以在同样的 Web 页面提供结构化的信息，完成了对这个电影 Item 的描述。从而帮助豌豆荚更好地检索和展现内容。