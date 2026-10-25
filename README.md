# 英雄缩略图

头像在 `img/heroes/<slug>.webp`（约 90×90），页面只引用仓库里的文件，不要外链。

新增一个英雄：

1. 打开该英雄的 fastidious.gg 页面，取 `hero.image_card_micro`（一般是 `https://fastidious.gg/storage/cards/<slug>_card_micro.webp`），原样存成 `img/heroes/<slug>.webp`。
2. 如果没有 micro 图标，改用 Wiki 的 `File:<Name>_portrait.png`，下载后转成 90×90 的 webp。
3. 在名册、愿望单或编队里，把这张图放在英雄名字前面。缺图时用首字母占位，不要裁 Fastidious 卡面来凑。

Fastidious 的 micro 已经自带稀有度底、阵营和职业。只有裸的 Wiki 立绘需要在后面垫 `img/frames/<rarity>-90.webp`（页面类名 `hero-slot`）。Veyrathia 是史诗，用 `epic-90.webp`；Nerissa 是传说，用 `legendary-90.webp`。Fastidious 把 Erlang Shen 标成 Legendary，所以如果写进正文，用 `legendary-90.webp`，不用红色远古框。仓库里没有神话/远古卡面，那种立绘才用 `rarity.css` 里的 `.r-mythic` 红框渐变。

名字旁边表示该英雄星级的 `N★` 用 `img/frames/<rarity>-star-wiki.webp`，颜色跟稀有度走。数字留在 `title` 和视觉隐藏文字里。关卡星、狗粮和「不要升 6★」这类说明保持原文。觉醒 A1–A5 用 `rarity.css` 的徽章色（A1–A2 灰、A3–A4 琥珀、A5 金）。职业筛选按钮用 `img/icons/class-*.webp`。

Veyrathia、Nerissa、Erlang Shen 没有 Fastidious micro 图标，用的是 Wiki 立绘（`veyrathia.webp`、`nerissa.webp`、`erlangshen.webp`），没有裁卡面。Erlang Shen、Malvira、Nastya 的图已经放在目录里，当前正文还没写到这三个人，所以页面上不显示。Valara 同样没有 micro，页面上暂时用首字母。
