[原网站](http://developer.wandoujia.com/search/items/)

### 数据标准说明

[电子书](#Book)

[电影](#Movie)

[主题](#Theme)

[新闻](#News)

[团购](#GroupPurchase)

[专题](#Subject)

[问答](#QuestionAndAnswer)

[音乐](#Music)

[商家](#Business)

[电视剧](#VideoTV)

[电影票](#MovieTicket)

[漫画](#Cartoon)

[图片](#ImageObject)

[内容评论](#Commentary)

[文库](#Library)

[彩票](#Lottery)

[公开课](#OpenClass)

[游戏攻略](#GameGuide)

[旅行攻略](#TravelTips)

[购物](#Shopping)

[有声读物](#AudioBook)

[旅行折扣](#TravleDiscount)

[百科](#Encyclopedia)

[健康资讯](#HealthInfo)

[票务](#Ticketing)

[应用](#App)

[动画](#Animation)

[短视频](#ShortVideo)

[综艺](#Variety)

[天气](#weatherInfo)

[人物](#Personage)

### 基本数据类型

[Text](#Text)

[URL](#URL)

[Number](#Number)

[Date](#Date)

[Enum](#Enum)

[Integer](#Integer)

[Boolean](#Boolean)

[Duration](#Duration)

[Float](#Float)

### 通用数据类型

[Image](#Image)

[AggregateRating](#AggregateRating)

[Person](#Person)

[评论信息](#UserComments)

[Place](#Place)

[个体](#Entity)

[InteractionCount](#InteractionCount)

[Tag](#Tag)

[Offer](#Offer)

[Organization](#Organization)

[Chapter](#Chapter)

[BookFormatType](#BookFormatType)

[VideoObject](#VideoObject)

[视频下载信息](#DownloadInfo)

[TVEpisode](#TVEpisode)

[Shop](#Shop)

[问题](#Question)

[答案](#Answer)

[Author](#Author)

[MusicGroup](#MusicGroup)

[AudioObject](#AudioObject)

[TVSeason](#TVSeason)

[Cinema](#Cinema)

[Show](#Show)

[回复](#Reply)

[奖项列表](#rewardList)

[章节](#Section)

[AudioEpisode](#AudioEpisode)

[表格](#BasicInfo)

[Venue](#Venue)

[Performance](#Performance)

[AnimationEpisode](#AnimationEpisode)

[周际预报](#weekForecast)

[精确日报（分小时数据）](#hourlyForecast)

[空气质量](#airQuality)

[生活指数](#livingIndex)

[灾害天气预警信息](#warningInfo)

[天气预报](#Forecast)

[命名实体](#namedEntity)

# <a name="Book"></a>**电子书(Book)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 名称</td>
</tr>

<tr><td >alternativeHeadline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 别名</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > Y</td>
<td > 截图</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页的 AppURL</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 描述</td>
</tr>

<tr><td >aggregateRating</td>
<td > [AggregateRating](#AggregateRating)</td>
<td > </td>
<td > </td>
<td > 评分信息</td>
</tr>

<tr><td >author</td>
<td > [Person](#Person)</td>
<td > Y</td>
<td > </td>
<td > 作者</td>
</tr>

<tr><td >comment</td>
<td > [UserComments](#UserComments)</td>
<td > </td>
<td > Y</td>
<td > 用户评论</td>
</tr>

<tr><td >contentLocation</td>
<td > [Place](#Place)</td>
<td > </td>
<td > </td>
<td > 地域/国别</td>
</tr>

<tr><td >contentRating</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 官方分级</td>
</tr>

<tr><td >copyrightHolder</td>
<td > [Entity](#Entity)</td>
<td > </td>
<td > </td>
<td > 版权方</td>
</tr>

<tr><td >copyrightYear</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 内容版权生效年份</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 创建日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 最近更新日期</td>
</tr>

<tr><td >datePublished</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 出版日期</td>
</tr>

<tr><td >commentUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 评论页的 WebURL</td>
</tr>

<tr><td >commentAppUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 评论页的 AppURL</td>
</tr>

<tr><td >editor</td>
<td > [Person](#Person)</td>
<td > </td>
<td > </td>
<td > 编辑</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 类型</td>
</tr>

<tr><td >headline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 标题，同 name</td>
</tr>

<tr><td >inLanguage</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 语言(中文/英文等)</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 用户对电子书的操作次数</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > </td>
<td > 描述内容的关键词/标签</td>
</tr>

<tr><td >offer</td>
<td > [Offer](#Offer)</td>
<td > </td>
<td > </td>
<td > 为该电子书提供的优惠，例如“豌豆荚用户可8折购买”</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 内容提供方</td>
</tr>

<tr><td >publisher</td>
<td > [Organization](#Organization)</td>
<td > </td>
<td > </td>
<td > 出版方</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > </td>
<td > </td>
<td > item 内容的状态（主要用来标记该内容是否下线）(**取值范围:new;updated;offline** )</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 封面缩略图</td>
</tr>

<tr><td >catalogueUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 目录页网页 URL</td>
</tr>

<tr><td >chapter</td>
<td > [Chapter](#Chapter)</td>
<td > </td>
<td > </td>
<td > 章节内容信息</td>
</tr>

<tr><td >bookEdition</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 版本</td>
</tr>

<tr><td >bookFormat</td>
<td > [BookFormatType](#BookFormatType)</td>
<td > </td>
<td > </td>
<td > 电子书文件格式</td>
</tr>

<tr><td >isbn</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > ISBN 号</td>
</tr>

<tr><td >numberOfPages</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 页数(传统出版物)/章节数(网络小说)</td>
</tr>

<tr><td >numberOfWords</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 字数</td>
</tr>

<tr><td >accountablePerson</td>
<td > [Person](#Person)</td>
<td > </td>
<td > </td>
<td > 责任编辑</td>
</tr>

<tr><td >translator</td>
<td > [Person](#Person)</td>
<td > </td>
<td > </td>
<td > 译者</td>
</tr>

<tr><td >isFinished</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否完结</td>
</tr>

<tr><td >price</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 电子书的价格</td>
</tr>

<tr><td >video</td>
<td > [VideoObject](#VideoObject)</td>
<td > </td>
<td > </td>
<td > 相关视频的信息</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 封面图片</td>
</tr>
</tbody></table>

# <a name="Movie"></a>**电影(Movie)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 名称</td>
</tr>

<tr><td >alternativeHeadline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 别名</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 描述</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 剧照图片</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页的 AppURL</td>
</tr>

<tr><td >aggregateRating</td>
<td > [AggregateRating](#AggregateRating)</td>
<td > </td>
<td > </td>
<td > 评分信息</td>
</tr>

<tr><td >author</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 原著作者</td>
</tr>

<tr><td >comment</td>
<td > [UserComments](#UserComments)</td>
<td > </td>
<td > Y</td>
<td > 用户评论</td>
</tr>

<tr><td >contentLocation</td>
<td > [Place](#Place)</td>
<td > </td>
<td > Y</td>
<td > 电影地域/国别</td>
</tr>

<tr><td >contentRating</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 电影内容的官方分级</td>
</tr>

<tr><td >copyrightHolder</td>
<td > [Entity](#Entity)</td>
<td > </td>
<td > </td>
<td > 电影版权方</td>
</tr>

<tr><td >copyrightYear</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 电影内容版权生效年份</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 创建日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 最近更新日期</td>
</tr>

<tr><td >datePublished</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 首次发布日期</td>
</tr>

<tr><td >commentUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 评论页的 WebURL</td>
</tr>

<tr><td >commentAppUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 评论页的 AppURL</td>
</tr>

<tr><td >editor</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 编剧</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 类型</td>
</tr>

<tr><td >headline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 标题，同 name</td>
</tr>

<tr><td >inLanguage</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 语言(粤语/英语等)</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 用户对电影的操作次数</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 用来描述电影内容的关键词/标签</td>
</tr>

<tr><td >offer</td>
<td > [Offer](#Offer)</td>
<td > </td>
<td > </td>
<td > 为该电影提供的优惠，例如“豌豆荚用户可免费下载到手机”</td>
</tr>

<tr><td >publisher</td>
<td > [Organization](#Organization)</td>
<td > </td>
<td > </td>
<td > 电影出版方</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > </td>
<td > </td>
<td > item 内容的状态（主要用来标记该内容是否下线）(**取值范围:new;updated;offline** )</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > Y</td>
<td > 封面图片</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 封面图片缩略图</td>
</tr>

<tr><td >actor</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 演员</td>
</tr>

<tr><td >director</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 导演</td>
</tr>

<tr><td >duration</td>
<td > [Duration](#Duration)</td>
<td > </td>
<td > </td>
<td > 时长</td>
</tr>

<tr><td >producer</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 制片人</td>
</tr>

<tr><td >producerCompany</td>
<td > [Organization](#Organization)</td>
<td > </td>
<td > </td>
<td > 制片公司</td>
</tr>

<tr><td >award</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 影片获奖情况</td>
</tr>

<tr><td >trailer</td>
<td > [VideoObject](#VideoObject)</td>
<td > </td>
<td > Y</td>
<td > 预告片</td>
</tr>

<tr><td >videoEpisode</td>
<td > [TVEpisode](#TVEpisode)</td>
<td > Y</td>
<td > Y</td>
<td > 电影具体的视频信息</td>
</tr>

<tr><td >role</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 电影角色</td>
</tr>

<tr><td >packageName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > Y</td>
<td > 包名</td>
</tr>

<tr><td >minVersionCode</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 用于调起时的判断逻辑</td>
</tr>

<tr><td >sourceName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 来自什么应用</td>
<td >用于ranking和呈现等多个逻辑</td>
</tr>
</tbody></table>

# <a name="Theme"></a>**主题(Theme)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 主题名称</td>
</tr>

<tr><td >designer</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 设计师</td>
</tr>

<tr><td >author</td>
<td > [Person](#Person)</td>
<td > </td>
<td > </td>
<td > 制作者/作者</td>
</tr>

<tr><td >version</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 版本号</td>
</tr>

<tr><td >size</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 大小，单位为 KB</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 更新日期</td>
</tr>

<tr><td >module</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 包含模块的个数</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 封面图片缩略图</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 截图</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 描述</td>
</tr>

<tr><td >aggregateRating</td>
<td > [AggregateRating](#AggregateRating)</td>
<td > </td>
<td > </td>
<td > 评分信息</td>
</tr>

<tr><td >price</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 价格，如果免费，请填写「免费」；否则请填写「5.0 **币」等</td>
</tr>

<tr><td >apk</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 主题包的 url</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 类型</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 关键词/标签</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 主题的提供方</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > </td>
<td > </td>
<td > 主题的状态（主要用来标记该内容是否下线）(**取值范围:new;updated;offline** )</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 封面图片</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 用户对主题的操作次数</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 主题详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 主题详情页的 AppURL</td>
</tr>

<tr><td >packageName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > Y</td>
<td > 包名</td>
</tr>

<tr><td >minVersionCode</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 用于调起时的判断逻辑</td>
</tr>

<tr><td >sourceName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 来自什么应用，用于ranking和呈现等多个逻辑</td>
</tr>
</tbody></table>

# <a name="News"></a>**新闻(News)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 新闻标题</td>
</tr>

<tr><td >alternativeHeadline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 别名</td>
</tr>

<tr><td >digest</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 新闻摘要</td>
</tr>

<tr><td >body</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 新闻内容</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 封面图片缩略图</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 新闻图片</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 新闻的 WebURL</td>
</tr>

<tr><td >aggregateRating</td>
<td > [AggregateRating](#AggregateRating)</td>
<td > </td>
<td > </td>
<td > 评分信息</td>
</tr>

<tr><td >author</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 作者</td>
</tr>

<tr><td >datePublished</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 发布日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 最近更新日期</td>
</tr>

<tr><td >editor</td>
<td > [Person](#Person)</td>
<td > </td>
<td > </td>
<td > 编辑</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 所属栏目</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 描述新闻的关键词/标签</td>
</tr>

<tr><td >inLanguage</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 语言(中文/英文等)</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 内容提供方，如「网易新闻」</td>
</tr>

<tr><td >publisher</td>
<td > [Organization](#Organization)</td>
<td > </td>
<td > </td>
<td > 新闻来源</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > </td>
<td > </td>
<td > 新闻的状态（主要用来标记该内容是否下线）(**取值范围:new;updated;offline** )</td>
</tr>

<tr><td >video</td>
<td > [VideoObject](#VideoObject)</td>
<td > </td>
<td > Y</td>
<td > 新闻相关视频的信息</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 新闻的 AppURL</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 用户对新闻的操作次数</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 封面图片</td>
</tr>
</tbody></table>

# <a name="GroupPurchase"></a>**团购(GroupPurchase)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 团购标题</td>
</tr>

<tr><td >shortName</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 团购短标题</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 团购详情页的 WebURL</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > Y</td>
<td > 团购图片</td>
</tr>

<tr><td >city</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 城市名称。城市名称不需要附带省、市、区、县等字，如果是全国范围请指明：全国，并且在title 中加入「全国」二字</td>
</tr>

<tr><td >businessDistrict</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 所属商圈</td>
</tr>

<tr><td >destination</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 酒店旅游类团购的目的名称。如果是境内旅游，destination 填写城市名称或景点名称，城市名称不需要附带省、市、区、县等字，例如：北京；如果是境外旅游，destination 填写国家名称或景点名称，例如：夏威夷。</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 内容提供方，也就是站点名称</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 关键词/标签</td>
</tr>

<tr><td >startTime</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 团购开始时间，例如：2014-04-01 00:00:00</td>
</tr>

<tr><td >endTime</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 团购结束时间，例如：2014-04-02 00:00:00</td>
</tr>

<tr><td >value</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 商品原价</td>
</tr>

<tr><td >price</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 商品现价</td>
</tr>

<tr><td >rebate</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 商品折扣</td>
</tr>

<tr><td >boughtCount</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 已购买人数</td>
</tr>

<tr><td >maxCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 最多购买人数</td>
</tr>

<tr><td >minCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 最少购买人数，有多少人参加团购才会成功的人数</td>
</tr>

<tr><td >inventoryCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 库存</td>
</tr>

<tr><td >restrictedCondition</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 限制条件</td>
</tr>

<tr><td >onSaleStatus</td>
<td > [Boolean](#Boolean)</td>
<td > Y</td>
<td > </td>
<td > 是否上架</td>
</tr>

<tr><td >post</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否为邮寄</td>
</tr>

<tr><td >soldOut</td>
<td > [Boolean](#Boolean)</td>
<td > Y</td>
<td > </td>
<td > 是否已卖光</td>
</tr>

<tr><td >appointment</td>
<td > [Enum](#Enum)</td>
<td > </td>
<td > </td>
<td > 可选值 unknown/need/no。unknown: 未知，need: 需要预约，no: 不需要预约(**取值范围:need;no;unknown** )</td>
</tr>

<tr><td >textDescription</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 对团购详情的文本描述</td>
</tr>

<tr><td >richDescription</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 对团购详情的富文本描述，可以带图片和 html 等</td>
</tr>

<tr><td >tips</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 重要提示信息</td>
</tr>

<tr><td >hotLevel</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 热门程度，取值1-5。数值越大越热门</td>
</tr>

<tr><td >shop</td>
<td > [Shop](#Shop)</td>
<td > Y</td>
<td > Y</td>
<td > 商家信息</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 团购详情页的 AppURL</td>
</tr>
</tbody></table>

# <a name="Subject"></a>**专题(Subject)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 专题名称</td>
</tr>

<tr><td >datePublished</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 发布日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 更新日期</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 封面图片缩略图</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 图片</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 描述</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 所属栏目</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 关键词/标签</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 专题的提供方</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > </td>
<td > Y</td>
<td > 专题的状态（主要用来标记该内容是否下线）(**取值范围:new;updated;offline** )</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 封面图片</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 专题的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 专题的 AppURL</td>
</tr>
</tbody></table>

# <a name="QuestionAndAnswer"></a>**问答(QuestionAndAnswer)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >question</td>
<td > [Question](#Question)</td>
<td > Y</td>
<td > </td>
<td > 问题</td>
</tr>

<tr><td >answer</td>
<td > [Answer](#Answer)</td>
<td > Y</td>
<td > Y</td>
<td > 回答</td>
</tr>
</tbody></table>

# <a name="Music"></a>**音乐(Music)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 名称</td>
</tr>

<tr><td >alternativeHeadline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 别名</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 描述</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页的 AppURL</td>
</tr>

<tr><td >aggregateRating</td>
<td > [AggregateRating](#AggregateRating)</td>
<td > </td>
<td > </td>
<td > 评分信息</td>
</tr>

<tr><td >comment</td>
<td > [UserComments](#UserComments)</td>
<td > </td>
<td > Y</td>
<td > 用户评论</td>
</tr>

<tr><td >contentLocation</td>
<td > [Place](#Place)</td>
<td > </td>
<td > </td>
<td > 地域/国别</td>
</tr>

<tr><td >copyrightHolder</td>
<td > [Entity](#Entity)</td>
<td > </td>
<td > </td>
<td > 版权方</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 创建日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 最近更新日期</td>
</tr>

<tr><td >datePublished</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 发行日期</td>
</tr>

<tr><td >commentUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 评论页的 WebURL</td>
</tr>

<tr><td >commentAppUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 评论页的 AppURL</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 流派/风格</td>
</tr>

<tr><td >inLanguage</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 语言(英语/法语)</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 用户对音乐的操作次数</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 描述音乐的关键词/标签</td>
</tr>

<tr><td >offer</td>
<td > [Offer](#Offer)</td>
<td > </td>
<td > </td>
<td > 为该音乐提供的优惠，例如“豌豆荚用户可免费下载HQ(高品质)音乐和SQ(超品质)音乐到手机”</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 音乐提供方</td>
</tr>

<tr><td >publisher</td>
<td > [Organization](#Organization)</td>
<td > </td>
<td > </td>
<td > 音乐出版方</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > </td>
<td > </td>
<td > item内容的状态（主要用来标记该内容是否下线）(**取值范围:new;updated;offline** )</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 封面缩略图</td>
</tr>

<tr><td >byArtist</td>
<td > [MusicGroup](#MusicGroup)</td>
<td > Y</td>
<td > Y</td>
<td > 歌手/组合</td>
</tr>

<tr><td >accountablePerson</td>
<td > [Person](#Person)</td>
<td > </td>
<td > </td>
<td > 责任人</td>
</tr>

<tr><td >audio</td>
<td > [AudioObject](#AudioObject)</td>
<td > Y</td>
<td > </td>
<td > 音频文件的信息</td>
</tr>

<tr><td >award</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 获奖情况</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 封面图片</td>
</tr>

<tr><td >medium</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 介质（如CD）</td>
</tr>

<tr><td >isrc</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > ISRC</td>
</tr>

<tr><td >upc</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 通用产品代码/条形码/UPC</td>
</tr>

<tr><td >numberOfRecord</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 唱片数</td>
</tr>

<tr><td >typeOfAlbum</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 专辑类型/类别（如EP）</td>
</tr>

<tr><td >tracks</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 曲目</td>
</tr>
</tbody></table>

# <a name="Business"></a>**商家(Business)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 商家名称</td>
</tr>

<tr><td >brand</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 品牌名称</td>
</tr>

<tr><td >branchName</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 分店名称</td>
</tr>

<tr><td >telephone</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 联系电话</td>
</tr>

<tr><td >city</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 商家所在城市（若无特定城市则填写“全国”）</td>
</tr>

<tr><td >address</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 地址信息</td>
</tr>

<tr><td >area</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 商圈</td>
</tr>

<tr><td >openTime</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 商铺营业时间</td>
</tr>

<tr><td >longitude</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 经度</td>
</tr>

<tr><td >latitude</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 纬度</td>
</tr>

<tr><td >trafficInfo</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 交通信息</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 分类/标签</td>
</tr>

<tr><td >aggregateRating</td>
<td > [AggregateRating](#AggregateRating)</td>
<td > </td>
<td > </td>
<td > 评分信息</td>
</tr>

<tr><td >productGrade</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 产品/食品口味评价，1：一般，2：尚可，3：好，4：很好，5：非常好</td>
</tr>

<tr><td >decorationGrade</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 环境评价，1：一般，2：尚可，3：好，4：很好，5：非常好</td>
</tr>

<tr><td >serviceGrade</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 服务评价，1：一般，2：尚可，3：好，4：很好，5：非常好</td>
</tr>

<tr><td >productScore</td>
<td > [Float](#Float)</td>
<td > Y</td>
<td > </td>
<td > 产品/食品口味评价单项分，精确到小数点后一位（十分制）</td>
</tr>

<tr><td >decorationScore</td>
<td > [Float](#Float)</td>
<td > Y</td>
<td > </td>
<td > 环境评价单项分，精确到小数点后一位（十分制）</td>
</tr>

<tr><td >serviceScore</td>
<td > [Float](#Float)</td>
<td > Y</td>
<td > </td>
<td > 服务评价单项分，精确到小数点后一位（十分制）</td>
</tr>

<tr><td >avgPrice</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 人均价格，单位:元</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页的 AppURL</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > Y</td>
<td > 图片</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 封面图片</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 封面缩略图</td>
</tr>

<tr><td >hasCoupon</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否有优惠券</td>
</tr>

<tr><td >hasDeal</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否有团购</td>
</tr>

<tr><td >hasCard</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否有会员卡</td>
</tr>

<tr><td >onlineReserved</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否可以在线预订</td>
</tr>
</tbody></table>

# <a name="VideoTV"></a>**电视剧(VideoTV)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 名称</td>
</tr>

<tr><td >alternativeHeadline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 别名</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 描述</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 剧照图片</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页的 AppURL</td>
</tr>

<tr><td >aggregateRating</td>
<td > [AggregateRating](#AggregateRating)</td>
<td > </td>
<td > </td>
<td > 评分信息</td>
</tr>

<tr><td >author</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 原著作者</td>
</tr>

<tr><td >comment</td>
<td > [UserComments](#UserComments)</td>
<td > </td>
<td > Y</td>
<td > 用户评论</td>
</tr>

<tr><td >contentLocation</td>
<td > [Place](#Place)</td>
<td > </td>
<td > Y</td>
<td > 地域/国别</td>
</tr>

<tr><td >contentRating</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 官方分级</td>
</tr>

<tr><td >copyrightHolder</td>
<td > [Entity](#Entity)</td>
<td > </td>
<td > </td>
<td > 版权方</td>
</tr>

<tr><td >copyrightYear</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 内容版权生效年份</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 创建日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 最近更新日期</td>
</tr>

<tr><td >datePublished</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 首次发布日期</td>
</tr>

<tr><td >commentUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 评论页的 WebURL</td>
</tr>

<tr><td >commentAppUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 评论页的 AppURL</td>
</tr>

<tr><td >editor</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 编剧</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 类型，二级分类</td>
</tr>

<tr><td >headline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 标题，同 name</td>
</tr>

<tr><td >inLanguage</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 语言(粤语/英语等)</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 用户对电视剧的操作次数</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 用来描述内容的关键词/标签</td>
</tr>

<tr><td >offer</td>
<td > [Offer](#Offer)</td>
<td > </td>
<td > </td>
<td > 为该内容提供的优惠，例如“豌豆荚用户可免费下载到手机”</td>
</tr>

<tr><td >publisher</td>
<td > [Organization](#Organization)</td>
<td > </td>
<td > </td>
<td > 出版方</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > Y</td>
<td > </td>
<td > item 内容的状态（主要用来标记该内容是否下线）(**取值范围:new;updated;offline** )</td>
</tr>

<tr><td >actor</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 演员</td>
</tr>

<tr><td >director</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 导演</td>
</tr>

<tr><td >startDate</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 播出开始日期</td>
</tr>

<tr><td >endDate</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 播出结束日期</td>
</tr>

<tr><td >videoEpisode</td>
<td > [TVEpisode](#TVEpisode)</td>
<td > Y</td>
<td > Y</td>
<td > 分集信息</td>
</tr>

<tr><td >numberOfEpisodes</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 总集数</td>
</tr>

<tr><td >lastEpisodeNumber</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 最新集</td>
</tr>

<tr><td >lastEpisodeDate</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 最新集的更新时间</td>
</tr>

<tr><td >producer</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 出品人</td>
</tr>

<tr><td >producerCompany</td>
<td > [Organization](#Organization)</td>
<td > </td>
<td > </td>
<td > 出品公司/电视台</td>
</tr>

<tr><td >season</td>
<td > [TVSeason](#TVSeason)</td>
<td > </td>
<td > </td>
<td > 季的信息，如果有多季的话</td>
</tr>

<tr><td >trailer</td>
<td > [VideoObject](#VideoObject)</td>
<td > </td>
<td > Y</td>
<td > 预告片</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > Y</td>
<td > 封面图片</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 封面图片缩略图</td>
</tr>

<tr><td >award</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 获奖情况</td>
</tr>

<tr><td >role</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 电视角色</td>
</tr>

<tr><td >packageName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > Y</td>
<td > 包名</td>
</tr>

<tr><td >minVersionCode</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 用于调起时的判断逻辑</td>
</tr>

<tr><td >sourceName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 来自什么应用</td>
<td >用于ranking和呈现等多个逻辑</td>
</tr>
</tbody></table>

# <a name="MovieTicket"></a>**电影票(MovieTicket)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 电影名称</td>
</tr>

<tr><td >alternativeHeadline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 别名</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 描述</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 封面图片</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 封面缩略图</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > Y</td>
<td > 剧照图片</td>
</tr>

<tr><td >trailer</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 预告片的 WebURL</td>
</tr>

<tr><td >datePublished</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 上映日期</td>
</tr>

<tr><td >actor</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 演员</td>
</tr>

<tr><td >director</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 导演</td>
</tr>

<tr><td >duration</td>
<td > [Duration](#Duration)</td>
<td > </td>
<td > </td>
<td > 时长</td>
</tr>

<tr><td >contentLocation</td>
<td > [Place](#Place)</td>
<td > </td>
<td > Y</td>
<td > 电影地域/国别</td>
</tr>

<tr><td >inLanguage</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 语言(粤语/英语等)</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 类型</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 用来描述内容的关键词/标签</td>
</tr>

<tr><td >briefComment</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 短评</td>
</tr>

<tr><td >version</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 版本（2D/3D）</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 影片详情页 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 影片详情页 AppURL</td>
</tr>

<tr><td >onSaleStatus</td>
<td > [Boolean](#Boolean)</td>
<td > Y</td>
<td > </td>
<td > 是否上架</td>
</tr>

<tr><td >cinemaCount</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 上映影院数目</td>
</tr>

<tr><td >showCount</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 上映场数</td>
</tr>

<tr><td >wishCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 想看人数</td>
</tr>

<tr><td >boughtCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 购票人数</td>
</tr>

<tr><td >preSale</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否预售</td>
</tr>

<tr><td >aggregateRating</td>
<td > [AggregateRating](#AggregateRating)</td>
<td > </td>
<td > </td>
<td > 评分信息</td>
</tr>

<tr><td >hotLevel</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 热门程度，取值1-5。数值越大越热门</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 内容提供方</td>
</tr>

<tr><td >cinema</td>
<td > [Cinema](#Cinema)</td>
<td > </td>
<td > Y</td>
<td > 上映影院的信息</td>
</tr>

<tr><td >packageName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > Y</td>
<td > 包名</td>
</tr>

<tr><td >minVersionCode</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 用于调起时的判断逻辑</td>
</tr>

<tr><td >sourceName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 来自什么应用，用于ranking和呈现等多个逻辑</td>
</tr>
</tbody></table>

# <a name="Cartoon"></a>**漫画(Cartoon)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 漫画名</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 封面图片</td>
</tr>

<tr><td >author</td>
<td > [Author](#Author)</td>
<td > Y</td>
<td > </td>
<td > 作者</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 简介和说明</td>
</tr>

<tr><td >serializeStatus</td>
<td > [Enum](#Enum)</td>
<td > Y</td>
<td > </td>
<td > 连载状态(**取值范围:FINISH;NOT_FINISH** )</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 类别信息/关键词</td>
</tr>

<tr><td >contentLocation</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 地区（国家和地区:日本，香港，中国）</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 最后一次更新时间</td>
</tr>

<tr><td >price</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 价格: e.g. 3元/3xx币</td>
</tr>

<tr><td >aggregateRating</td>
<td > [AggregateRating](#AggregateRating)</td>
<td > </td>
<td > </td>
<td > 评论/评分相关信息</td>
</tr>

<tr><td >lastChapter</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 最新章节</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 用户行为的统计计数</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 创建的时间</td>
</tr>

<tr><td >chapterCount</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 总章节数</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > </td>
<td > </td>
<td > 状态信息(**取值范围:new;updated;offline** )</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页的 AppURL</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 内容图片，展示用</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 封面图片缩略图</td>
</tr>

<tr><td >packageName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > Y</td>
<td > 包名</td>
</tr>

<tr><td >minVersionCode</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 用于调起时的判断逻辑</td>
</tr>

<tr><td >provider</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 来自什么应用，用于ranking和呈现等多个逻辑</td>
</tr>
</tbody></table>

# <a name="ImageObject"></a>**图片(ImageObject)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 名称</td>
</tr>

<tr><td >alternativeHeadline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 别名</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 描述</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 图片</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页的 AppURL</td>
</tr>

<tr><td >aggregateRating</td>
<td > [AggregateRating](#AggregateRating)</td>
<td > </td>
<td > </td>
<td > 评分信息</td>
</tr>

<tr><td >author</td>
<td > [Person](#Person)</td>
<td > </td>
<td > </td>
<td > 作者</td>
</tr>

<tr><td >comment</td>
<td > [UserComments](#UserComments)</td>
<td > </td>
<td > Y</td>
<td > 用户评论</td>
</tr>

<tr><td >contentLocation</td>
<td > [Place](#Place)</td>
<td > </td>
<td > </td>
<td > 地域/国别</td>
</tr>

<tr><td >copyrightHolder</td>
<td > [Entity](#Entity)</td>
<td > </td>
<td > </td>
<td > 版权方</td>
</tr>

<tr><td >copyrightYear</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 内容版权生效年份</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 创建日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 最近更新日期</td>
</tr>

<tr><td >datePublished</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 出版日期</td>
</tr>

<tr><td >commentUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 用户评论的 WebURL</td>
</tr>

<tr><td >commentAppUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 用户评论的 AppURL</td>
</tr>

<tr><td >editor</td>
<td > [Person](#Person)</td>
<td > </td>
<td > </td>
<td > 编辑</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 类型</td>
</tr>

<tr><td >headline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 标题，同 caption</td>
</tr>

<tr><td >inLanguage</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 语言(英语/法语)</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 用户对图片的操作次数</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 描述图片的关键词/标签</td>
</tr>

<tr><td >offer</td>
<td > [Offer](#Offer)</td>
<td > </td>
<td > </td>
<td > 为该图片提供的优惠，例如“豌豆荚用户可免费下载高清大图到手机”</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 图片提供方</td>
</tr>

<tr><td >publisher</td>
<td > [Organization](#Organization)</td>
<td > </td>
<td > </td>
<td > 图片出版方</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > </td>
<td > </td>
<td > item 内容的状态（主要用来标记该内容是否下线）(**取值范围:new;updated;offline** )</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 缩略图</td>
</tr>

<tr><td >caption</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 标题</td>
</tr>

<tr><td >contentSize</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 大小(KB)</td>
</tr>

<tr><td >hight</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 高</td>
</tr>

<tr><td >width</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 宽</td>
</tr>

<tr><td >accountablePerson</td>
<td > [Person](#Person)</td>
<td > </td>
<td > </td>
<td > 责任人</td>
</tr>

<tr><td >version</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 版本</td>
</tr>

<tr><td >video</td>
<td > [VideoObject](#VideoObject)</td>
<td > </td>
<td > </td>
<td > 相关视频的信息</td>
</tr>
</tbody></table>

# <a name="Commentary"></a>**内容评论(Commentary)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >id</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 文章ID</td>
</tr>

<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 文章标题</td>
</tr>

<tr><td >content</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 文章正文</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 内容提供方（即应用名称）</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 发表日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 文章最后修改日期</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 文章详情页的webUrl</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 文章详情页的appUrl</td>
</tr>

<tr><td >author</td>
<td > [Author](#Author)</td>
<td > </td>
<td > </td>
<td > 文章作者</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 文章标签</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 文章分类</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 文章中图片</td>
</tr>

<tr><td >interactionCount</td>
<td > [interactionCount](#interactionCount)</td>
<td > </td>
<td > </td>
<td > 用户行为统计</td>
</tr>

<tr><td >isRecommend</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否为精华文章</td>
</tr>

<tr><td >lastReplyDate</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 最后评论时间</td>
</tr>

<tr><td >recommendReplyCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 优质评论数</td>
</tr>

<tr><td >reply</td>
<td > [Reply](#Reply)</td>
<td > </td>
<td > </td>
<td > 文章评论</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 简介</td>
</tr>

<tr><td >packageName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > Y</td>
<td > 包名</td>
</tr>

<tr><td >minVersionCode</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 用于调起时的判断逻辑</td>
</tr>

<tr><td >sourceName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 来自什么应用，用于ranking和呈现等多个逻辑</td>
</tr>
</tbody></table>

# <a name="Library"></a>**文库(Library)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >id</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 文件ID</td>
</tr>

<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 名称</td>
</tr>

<tr><td >fileFormat</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 文件格式</td>
</tr>

<tr><td >contentSize</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 文件大小（字节）</td>
</tr>

<tr><td >author</td>
<td > [Person](#Person)</td>
<td > </td>
<td > </td>
<td > 作者</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 简介</td>
</tr>

<tr><td >numberOfPages</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 总页数</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 浏览数和下载数等信息</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 文件分类</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 文件详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 文件详情页的 AppURL</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 内容提供方</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 创建日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 最近更新日期</td>
</tr>

<tr><td >packageName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > Y</td>
<td > 包名</td>
</tr>

<tr><td >minVersionCode</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 用于调起时的判断逻辑</td>
</tr>
</tbody></table>

# <a name="Lottery"></a>**彩票(Lottery)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >id</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 彩种ID</td>
</tr>

<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 彩种名称</td>
</tr>

<tr><td >issue</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 期数</td>
</tr>

<tr><td >buyAmount</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 购买人数</td>
</tr>

<tr><td >dateErnie</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 开奖日期</td>
</tr>

<tr><td >lotteryNumber</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 开奖号码</td>
</tr>

<tr><td >prizePool</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 奖池金额</td>
</tr>

<tr><td >rewardList</td>
<td > [rewardList](#rewardList)</td>
<td > Y</td>
<td > Y</td>
<td > 奖项列表</td>
</tr>

<tr><td >district</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 发行地区</td>
</tr>
</tbody></table>

# <a name="OpenClass"></a>**公开课(OpenClass)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 课程名称</td>
</tr>

<tr><td >classId</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 课程 ID</td>
</tr>

<tr><td >alternativeHeadline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 课程英文名称</td>
</tr>

<tr><td >inLanguage</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 语言类型</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页的 AppURL</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 课程简介</td>
</tr>

<tr><td >type</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 课程类型（一级分类）</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 所属学科（二级分类）及其他信息</td>
</tr>

<tr><td >organization</td>
<td > [Organization](#Organization)</td>
<td > </td>
<td > </td>
<td > 课程所属机构名称</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 课程封面</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 课程封面缩略图</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 创建日期</td>
</tr>

<tr><td >numberOfClass</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 总课程数</td>
</tr>

<tr><td >lastClassNumber</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 最新课程数</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 最新课程更新时间</td>
</tr>

<tr><td >class</td>
<td > [TVEpisode](#TVEpisode)</td>
<td > Y</td>
<td > </td>
<td > 分集信息</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 总点击/播放/收藏/评论次数</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > </td>
<td > </td>
<td > 在线状态(**取值范围:OFFLINE;ONLINE** )</td>
</tr>

<tr><td >copyrightHolder</td>
<td > [Entity](#Entity)</td>
<td > </td>
<td > </td>
<td > 版权方</td>
</tr>

<tr><td >copyrightYear</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 内容版权生效年份</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 内容提供方</td>
</tr>

<tr><td >lecturer</td>
<td > [Person](#Person)</td>
<td > </td>
<td > </td>
<td > 讲师名称</td>
</tr>

<tr><td >price</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 公开课价格</td>
</tr>
</tbody></table>

# <a name="GameGuide"></a>**游戏攻略(GameGuide)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 攻略标题</td>
</tr>

<tr><td >author</td>
<td > [Person](#Person)</td>
<td > </td>
<td > </td>
<td > 攻略作者</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 攻略类型</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 攻略详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 攻略详情页的 AppURL</td>
</tr>

<tr><td >gameAlias</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 攻略所属游戏的别名</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 攻略封面</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 攻略封面的缩略图</td>
</tr>

<tr><td >content</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 攻略正文</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 攻略内包含的图片内容</td>
</tr>

<tr><td >video</td>
<td > [VideoObject](#VideoObject)</td>
<td > </td>
<td > Y</td>
<td > 攻略视频</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > Y</td>
<td > Y</td>
<td > 描述攻略的关键词/标签</td>
</tr>

<tr><td >datePublished</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 攻略发布日期</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > </td>
<td > </td>
<td > 在线状态(**取值范围:OFFLINE;ONLINE** )</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 评论/阅读数等</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 内容提供方</td>
</tr>

<tr><td >gameName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 攻略所属游戏的名称</td>
</tr>
</tbody></table>

# <a name="TravelTips"></a>**旅行攻略(TravelTips)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >destination</td>
<td > [Place](#Place)</td>
<td > Y</td>
<td > Y</td>
<td > 目的地名称</td>
</tr>

<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 攻略标题</td>
</tr>

<tr><td >editorComments</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 编辑点评/摘要</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 封面图片</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 封面缩略图</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页的 AppURL</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 标签</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 攻略简介</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 创建日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 最近修改时间</td>
</tr>

<tr><td >section</td>
<td > [Section](#Section)</td>
<td > Y</td>
<td > Y</td>
<td > 攻略中每个章节的信息，如景点、餐饮、住宿等，包括标题和内容。</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 内容提供者（应用名称）</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 操作情况统计</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > </td>
<td > </td>
<td > item 内容的状态（主要用来标记该内容是否下线）(**取值范围:offline;online** )</td>
</tr>
</tbody></table>

# <a name="Shopping"></a>**购物(Shopping)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 封面图片缩略图</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 封面图片</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 商品详情图</td>
</tr>

<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 商品标题</td>
</tr>

<tr><td >price</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 商品价格</td>
</tr>

<tr><td >salesCount</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 商品销量</td>
</tr>

<tr><td >aggregateRating</td>
<td > [AggregateRating](#AggregateRating)</td>
<td > </td>
<td > </td>
<td > 商品评论数、好评率</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 商品类目</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 商品详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 商品详情页的 AppURL</td>
</tr>

<tr><td >sellerName</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 商家名称</td>
</tr>

<tr><td >sellerType</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 商家类型（B2C自营、B2C联营、C2C）</td>
</tr>

<tr><td >sellerScore</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 商家得分</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 内容提供方</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 创建日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 最近更新日期</td>
</tr>
</tbody></table>

# <a name="AudioBook"></a>**有声读物(AudioBook)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 作品名称</td>
</tr>

<tr><td >id</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 作品 ID</td>
</tr>

<tr><td >alternativeHeadline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 作品别名/英文名称</td>
</tr>

<tr><td >inLanguage</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 作品语言类型</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 描述</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 作品封面</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 封面图片的缩略图</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页的 AppURL</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 作品分类</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 描述有声作品的关键词/二级分类/标签等</td>
</tr>

<tr><td >price</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 价格</td>
</tr>

<tr><td >author</td>
<td > [Person](#Person)</td>
<td > </td>
<td > </td>
<td > 作者名称</td>
</tr>

<tr><td >announcer</td>
<td > [Person](#Person)</td>
<td > </td>
<td > </td>
<td > 有声读物的朗读者</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 创建日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 最近更新日期</td>
</tr>

<tr><td >audioEpisode</td>
<td > [AudioEpisode](#AudioEpisode)</td>
<td > Y</td>
<td > Y</td>
<td > 音频分集信息</td>
</tr>

<tr><td >copyrightHolder</td>
<td > [Entity](#Entity)</td>
<td > </td>
<td > </td>
<td > 版权方</td>
</tr>

<tr><td >copyrightYear</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 内容版权生效年份</td>
</tr>

<tr><td >isFinished</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否完结</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 总播放/点击/收藏次数</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 内容提供者</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > </td>
<td > </td>
<td > 在线状态(**取值范围:OFFLINE;ONLINE** )</td>
</tr>

<tr><td >packageName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > Y</td>
<td > 包名</td>
</tr>

<tr><td >minVersionCode</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 用于调起时的判断逻辑</td>
</tr>

<tr><td >sourceName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 来自什么应用，用于ranking和呈现等多个逻辑</td>
</tr>
</tbody></table>

# <a name="TravleDiscount"></a>**旅行折扣(TravleDiscount)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >destination</td>
<td > [Place](#Place)</td>
<td > Y</td>
<td > </td>
<td > 目的地信息</td>
</tr>

<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 折扣活动标题</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 折扣类型</td>
</tr>

<tr><td >startTime</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 折扣活动开始日期</td>
</tr>

<tr><td >endTime</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 折扣活动结束日期</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 封面图片</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 封面缩略图</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页的 AppURL</td>
</tr>

<tr><td >value</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 原价</td>
</tr>

<tr><td >price</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 折后价</td>
</tr>

<tr><td >rebate</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 折扣力度</td>
</tr>

<tr><td >boughtCount</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 已预定人数</td>
</tr>

<tr><td >restrictedCondition</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 限制条件（比如出发地，目的地和时间上得限制）</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 对团购详情的描述</td>
</tr>

<tr><td >hotLevel</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 折扣热门程度，取值1-5，数值越大越热门。</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 内容提供者（应用名称）</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 用户操作统计（点击数、阅读量、收藏数等）</td>
</tr>

<tr><td >start</td>
<td > [Place](#Place)</td>
<td > </td>
<td > </td>
<td > 出发地</td>
</tr>
</tbody></table>

# <a name="Encyclopedia"></a>**百科(Encyclopedia)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >id</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 词条 ID</td>
</tr>

<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 词条名</td>
</tr>

<tr><td >subName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 副标题</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 封面图片</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 词条内容图片</td>
</tr>

<tr><td >summary</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 概述</td>
</tr>

<tr><td >basicInfo</td>
<td > [BasicInfo](#BasicInfo)</td>
<td > </td>
<td > Y</td>
<td > 基本信息栏</td>
</tr>

<tr><td >section</td>
<td > [Section](#Section)</td>
<td > </td>
<td > Y</td>
<td > 词条一级标题、标题对应内容、标题对应 WebURL、标题对应 AppURL</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 浏览次数、感觉有用人数、收藏数、分享次数、编辑次数</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 词条类别</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > </td>
<td > 词条标签</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 词条详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 词条详情页的 AppURL</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 内容提供方</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 创建日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 最近更新日期</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 封面图片缩略图</td>
</tr>
</tbody></table>

# <a name="HealthInfo"></a>**健康资讯(HealthInfo)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 疾病名称</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 疾病描述</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > Y</td>
<td > 所属科室</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 标签</td>
</tr>

<tr><td >symptom</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > Y</td>
<td > 症状</td>
</tr>

<tr><td >checkups</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 检查方式</td>
</tr>

<tr><td >cure</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 治疗方法（药品或检查方式）</td>
</tr>

<tr><td >prevention</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 预防方式</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 疾病详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 疾病详情页的 AppURL</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 内容提供方（应用名称）</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 疾病封面图片</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 疾病示意缩略图</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 用户操作记录</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > </td>
<td > </td>
<td > 在线状态（用来标记该内容是否下线）(**取值范围:OFFLINE;ONLINE** )</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 该内容创建日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 该内容修改日期</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 疾病示意图</td>
</tr>
</tbody></table>

# <a name="Ticketing"></a>**票务(Ticketing)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >id</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 演出 ID</td>
</tr>

<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 演出名称</td>
</tr>

<tr><td >alternativeHeadline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 别名</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 演出简介</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 内容提供方</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 类别</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 描述标签</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 详情页 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页 AppURL</td>
</tr>

<tr><td >descriptionUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 演出详细介绍的 WebURL</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 剧照</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 封面图片缩略图</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > </td>
<td > 封面图片</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 创建日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 最近更新日期</td>
</tr>

<tr><td >originalPrice</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 原价</td>
</tr>

<tr><td >sellPrice</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > Y</td>
<td > 实际价格</td>
</tr>

<tr><td >dealPrice</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 团购价</td>
</tr>

<tr><td >deal</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否团购</td>
</tr>

<tr><td >onSaleStatus</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否出售</td>
</tr>

<tr><td >preSale</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否预售</td>
</tr>

<tr><td >bookSeat</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否可选座</td>
</tr>

<tr><td >boughtCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 购票人数</td>
</tr>

<tr><td >ticketClosed</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 演出开始前多少分钟停止售票</td>
</tr>

<tr><td >briefComment</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 短评</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 评论数、关注数量</td>
</tr>

<tr><td >aggregateRating</td>
<td > [AggregateRating](#AggregateRating)</td>
<td > </td>
<td > </td>
<td > 评分总数、整体评分</td>
</tr>

<tr><td >venue</td>
<td > [Venue](#Venue)</td>
<td > Y</td>
<td > </td>
<td > 演出场地信息</td>
</tr>

<tr><td >showInfo</td>
<td > [Performance](#Performance)</td>
<td > Y</td>
<td > </td>
<td > 演出信息</td>
</tr>
</tbody></table>

# <a name="App"></a>**应用(App)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >title</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 应用名称</td>
</tr>

<tr><td >id</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 应用在所属站的 id</td>
</tr>

<tr><td >hash</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 应用详情页 URL 生成的哈希值</td>
</tr>

<tr><td >developerName</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 开发者名称</td>
</tr>

<tr><td >category</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 应用分类</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 应用描述</td>
</tr>

<tr><td >changelog</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 更新日志</td>
</tr>

<tr><td >icon</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 应用图标</td>
</tr>

<tr><td >screenshots</td>
<td > [URL](#URL)</td>
<td > </td>
<td > Y</td>
<td > 应用截图</td>
</tr>

<tr><td >price</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 应用价格</td>
</tr>

<tr><td >downloadUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > apk 下载地址</td>
</tr>

<tr><td >packageName</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 应用包名</td>
</tr>

<tr><td >versionName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 版本名称</td>
</tr>

<tr><td >versionCode</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 版本号</td>
</tr>

<tr><td >lastModification</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 最近更新日期</td>
</tr>

<tr><td >providerName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 应用来源</td>
</tr>

<tr><td >video</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 应用视频演示</td>
</tr>

<tr><td >tags</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 标签</td>
</tr>

<tr><td >alias</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 别名</td>
</tr>

<tr><td >appType</td>
<td > [Enum](#Enum)</td>
<td > </td>
<td > </td>
<td > 类型：“APP”，“GAME”(**取值范围:APP;GAME** )</td>
</tr>

<tr><td >apkSize</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > apk 大小 bytes 数</td>
</tr>
</tbody></table>

# <a name="Animation"></a>**动画(Animation)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 名称（中文名）</td>
</tr>

<tr><td >alternativeHeadline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 别名</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 剧集介绍</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 剧照</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 剧集详情页的WebURL</td>
</tr>

<tr><td >aggregateRating</td>
<td > [AggregateRating](#AggregateRating)</td>
<td > </td>
<td > </td>
<td > 评分信息</td>
</tr>

<tr><td >author</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 原著作者</td>
</tr>

<tr><td >comment</td>
<td > [UserComments](#UserComments)</td>
<td > </td>
<td > Y</td>
<td > 用户评论</td>
</tr>

<tr><td >contentLocation</td>
<td > [Place](#Place)</td>
<td > </td>
<td > Y</td>
<td > 发行地区/国别</td>
</tr>

<tr><td >contentRating</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 官方分级</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 剧集详情页的 AppURL</td>
</tr>

<tr><td >copyrightHolder</td>
<td > [Entity](#Entity)</td>
<td > </td>
<td > </td>
<td > 版权方</td>
</tr>

<tr><td >copyrightYear</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 内容版权生效年份</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 内容创建日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 上次更新日期</td>
</tr>

<tr><td >commentUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 评论页的WebURL</td>
</tr>

<tr><td >editor</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 编剧</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 类型（剧情、悬疑等）</td>
</tr>

<tr><td >headline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 标题（同name）</td>
</tr>

<tr><td >inLanguage</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 语言（粤语/英语等）</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 内容质量评价字段（播放次数、分享次数、收藏次数等）</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 用来描述内容的关键词/标签</td>
</tr>

<tr><td >offer</td>
<td > [Offer](#Offer)</td>
<td > </td>
<td > </td>
<td > 为该内容提供的优惠，例如“豌豆荚用户可免费下载到手机”</td>
</tr>

<tr><td >publisher</td>
<td > [Organization](#Organization)</td>
<td > </td>
<td > </td>
<td > 出版方</td>
</tr>

<tr><td >type</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 类型（TV、OVA、MOVIE、OTHER）</td>
</tr>

<tr><td >role</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 动漫角色</td>
</tr>

<tr><td >director</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 导演</td>
</tr>

<tr><td >startDate</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 开始播出日期</td>
</tr>

<tr><td >endDate</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 结束播出日期</td>
</tr>

<tr><td >animationEpisode</td>
<td > [AnimationEpisode](#AnimationEpisode)</td>
<td > Y</td>
<td > Y</td>
<td > 分集信息</td>
</tr>

<tr><td >numberOfEpisodes</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 总集数</td>
</tr>

<tr><td >lastEpisodeNumber</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 当前最新集数</td>
</tr>

<tr><td >lastEpisodeDate</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 当前最新集的时间</td>
</tr>

<tr><td >producer</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 出品人</td>
</tr>

<tr><td >producerCompany</td>
<td > [Organization](#Organization)</td>
<td > </td>
<td > </td>
<td > 出品公司/电视台</td>
</tr>

<tr><td >season</td>
<td > [TVSeason](#TVSeason)</td>
<td > </td>
<td > </td>
<td > 第几季</td>
</tr>

<tr><td >trailer</td>
<td > [VideoObject](#VideoObject)</td>
<td > </td>
<td > Y</td>
<td > 预告片</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > Y</td>
<td > 封面图片</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 封面缩略图</td>
</tr>

<tr><td >award</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 获奖情况概述</td>
</tr>

<tr><td >dubbings</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 配音演员</td>
</tr>

<tr><td >singer</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 主题曲演唱者</td>
</tr>

<tr><td >update</td>
<td > [Boolean](#Boolean)</td>
<td > Y</td>
<td > </td>
<td > 是否在更新</td>
</tr>

<tr><td >jpName</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 日本名</td>
</tr>

<tr><td >romaji</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 罗马音</td>
</tr>

<tr><td >enName</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 英文名</td>
</tr>

<tr><td >characterSet</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 人设</td>
</tr>

<tr><td >musicSupervision</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 音乐监督</td>
</tr>

<tr><td >website</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 动画官网</td>
</tr>

<tr><td >updateFrequency</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 更新频率</td>
</tr>

<tr><td >stunt</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 一句话推荐</td>
</tr>

<tr><td >nextEpisodeNumber</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 下一集集数</td>
</tr>

<tr><td >nextEpisodeDate</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 下一集播放日期</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > Y</td>
<td > </td>
<td > 内容上下线状态(**取值范围:new;updated;offline** )</td>
</tr>

<tr><td >packageName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > Y</td>
<td > 包名</td>
</tr>

<tr><td >minVersionCode</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 用于调起时的判断逻辑</td>
</tr>

<tr><td >sourceName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 来自什么应用</td>
<td >用于ranking和呈现等多个逻辑</td>
</tr>
</tbody></table>

# <a name="ShortVideo"></a>**短视频(ShortVideo)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 名称</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 剧照图片</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页的 AppURL</td>
</tr>

<tr><td >aggregateRating</td>
<td > [AggregateRating](#AggregateRating)</td>
<td > </td>
<td > </td>
<td > 评分信息</td>
</tr>

<tr><td >author</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 原著作者</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 创建日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 最近更新日期</td>
</tr>

<tr><td >datePublished</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 首次发布日期</td>
</tr>

<tr><td >inLanguage</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 语言(粤语/英语等)</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 用户对视频的操作次数</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 用来描述视频内容的关键词/标签</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 视频内容提供方（即应用名称）</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > Y</td>
<td > </td>
<td > item 内容的状态（主要用来标记该内容是否下线）(**取值范围:new;updated;offline** )</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > Y</td>
<td > 封面图片</td>
</tr>

<tr><td >duration</td>
<td > [Duration](#Duration)</td>
<td > </td>
<td > </td>
<td > 时长</td>
</tr>

<tr><td >videoEpisode</td>
<td > [TVEpisode](#TVEpisode)</td>
<td > Y</td>
<td > Y</td>
<td > 具体的视频信息</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 描述</td>
</tr>

<tr><td >editor</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 编剧</td>
</tr>

<tr><td >director</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 导演</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 类型（剧情、悬疑等）</td>
</tr>

<tr><td >packageName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > Y</td>
<td > 包名</td>
</tr>

<tr><td >minVersionCode</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 用于调起时的判断逻辑</td>
</tr>

<tr><td >sourceName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 来自什么应用，用于ranking和呈现等多个逻辑</td>
</tr>
</tbody></table>

# <a name="Variety"></a>**综艺(Variety)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 名称</td>
</tr>

<tr><td >alternativeHeadline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 别名</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 描述</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 剧照图片</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 详情页的 AppURL</td>
</tr>

<tr><td >aggregateRating</td>
<td > [AggregateRating](#AggregateRating)</td>
<td > </td>
<td > </td>
<td > 评分信息</td>
</tr>

<tr><td >comment</td>
<td > [UserComments](#UserComments)</td>
<td > </td>
<td > Y</td>
<td > 用户评论</td>
</tr>

<tr><td >contentLocation</td>
<td > [Place](#Place)</td>
<td > </td>
<td > Y</td>
<td > 地域/国别</td>
</tr>

<tr><td >contentRating</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 官方分级</td>
</tr>

<tr><td >copyrightHolder</td>
<td > [Entity](#Entity)</td>
<td > </td>
<td > </td>
<td > 版权方</td>
</tr>

<tr><td >copyrightYear</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 内容版权生效年份</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 创建日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 最近更新日期</td>
</tr>

<tr><td >datePublished</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 首次发布日期</td>
</tr>

<tr><td >commentUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 评论页的 WebURL</td>
</tr>

<tr><td >commentAppUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 评论页的 AppURL</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 类型（脱口秀、纪录片等）</td>
</tr>

<tr><td >headline</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 标题，同 name</td>
</tr>

<tr><td >inLanguage</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 语言(粤语/英语等)</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 用户对该节目的操作次数</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 用来描述内容的关键词/标签</td>
</tr>

<tr><td >offer</td>
<td > [Offer](#Offer)</td>
<td > </td>
<td > </td>
<td > 为该内容提供的优惠，例如“豌豆荚用户可免费下载到手机”</td>
</tr>

<tr><td >publisher</td>
<td > [Organization](#Organization)</td>
<td > </td>
<td > </td>
<td > 出版方</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > Y</td>
<td > </td>
<td > 状态信息，默认填写new(**取值范围:new;updated;offline** )</td>
</tr>

<tr><td >startDate</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 播出开始日期</td>
</tr>

<tr><td >endDate</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 播出结束日期</td>
</tr>

<tr><td >videoEpisode</td>
<td > [TVEpisode](#TVEpisode)</td>
<td > Y</td>
<td > Y</td>
<td > 分集信息</td>
</tr>

<tr><td >numberOfEpisodes</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 总集数</td>
</tr>

<tr><td >lastEpisodeNumber</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 最新集</td>
</tr>

<tr><td >lastEpisodeDate</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 最新集的更新时间</td>
</tr>

<tr><td >producer</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 出品人/制作人</td>
</tr>

<tr><td >producerCompany</td>
<td > [Organization](#Organization)</td>
<td > </td>
<td > </td>
<td > 出品公司/电视台</td>
</tr>

<tr><td >season</td>
<td > [TVSeason](#TVSeason)</td>
<td > </td>
<td > </td>
<td > 季的信息，如果有多季的话</td>
</tr>

<tr><td >trailer</td>
<td > [VideoObject](#VideoObject)</td>
<td > </td>
<td > Y</td>
<td > 预告片</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > Y</td>
<td > Y</td>
<td > 封面图片</td>
</tr>

<tr><td >thumbnail</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 封面图片缩略图</td>
</tr>

<tr><td >award</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 获奖情况</td>
</tr>

<tr><td >host</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 主持人</td>
</tr>

<tr><td >guest</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 嘉宾</td>
</tr>

<tr><td >packageName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > Y</td>
<td > 包名</td>
</tr>

<tr><td >minVersionCode</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 用于调起时的判断逻辑</td>
</tr>

<tr><td >sourceName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 来自什么应用</td>
<td >用于ranking和呈现等多个逻辑</td>
</tr>
</tbody></table>

# <a name="weatherInfo"></a>**天气(weatherInfo)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >city</td>
<td > [Place](#Place)</td>
<td > Y</td>
<td > </td>
<td > 预报区域</td>
</tr>

<tr><td >temperature</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 实时温度℃</td>
</tr>

<tr><td >sendibleTemperature</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 实时体感温度℃</td>
</tr>

<tr><td >atmosphere</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 实时气压 hPa</td>
</tr>

<tr><td >weather</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 实时天气</td>
</tr>

<tr><td >humidity</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 实时湿度%</td>
</tr>

<tr><td >windForce</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 实时风力/级</td>
</tr>

<tr><td >windSpeed</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 实时风速 km/h</td>
</tr>

<tr><td >windDirection</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 实时风向</td>
</tr>

<tr><td >forecast</td>
<td > [weekForecast](#weekForecast)</td>
<td > Y</td>
<td > </td>
<td > 一周天气预报</td>
</tr>

<tr><td >accurateForecast</td>
<td > [hourlyForecast](#hourlyForecast)</td>
<td > </td>
<td > Y</td>
<td > 精确日报（分小时数据）</td>
</tr>

<tr><td >airQuality</td>
<td > [airQuality](#airQuality)</td>
<td > </td>
<td > </td>
<td > 空气质量信息</td>
</tr>

<tr><td >livingIndex</td>
<td > [livingIndex](#livingIndex)</td>
<td > </td>
<td > Y</td>
<td > 当日生活指数</td>
</tr>

<tr><td >warningInfo</td>
<td > [warningInfo](#warningInfo)</td>
<td > </td>
<td > Y</td>
<td > 灾害天气预警</td>
</tr>

<tr><td >dateRelease</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 天气信息发布时间</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 预报地天气信息对应的 wap 页面</td>
</tr>

<tr><td >appurl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 调起到预报地天气信息的 appUrl</td>
</tr>

<tr><td >sourceName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 来自什么应用，用于ranking和呈现等多个逻辑</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > Y</td>
<td > </td>
<td > 内容上下线状态(**取值范围:new;updated;offline** )</td>
</tr>

<tr><td >packageName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 包名</td>
</tr>

<tr><td >minVersionCode</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 用于调起时的判断逻辑</td>
</tr>

<tr><td >provider</td>
<td > [Organization](#Organization)</td>
<td > Y</td>
<td > </td>
<td > 内容提供方（应用名称）</td>
</tr>
</tbody></table>

# <a name="Personage"></a>**人物(Personage)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 人物姓名</td>
</tr>

<tr><td >alias</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 人物艺名、外号，或者其他广为人知的名字</td>
</tr>

<tr><td >enName</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 人物外文名</td>
</tr>

<tr><td >gender</td>
<td > [Enum](#Enum)</td>
<td > Y</td>
<td > </td>
<td > 性别，女性为Female，男性为Male(**取值范围:Femal;Male** )</td>
</tr>

<tr><td >birthDate</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 出生日期</td>
</tr>

<tr><td >birthPlace</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 出生地</td>
</tr>

<tr><td >nation</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 民族</td>
</tr>

<tr><td >country</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 国籍</td>
</tr>

<tr><td >horoscope</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 星座</td>
</tr>

<tr><td >bloodType</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 血型</td>
</tr>

<tr><td >height</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 身高，单位 cm，如：180</td>
</tr>

<tr><td >weight</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 体重，单位 kg，如：42</td>
</tr>

<tr><td >interest</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 爱好</td>
</tr>

<tr><td >religion</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 信仰</td>
</tr>

<tr><td >IMDb</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > IMDb编号</td>
</tr>

<tr><td >website</td>
<td > [URL](#URL)</td>
<td > </td>
<td > Y</td>
<td > 官方网站，微博等链接</td>
</tr>

<tr><td >school</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 毕业学校</td>
</tr>

<tr><td >jobs</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 职业</td>
</tr>

<tr><td >company</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 人物所在公司或经纪公司等</td>
</tr>

<tr><td >represent</td>
<td > [namedEntity](#namedEntity)</td>
<td > </td>
<td > Y</td>
<td > 代表作品，Entity的name填写作品名称，如歌名、电影名等，type填写作品类型，如music、movie等，如果没有明确分类，则填写default</td>
</tr>

<tr><td >product</td>
<td > [namedEntity](#namedEntity)</td>
<td > </td>
<td > Y</td>
<td > 主要作品，Entity的name填写作品名称，如歌名、电影名等，type填写作品类型，如music、movie等，如果没有明确分类，则填写default</td>
</tr>

<tr><td >introduction</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 人物介绍，简要描述人物经历以及成就</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 人物封面图片，展示在最外层</td>
</tr>

<tr><td >albums</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 人物相册图片</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 条目发布日期</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 条目修改日期</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 表现人物特征或话题的标签，宫斗剧、偶像等</td>
</tr>

<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 人物领域分类，商业、娱乐等</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 人物详情页webUrl</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 人物详情页appUrl</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 收藏、评论、分享数、喜欢数等用户行为数据</td>
</tr>

<tr><td >packageName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 来源应用包名</td>
</tr>

<tr><td >minVersionCode</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 支持调起最小版本</td>
</tr>

<tr><td >sourceName</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 来源应用名称</td>
</tr>

<tr><td >relationship</td>
<td > [namedEntity](#namedEntity)</td>
<td > </td>
<td > Y</td>
<td > 人物关系，Entity的name填写姓名，如：小明，type填写关系，如：儿子</td>
</tr>
</tbody></table>

# <a name="basicTypes"></a>**基础数据类型**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >类型</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td ><a name="Text"></a>Text</td>
<td >文本</td>
</tr>

<tr><td ><a name="URL"></a>URL</td>
<td ><a name="URL"></a>URL</td>
<td >http://www.example.com or {scheme}://{host_path}</td>
</tr>

<tr><td ><a name="Number"></a>Number</td>
<td >整数或浮点数</td>
</tr>

<tr><td ><a name="Date"></a>Date</td>
<td >日期 YYYY or YYYY-MM-DD or YYYY-MM-DD hh:mm:ss，例如：1984-8-12 09:00:00</td>
</tr>

<tr><td ><a name="Enum"></a>Enum</td>
<td >枚举值，赋值为数据标准对应项的指定字符串</td>
</tr>

<tr><td ><a name="Integer"></a>Integer</td>
<td >整数</td>
</tr>

<tr><td ><a name="Boolean"></a>Boolean</td>
<td >布尔值，取值：True or False</td>
</tr>

<tr><td ><a name="Duration"></a>Duration</td>
<td >正整数，以秒为单位</td>
</tr>

<tr><td ><a name="Float"></a>Float</td>
<td >浮点数</td>
</tr>
</tbody></table>

# <a name="Image"></a>**Image(Image)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 图片的 url</td>
</tr>

<tr><td >height</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 图片的高度</td>
</tr>

<tr><td >width</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 图片的宽度</td>
</tr>
</tbody></table>

# <a name="AggregateRating"></a>**AggregateRating(AggregateRating)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >ratingValue</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 整体评分</td>
</tr>

<tr><td >bestRating</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 最高评分</td>
</tr>

<tr><td >ratingCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 评分总数</td>
</tr>

<tr><td >reviewCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 评论总数</td>
</tr>

<tr><td >worstRating</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 最低评分</td>
</tr>
</tbody></table>

# <a name="Person"></a>**Person(Person)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 人名</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 人物图片</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 人物描述</td>
</tr>
</tbody></table>

# <a name="UserComments"></a>**评论信息(UserComments)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >commentText</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 评论</td>
</tr>

<tr><td >commentTime</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 评论时间</td>
</tr>

<tr><td >creator</td>
<td > [Person](#Person)</td>
<td > Y</td>
<td > </td>
<td > 评论者</td>
</tr>
</tbody></table>

# <a name="Place"></a>**Place(Place)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 地名</td>
</tr>

<tr><td >alias</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 地名的别名/英文名</td>
</tr>

<tr><td >district</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 地点所属区/县</td>
</tr>

<tr><td >districtAlias</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 地点所属区/县英文名</td>
</tr>

<tr><td >city</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 地点所属城市</td>
</tr>

<tr><td >cityAlias</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 地点所属城市英文名</td>
</tr>

<tr><td >location</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 城市所属地域（国家、洲际等）</td>
</tr>

<tr><td >locationAlias</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 城市所属地域（国家、洲际等）英文名</td>
</tr>

<tr><td >longitude</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 位置经度</td>
</tr>

<tr><td >attitude</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 位置纬度</td>
</tr>

<tr><td >locationId</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 城市编码</td>
</tr>
</tbody></table>

# <a name="Entity"></a>**个体(Entity)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 名称</td>
</tr>
</tbody></table>

# <a name="InteractionCount"></a>**InteractionCount(InteractionCount)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >viewCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 阅读/播放数量</td>
</tr>

<tr><td >commentCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 评论数</td>
</tr>

<tr><td >proCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 好评/赞成数量</td>
</tr>

<tr><td >conCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 差评/反对数量</td>
</tr>

<tr><td >favoriteCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 收藏数</td>
</tr>

<tr><td >downloadCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 下载数</td>
</tr>

<tr><td >followerCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 关注数量</td>
</tr>

<tr><td >shareCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 分享次数</td>
</tr>

<tr><td >editCount</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 编辑次数</td>
</tr>
</tbody></table>

# <a name="Tag"></a>**Tag(Tag)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 名字</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 分类/标签/话题详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 分类/标签/话题详情页的 AppURL</td>
</tr>
</tbody></table>

# <a name="Offer"></a>**Offer(Offer)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >description</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 对 offer 的描述</td>
</tr>
</tbody></table>

# <a name="Organization"></a>**Organization(Organization)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 机构名称</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 机构图片</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 机构简介</td>
</tr>
</tbody></table>

# <a name="Chapter"></a>**Chapter(Chapter)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >title</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 标题</td>
</tr>

<tr><td >numberofWords</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 章节字数</td>
</tr>
</tbody></table>

# <a name="BookFormatType"></a>**BookFormatType(BookFormatType)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 格式名称</td>
</tr>
</tbody></table>

# <a name="VideoObject"></a>**VideoObject(VideoObject)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >h5Url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > Y</td>
<td > 视频的 html5 播放页的 WebURL</td>
</tr>

<tr><td >playAppUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 视频播放的 AppURL</td>
</tr>

<tr><td >duration</td>
<td > [Duration](#Duration)</td>
<td > Y</td>
<td > </td>
<td > 时长</td>
</tr>

<tr><td >bitrate</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 码率</td>
</tr>

<tr><td >contentSize</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 播放视频大小</td>
</tr>

<tr><td >encodingFormat</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 播放的视频格式</td>
</tr>

<tr><td >expires</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 视频过期时间</td>
</tr>

<tr><td >videoQuality</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 视频播放分辨率</td>
</tr>

<tr><td >hasCaption</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 播放时是否有字幕</td>
</tr>

<tr><td >free</td>
<td > [Boolean](#Boolean)</td>
<td > Y</td>
<td > </td>
<td > 是否免费</td>
</tr>

<tr><td >downloadInfo</td>
<td > [DownloadInfo](#DownloadInfo)</td>
<td > </td>
<td > </td>
<td > 下载信息</td>
</tr>
</tbody></table>

# <a name="DownloadInfo"></a>**视频下载信息(DownloadInfo)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >encodingFormat</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 视频格式，如 mp4、avi</td>
</tr>

<tr><td >contentSize</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 视频大小，单位为 MB</td>
</tr>

<tr><td >videoQuality</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 视频分辨率，用 pixel 宽×高来标识，如 1920×1080</td>
</tr>

<tr><td >hasCaption</td>
<td > [Boolean](#Boolean)</td>
<td > Y</td>
<td > </td>
<td > 是否有字幕</td>
</tr>

<tr><td >downloadUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 视频的下载地址</td>
</tr>
</tbody></table>

# <a name="TVEpisode"></a>**TVEpisode(TVEpisode)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 名称</td>
</tr>

<tr><td >episodeNumber</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 第几集</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 该集详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 该集详情页的 AppURL</td>
</tr>

<tr><td >commentUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 该集评论页的 WebURL</td>
</tr>

<tr><td >commentAppUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 该集评论页的 AppURL</td>
</tr>

<tr><td >video</td>
<td > [VideoObject](#VideoObject)</td>
<td > Y</td>
<td > Y</td>
<td > 视频信息</td>
</tr>

<tr><td >episodeDate</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 分级播放日期</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 分集封面</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 分集简介</td>
</tr>

<tr><td >playInfo</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 播放参数</td>
</tr>

<tr><td >canDownload</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否能下载</td>
</tr>
</tbody></table>

# <a name="Shop"></a>**Shop(Shop)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 商家名称</td>
</tr>

<tr><td >brand</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 品牌名称</td>
</tr>

<tr><td >telephone</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 联系电话</td>
</tr>

<tr><td >city</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 商家所在城市</td>
</tr>

<tr><td >address</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 地址信息</td>
</tr>

<tr><td >area</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 商圈</td>
</tr>

<tr><td >openTime</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 商铺营业时间</td>
</tr>

<tr><td >longitude</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 经度</td>
</tr>

<tr><td >latitude</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 纬度</td>
</tr>

<tr><td >trafficInfo</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 交通信息</td>
</tr>
</tbody></table>

# <a name="Question"></a>**问题(Question)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >id</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 问题编号</td>
</tr>

<tr><td >author</td>
<td > [Author](#Author)</td>
<td > Y</td>
<td > </td>
<td > 提问者</td>
</tr>

<tr><td >title</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 问题标题</td>
</tr>

<tr><td >detail</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 问题描述</td>
</tr>

<tr><td >tag</td>
<td > [Tag](#Tag)</td>
<td > </td>
<td > Y</td>
<td > 问题的分类/标签/话题</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 创建时间</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 最后一次修改时间</td>
</tr>

<tr><td >dateActivated</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 最近活跃时间</td>
</tr>

<tr><td >answerCount</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 回答数</td>
</tr>

<tr><td >popularity</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 热度，取值1-5。数值越大热度越高</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > </td>
<td > </td>
<td > 问题状态：正常/已关闭/已下线(**取值范围:normal;closed;offline** )</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 用户对问题的操作次数</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 问题的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 问题的 AppURL</td>
</tr>
</tbody></table>

# <a name="Answer"></a>**答案(Answer)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >rank</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 该回答在默认排序方式下的排名</td>
</tr>

<tr><td >author</td>
<td > [Author](#Author)</td>
<td > Y</td>
<td > </td>
<td > 作者</td>
</tr>

<tr><td >content</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 回答内容</td>
</tr>

<tr><td >dateCreated</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 创建时间</td>
</tr>

<tr><td >dateModified</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 最后一次修改时间</td>
</tr>

<tr><td >isAccepted</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否被采用</td>
</tr>

<tr><td >comment</td>
<td > [UserComments](#UserComments)</td>
<td > </td>
<td > Y</td>
<td > 评论信息</td>
</tr>

<tr><td >popularity</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 热度，取值1-5。数值越大热度越高</td>
</tr>

<tr><td >interactionCount</td>
<td > [InteractionCount](#InteractionCount)</td>
<td > </td>
<td > </td>
<td > 用户对答案的操作次数</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 回答内容中的图片</td>
</tr>
</tbody></table>

# <a name="Author"></a>**Author(Author)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 名字</td>
</tr>

<tr><td >detail</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 详细信息</td>
</tr>

<tr><td >level</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 级别</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 用户详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 用户详情页的 AppURL</td>
</tr>
</tbody></table>

# <a name="MusicGroup"></a>**MusicGroup(MusicGroup)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >member</td>
<td > [Person](#Person)</td>
<td > Y</td>
<td > Y</td>
<td > 成员</td>
</tr>
</tbody></table>

# <a name="AudioObject"></a>**AudioObject(AudioObject)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 音频文件的 url</td>
</tr>

<tr><td >duration</td>
<td > [Duration](#Duration)</td>
<td > </td>
<td > </td>
<td > 时长</td>
</tr>

<tr><td >bitrate</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 码率</td>
</tr>

<tr><td >contentSize</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 音频大小</td>
</tr>

<tr><td >encodingFormat</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 音频格式</td>
</tr>
</tbody></table>

# <a name="TVSeason"></a>**TVSeason(TVSeason)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 名称</td>
</tr>

<tr><td >seasonNumber</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 第几季</td>
</tr>

<tr><td >video</td>
<td > [VideoObject](#VideoObject)</td>
<td > Y</td>
<td > </td>
<td > 视频信息</td>
</tr>
</tbody></table>

# <a name="Cinema"></a>**Cinema(Cinema)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 影院名称</td>
</tr>

<tr><td >telephone</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 电话</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 影院图片</td>
</tr>

<tr><td >longitude</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 经度</td>
</tr>

<tr><td >latitude</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 纬度</td>
</tr>

<tr><td >city</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 城市</td>
</tr>

<tr><td >address</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 影院地址</td>
</tr>

<tr><td >area</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 行政区</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 电影院详情页的 url</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 对应的 AppURL</td>
</tr>

<tr><td >businessDistrict</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 商圈</td>
</tr>

<tr><td >busInfo</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 公交信息</td>
</tr>

<tr><td >subwayInfo</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 地铁信息</td>
</tr>

<tr><td >driveInfo</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 自驾信息</td>
</tr>

<tr><td >parkInfo</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 停车信息</td>
</tr>

<tr><td >referencePrice</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 参考价</td>
</tr>

<tr><td >bookSeat</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否可选座</td>
</tr>

<tr><td >sellPrice</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 实际价格</td>
</tr>

<tr><td >deal</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否团购</td>
</tr>

<tr><td >dealPrice</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 团购价</td>
</tr>

<tr><td >feature</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 影院特色</td>
</tr>

<tr><td >note</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 特殊说明</td>
</tr>

<tr><td >brand</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 品牌</td>
</tr>

<tr><td >imax</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否是 IMAX</td>
</tr>

<tr><td >showInfo</td>
<td > [Show](#Show)</td>
<td > </td>
<td > Y</td>
<td > 影片信息</td>
</tr>
</tbody></table>

# <a name="Show"></a>**Show(Show)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >language</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 语言</td>
</tr>

<tr><td >type</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 类型，比如2D、3D、IMAX等</td>
</tr>

<tr><td >date</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 日期</td>
</tr>

<tr><td >showTime</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 放映时间</td>
</tr>

<tr><td >theatre</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 影厅</td>
</tr>

<tr><td >ticketClosed</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 放映前多少分钟停止售票</td>
</tr>

<tr><td >originalPrice</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 原价</td>
</tr>

<tr><td >bookSeat</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否可选座</td>
</tr>

<tr><td >sellPrice</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 实际价格</td>
</tr>

<tr><td >seatUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 座位图页面</td>
</tr>
</tbody></table>

# <a name="Reply"></a>**回复(Reply)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >id</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 评论ID</td>
</tr>

<tr><td >content</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 评论正文</td>
</tr>

<tr><td >replyId</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td ></td>
</tr>

<tr><td >回复评论的ID（用于该条是其他评论的子评论的情况）</td>
</tr>

<tr><td >replyDate</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 评论日期</td>
</tr>

<tr><td >author</td>
<td > [Author](#Author)</td>
<td > </td>
<td > </td>
<td > 评论人</td>
</tr>

<tr><td >interactionCount</td>
<td > [interactionCount](#interactionCount)</td>
<td > </td>
<td > </td>
<td > 用户行为统计</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 回帖图片</td>
</tr>

<tr><td >isRecommend</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否优质（默认为非优质）</td>
</tr>

<tr><td >status</td>
<td > [Enum](#Enum)</td>
<td > </td>
<td > </td>
<td > 内容状态（是否下线）(**取值范围:offline;online** )</td>
</tr>
</tbody></table>

# <a name="rewardList"></a>**奖项列表(rewardList)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >reward</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 奖项名称（如一等奖、二等奖）</td>
</tr>

<tr><td >winningNote</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 中奖注数</td>
</tr>

<tr><td >singleBonus</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 单注奖金</td>
</tr>
</tbody></table>

# <a name="Section"></a>**章节(Section)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >title</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 章节名称</td>
</tr>

<tr><td >content</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 章节内容</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 章节对应WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 章节对应AppUrl</td>
</tr>
</tbody></table>

# <a name="AudioEpisode"></a>**AudioEpisode(AudioEpisode)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 名称</td>
</tr>

<tr><td >episodeNumber</td>
<td > [Integer](#Integer)</td>
<td > Y</td>
<td > </td>
<td > 第几集</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 该集详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 该集详情页的 AppURL</td>
</tr>

<tr><td >commentUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 该集评论页的 WebURL</td>
</tr>

<tr><td >commentAppUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 该集评论页的 AppURL</td>
</tr>

<tr><td >audio</td>
<td > [AudioObject](#AudioObject)</td>
<td > Y</td>
<td > Y</td>
<td > 音频信息</td>
</tr>
</tbody></table>

# <a name="BasicInfo"></a>**表格(BasicInfo)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 属性名称</td>
</tr>

<tr><td >content</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 属性值</td>
</tr>
</tbody></table>

# <a name="Venue"></a>**Venue(Venue)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 场地名称</td>
</tr>

<tr><td >telephone</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 电话</td>
</tr>

<tr><td >image</td>
<td > [Image](#Image)</td>
<td > </td>
<td > Y</td>
<td > 场地图片</td>
</tr>

<tr><td >longitude</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 经度</td>
</tr>

<tr><td >latitude</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 纬度</td>
</tr>

<tr><td >city</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 城市</td>
</tr>

<tr><td >address</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 场地地址</td>
</tr>

<tr><td >area</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 行政区</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 场地详情页的 url</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 场地详情页的 AppURL</td>
</tr>

<tr><td >seatUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 座位图页面</td>
</tr>

<tr><td >theatre</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 演出厅</td>
</tr>

<tr><td >businessDistrict</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 商圈</td>
</tr>

<tr><td >busInfo</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 公交信息</td>
</tr>

<tr><td >subwayInfo</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 地铁信息</td>
</tr>

<tr><td >driveInfo</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 自驾信息</td>
</tr>

<tr><td >parkInfo</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 停车信息</td>
</tr>

<tr><td >feature</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 场地特色</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 场地简介</td>
</tr>

<tr><td >note</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 特殊说明</td>
</tr>
</tbody></table>

# <a name="Performance"></a>**Performance(Performance)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >language</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 语言</td>
</tr>

<tr><td >showTime</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > Y</td>
<td > 演出时间</td>
</tr>

<tr><td >duration</td>
<td > [Duration](#Duration)</td>
<td > </td>
<td > </td>
<td > 时长</td>
</tr>

<tr><td >actor</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 演员</td>
</tr>

<tr><td >director</td>
<td > [Person](#Person)</td>
<td > </td>
<td > </td>
<td > 导演</td>
</tr>

<tr><td >screenwriter</td>
<td > [Person](#Person)</td>
<td > </td>
<td > </td>
<td > 编剧</td>
</tr>

<tr><td >others</td>
<td > [Person](#Person)</td>
<td > </td>
<td > Y</td>
<td > 其他人员</td>
</tr>
</tbody></table>

# <a name="AnimationEpisode"></a>**AnimationEpisode(AnimationEpisode)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 名称</td>
</tr>

<tr><td >episodeNumber</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 第几集</td>
</tr>

<tr><td >url</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 该集详情页的 WebURL</td>
</tr>

<tr><td >appUrl</td>
<td > [URL](#URL)</td>
<td > Y</td>
<td > </td>
<td > 该集详情页的 AppURL</td>
</tr>

<tr><td >commentUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 该集评论页的 WebURL</td>
</tr>

<tr><td >commentAppUrl</td>
<td > [URL](#URL)</td>
<td > </td>
<td > </td>
<td > 该集评论页的 AppURL</td>
</tr>

<tr><td >video</td>
<td > [VideoObject](#VideoObject)</td>
<td > Y</td>
<td > Y</td>
<td > 视频信息</td>
</tr>

<tr><td >episodeDate</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 分级播放日期</td>
</tr>

<tr><td >cover</td>
<td > [Image](#Image)</td>
<td > </td>
<td > </td>
<td > 分集封面</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 分集简介</td>
</tr>

<tr><td >playInfo</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 播放参数</td>
</tr>

<tr><td >canDownload</td>
<td > [Boolean](#Boolean)</td>
<td > </td>
<td > </td>
<td > 是否能下载</td>
</tr>

<tr><td >jpName</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 日文名</td>
</tr>

<tr><td >romaji</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 罗马音</td>
</tr>

<tr><td >enName</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 英文名</td>
</tr>

<tr><td >episodeId</td>
<td > [Integer](#Integer)</td>
<td > </td>
<td > </td>
<td > 分集的ID</td>
</tr>
</tbody></table>

# <a name="weekForecast"></a>**周际预报(weekForecast)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >dayOne</td>
<td > [Forecast](#Forecast)</td>
<td > Y</td>
<td > </td>
<td > 当日(T+0)预报</td>
</tr>

<tr><td >dayTwo</td>
<td > [Forecast](#Forecast)</td>
<td > Y</td>
<td > </td>
<td > T+1 预报</td>
</tr>

<tr><td >dayThree</td>
<td > [Forecast](#Forecast)</td>
<td > Y</td>
<td > </td>
<td > T+2 预报</td>
</tr>

<tr><td >dayFour</td>
<td > [Forecast](#Forecast)</td>
<td > Y</td>
<td > </td>
<td > T+3 预报</td>
</tr>

<tr><td >dayFive</td>
<td > [Forecast](#Forecast)</td>
<td > Y</td>
<td > </td>
<td > T+4 预报</td>
</tr>

<tr><td >daySix</td>
<td > [Forecast](#Forecast)</td>
<td > Y</td>
<td > </td>
<td > T+5 预报</td>
</tr>

<tr><td >daySeven</td>
<td > [Forecast](#Forecast)</td>
<td > </td>
<td > </td>
<td > T+6 预报</td>
</tr>
</tbody></table>

# <a name="hourlyForecast"></a>**精确日报（分小时数据）(hourlyForecast)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >temperature</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 温度</td>
</tr>

<tr><td >weather</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 天气</td>
</tr>

<tr><td >humidity</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 湿度</td>
</tr>

<tr><td >windForce</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 风力</td>
</tr>

<tr><td >windDirection</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 风向</td>
</tr>

<tr><td >precipitation</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 降水量 mm/h</td>
</tr>

<tr><td >precipitationProbability</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 降水概率</td>
</tr>

<tr><td >time</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 预报时间</td>
</tr>
</tbody></table>

# <a name="airQuality"></a>**空气质量(airQuality)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >AQI</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 空气质量指数</td>
</tr>

<tr><td >qualityLevel</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 总体评级（如：严重污染）</td>
</tr>

<tr><td >PM2.5</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 细颗粒物浓度ug/m3</td>
</tr>

<tr><td >PM10</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 可吸入颗粒物浓度ug/m3</td>
</tr>

<tr><td >SO2</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 二氧化硫浓度ug/m3</td>
</tr>

<tr><td >NO2</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 二氧化氮浓度ug/m3</td>
</tr>

<tr><td >O3</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 臭氧浓度</td>
</tr>

<tr><td >CO</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 一氧化碳浓度</td>
</tr>

<tr><td >suggestion</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 活动建议</td>
</tr>

<tr><td >dateRelease</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 发布时间</td>
</tr>
</tbody></table>

# <a name="livingIndex"></a>**生活指数(livingIndex)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 指数名称</td>
</tr>

<tr><td >level</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 指数级别</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 指数内容&amp;活动建议</td>
</tr>
</tbody></table>

# <a name="warningInfo"></a>**灾害天气预警信息(warningInfo)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >genre</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 预警类别</td>
</tr>

<tr><td >level</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 预警级别</td>
</tr>

<tr><td >title</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 预警标题</td>
</tr>

<tr><td >description</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 预警详情</td>
</tr>

<tr><td >dateRelease</td>
<td > [Date](#Date)</td>
<td > Y</td>
<td > </td>
<td > 预警发布时间</td>
</tr>
</tbody></table>

# <a name="Forecast"></a>**天气预报(Forecast)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >maxTemperature</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 最高气温℃</td>
</tr>

<tr><td >minTemperature</td>
<td > [Number](#Number)</td>
<td > Y</td>
<td > </td>
<td > 最低气温℃</td>
</tr>

<tr><td >dayWeather</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 日间天气</td>
</tr>

<tr><td >nightWeather</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > 夜间天气</td>
</tr>

<tr><td >maxHumidity</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 最大相对湿度%</td>
</tr>

<tr><td >minHumidity</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 最小相对湿度%</td>
</tr>

<tr><td >daywindForce</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 日间风力/级</td>
</tr>

<tr><td >nightwindForce</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 夜间风力/级</td>
</tr>

<tr><td >daywindDirection</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 日间风向</td>
</tr>

<tr><td >nightwindDirection</td>
<td > [Text](#Text)</td>
<td > </td>
<td > </td>
<td > 夜间风向</td>
</tr>

<tr><td >sunrise</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 日出时间</td>
</tr>

<tr><td >sunset</td>
<td > [Date](#Date)</td>
<td > </td>
<td > </td>
<td > 日落时间</td>
</tr>

<tr><td >dayprecipitationProbability</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 日间降水概率</td>
</tr>

<tr><td >nightprecipitationProbability</td>
<td > [Number](#Number)</td>
<td > </td>
<td > </td>
<td > 夜间降水概率</td>
</tr>

<tr><td >trafficControls</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > 当日限行号码</td>
</tr>
</tbody></table>

# <a name="namedEntity"></a>**命名实体(namedEntity)标准**

<table  style="width:100%; "  class="easy-table easy-table-cuscosky " >
<thead>
<tr><th >属性</th>
<th >期望类型</th>
<th style="width:50px">是否必须</th>
<th style="width:80px">是否可以有多个</th>
<th >描述</th>
</tr>
</thead>
<tbody>
<tr><td >name</td>
<td > [Text](#Text)</td>
<td > Y</td>
<td > </td>
<td > Entity的名称</td>
</tr>

<tr><td >type</td>
<td > [Text](#Text)</td>
<td > </td>
<td > Y</td>
<td > Entity的类型</td>
</tr>
</tbody></table>

		</article>
		<!-- /article -->

	<div class="more-help">

如果您需要更多帮助，请在此提交，我们将在 1 个工作日内回复。[请求帮助](http://uowechat.wandoujia.com/feedback)

	</div>

	</section>
	<!-- /section -->
</div>