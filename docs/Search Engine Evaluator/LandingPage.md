## Landing Page

### 任务

> 评价目标网页

### 什么是Landing Page(LP)

当用户点击广告时，所导向的网页就是Landing Page

> The user starts a search on Google.com with a goal in mind. The user enters a query and reviews Google’s search results and ads. The user then clicks on the ad currently being reviewed, and that ad takes the user to the landing page (LP). In order for a user to have a positive experience with an advertiser landing page, he or she should be closer to the goal expressed in the query, otherwise it is a negative experience. (官方原文)



### Landing Page Ratings

- **Satisfaction Likely**

  - > To receive this rating, a landing page must offer exactly what the user is looking for.

    如果LP明确符合用户的意图，评分在76-100

    如果LP是用户想要的结果之一，但是不是用户想要的所有结果，有点单一，评分51-75

    

- **Satisfaction Possible**

  - 如果LP能够满足用户的需求，但是不能立即直接展现给用户，需要用户进行一些额外的操作

    > Use this rating if the page is satisfactory but does not immediately present exactly what the user seeks. If the product or service is for sale on the site, but a search or straightforward navigation is required to find the item, select a rating of Satisfaction Possible rather than Satisfaction Likely.

    如果LP能够满足用户的需求，但是不能立即展现给用户，还需要用户点击导航的，评分为26-50

    如果LP能够满足用户的需求，但是还需要用户进行较繁琐的操作（比如再次搜索商品），评分为1-25

- **Dissatisfaction Possible**

  - 如果LP的主要内容不是满足用户的需求，需要用户花费时间寻找想要的东西，甚至导向其它的网站

    > If the LP is marginally related to the query and you think there’s a small chance the user would be interested, use Dissatisfaction Possible. Also, if the page can eventually lead to what the user wants, but only through many clicks or through clicks that lead to an entirely different website, use Dissatisfaction Possible.

    如果LP主要内容不是满足用户的需求，但是提供了与用户的意图有比较大关联的内容，评分为-25~ -1

    如果LP主要内容不是满足用户的需求，但是提供了与用户的意图有比较小关联的内容，评分为-50~ -26

- **Dissatisfaction Likely**

  - 如果页面内容与用户意图毫无关联的，如果是产品或服务，页面不能提供购买服务的，如果查询有两个含义，但是如果用户的意图很明显，LP却提供不同的结果的，如果页面看起来像诈骗，用户会受到不良的影响的，如果LP试图在没有用户操作下下载文件的

    > If the page has nothing to do with the query, use Dissatisfaction Likely. If the query is for a product or service, and neither the product/service nor anything close to it can be purchased from the page, use Dissatisfaction Likely. If the query or a word in the query has two meanings, it is clear which meaning is intended by the user, and the advertiser responds to the wrong meaning, use Dissatisfaction Likely. If the page looks like a scam, you think users could be harmed by it, or it either attempts to trick the user into downloading something by labeling a download button in a confusing way or tries to download a file without action by the user, use Dissatisfaction Likely.

    如果LP与用户意图没有任何关系，但LP页面中有与查询内容相关联的单词，评分为-75~-51

    如果LP与用户意图没有任何关系，且与查询内容没有任何关联，评分为-100~-76

## Flagging the Landing Page

> In addition to rating the **landing page**, you should also select any applicable **LP flags**. 

除了给LP评分外，还需要给LP添加对应的标签，以表示LP的类型

* Navigational Bullseye

  > Use the **Navigational Bullseye** flag when both these things are true:
  >
  > - The query appears to be a search for a particular webpage.
  > - The landing page is that page.

  这个标签一般是对于特殊的，唯一的LP（例如官网）

* Foreign Language

  > Use the **Foreign Language** flag when the landing page is in a language other than the task language, with no obvious way of getting to a version in the task language. Don’t use this flag if there is some clear way to get to a version in the target language.

  这个标签适用于LP的语言与查询的语言不同

* Unexpected Porn

  > Use this flag when both these things are true:
  >
  > - The query is not a search for pornographic content or sexual services. If the query has both a pornographic interpretation and a non-pornographic interpretation, assume that the non-pornographic interpretation is the actual user intent.
  > - The landing page offers pornographic content or sexual services.

  这个标签用于LP是用户不想看到的成人页面

* Unexpected Download

  > Use the **Unexpected Download** flag when any of the following happens:
  >
  > - Clicking on the Visit Landing Page button initiates an attempt to download a file.
  > - Some link, button, or graphic on the landing page initiates a download when clicked, but does not clearly indicate that it will do so. For example, a big red button that says “Enter site” or “Check the weather,” but starts a download when clicked, deserves the flag. A similar button that says “Get It Now” or “Click here to download” does not.

  这个标签适用于LP在用户没有操作下去下载文件

* Error/Did Not Load

  > Use the **Error/Did Not Load** (EDNL) flag to indicate that you cannot evaluate the landing page because there is no landing site content provided by the advertiser.

  这个标签适用于LP未能完全加载，显示错误，网站错误

* Secondary Interpretation of the Query

  > Use this flag when the landing page content indicates that the advertiser is targeting a clearly **secondary interpretation of the query**. An interpretation is secondary if it’s reasonable, but there is some other interpretation of the query that you consider much more likely.
  >
  > - Don’t use this flag with interpretations that are wrong or unreasonable.
  >
  > - Don’t
  >
  >    use this flag if you think that the query has multiple, equally likely meanings, and the advertiser is targeting one of those meanings.
  >
  >   - Example: If a user is searching for [[mouse](https://www.google.com/search?q=mouse)], and the LP is [this](https://www.bestbuy.com/site/computer-accessories/mice-keyboards/abcat0513000.c?id=abcat0513000).
  >
  > - Do use the flag where the query has multiple, equally likely meanings and the advertiser targets an obscure or less-likely meaning.

  这个标签仅用于查询内容含义是多重的，如果LP的内容含义是查询内容很少见的含义的