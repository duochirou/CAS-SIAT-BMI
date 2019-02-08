=====Description=====</br>
We create two Chinese datasets by manually annotating the restaurant and digital camera reviews from the Dianping (https://www.dianping.com) website. The raw corpus was originally made public by (Y. Zhang, et al, 2013). We randomly select 6,000 restaurant reviews (in restaurant.txt) and 6,000 digital camera reviews (in digital_camera.txt ) from the original corpus, and three experienced human annotators are invited to label the aspect categories and their sentiment polarities (“positive”, “negative” and “neutral”) of each document.

[1] Yongfeng Zhang, Min Zhang, Yiqun Liu, Shaoping Ma and Shi Feng. Localized Matrix Factorization for Recommendation based on Matrix Block Diagonal Forms. In Proceedings of the 22nd International Conference on World Wide Web, 2013.

=====Format and Examples=====</br>
Each review is formatted as an XML entry. The following example illustrates the format of the annotated sentences of the restaurants dataset.</br>
&lt;sentence&gt;</br>
	&emsp;&emsp;&lt;text&gt;点评里的优惠券几乎没有断过.他们家非节假日的中午还会搞主食类半价的活动.石锅拌饭 觉得挺好吃的.就是不喜欢他家服务员的态度&lt;/text&gt;</br>
	&emsp;&emsp;&lt;aspectCategories&gt;</br>
		&emsp;&emsp;&emsp;&emsp;&lt;aspectCategory category="food" polarity="1"/&gt;</br>
		&emsp;&emsp;&emsp;&emsp;&lt;aspectCategory category="service" polarity="3"/&gt;</br>
	&emsp;&emsp;&lt;/aspectCategories&gt;</br>
&lt;/sentence&gt;</br>

The possible values of the polarity field are: 1 (“positive”), 2 (“neutral”), 3 (“negative”). The possible values of the category field are: “food”, “service”, “price”, “environment”.

The following example illustrates the format of the annotated sentences of the digital camera.</br>
&lt;sentence&gt;</br>
	&emsp;&emsp;&lt;text&gt;性价比高，值.对于这么超值的价格，有点不足都可以忽略.１５倍变焦很不错，全景拍摄效果好&lt;/text&gt;</br>
	&emsp;&emsp;&lt;aspectCategories&gt;</br>
		&emsp;&emsp;&emsp;&emsp;&lt;aspectCategory category="price" polarity="1"/&gt;</br>
		&emsp;&emsp;&emsp;&emsp;&lt;aspectCategory category="performance" polarity="1"/&gt;</br>
	&emsp;&emsp;&lt;/aspectCategories&gt;</br>
&lt;/sentence&gt;</br>

The possible values of the polarity field are: 1 (“positive”), 2 (“neutral”), 3 (“negative”). The possible values of the category field are: "performance", "price", "quality", "appearance", "easy_to_use".

=====Contact=====</br>
min.yang1129@gmail.com
