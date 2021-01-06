# 深度學習

## Word2Vec

### 資料集

[PTT小資料集](https://drive.google.com/open?id=1BT4h4-kzrtCS_52P2i7C1rlj1GZgEbs6)

[PTT大資料集](https://drive.google.com/open?id=15byko6d_9VJGPOW7DPAN8YiVsleRiURr)

### 標點符號去除

```python
punct = set(u''':!),.:;?]}¢'"、。〉》」』】〕〗〞︰︱︳﹐､﹒﹔﹕﹖﹗﹚﹜﹞！），．：；？｜｝︴︶︸︺︼︾﹀﹂﹄﹏､～￠々‖•·ˇˉ―--′’”([{£¥'"‵〈《「『【〔〖（［｛￡￥〝︵︷︹︻︽︿﹁﹃﹙﹛﹝（｛“‘-—_…~/ －＊➜■─★☆=@<>◉é''')
filter(lambda x: x not in punct, jieba.cut(content))
```

### 網址Regex

```python
content = re.sub(r'https?:\/\/.*[\r\n]*', '', content)
```

### 推薦文章

[w2v](https://colab.research.google.com/drive/1ViQxHhPZtGRKDO9ELAXEVux7bAgvY0In?usp=sharing)

[Face(GPU)](https://colab.research.google.com/drive/1Fdzjw0Rh4ZzRVDvObKAskPAY4AHP-2za?usp=sharing)
