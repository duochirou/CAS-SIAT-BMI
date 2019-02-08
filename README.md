=====Description=====</br>
We create two Chinese datasets by manually annotating the restaurant and digital camera reviews from the Dianping (https://www.dianping.com) website. The raw corpus was originally made public by (Y. Zhang, et al, 2013). We randomly select 6,000 restaurant reviews (in restaurant.txt) and 6,000 digital camera reviews (in digital_camera.txt ) from the original corpus, and three experienced human annotators are invited to label the aspect categories and their sentiment polarities (��positive��, ��negative�� and ��neutral��) of each document.

[1] Yongfeng Zhang, Min Zhang, Yiqun Liu, Shaoping Ma and Shi Feng. Localized Matrix Factorization for Recommendation based on Matrix Block Diagonal Forms. In Proceedings of the 22nd International Conference on World Wide Web, 2013.

=====Format and Examples=====</br>
Each review is formatted as an XML entry. The following example illustrates the format of the annotated sentences of the restaurants dataset.</br>
&lt;sentence&gt;</br>
	&emsp;&emsp;&lt;text&gt;��������Ż�ȯ����û�жϹ�.���Ǽҷǽڼ��յ����绹�����ʳ���۵Ļ.ʯ���跹 ����ͦ�óԵ�.���ǲ�ϲ�����ҷ���Ա��̬��&lt;/text&gt;</br>
	&emsp;&emsp;&lt;aspectCategories&gt;</br>
		&emsp;&emsp;&emsp;&emsp;&lt;aspectCategory category="food" polarity="1"/&gt;</br>
		&emsp;&emsp;&emsp;&emsp;&lt;aspectCategory category="service" polarity="3"/&gt;</br>
	&emsp;&emsp;&lt;/aspectCategories&gt;</br>
&lt;/sentence&gt;</br>

The possible values of the polarity field are: 1 (��positive��), 2 (��neutral��), 3 (��negative��). The possible values of the category field are: ��food��, ��service��, ��price��, ��environment��.

The following example illustrates the format of the annotated sentences of the digital camera.</br>
&lt;sentence&gt;</br>
	&emsp;&emsp;&lt;text&gt;�Լ۱ȸߣ�ֵ.������ô��ֵ�ļ۸��е㲻�㶼���Ժ���.�������佹�ܲ���ȫ������Ч����&lt;/text&gt;</br>
	&emsp;&emsp;&lt;aspectCategories&gt;</br>
		&emsp;&emsp;&emsp;&emsp;&lt;aspectCategory category="price" polarity="1"/&gt;</br>
		&emsp;&emsp;&emsp;&emsp;&lt;aspectCategory category="performance" polarity="1"/&gt;</br>
	&emsp;&emsp;&lt;/aspectCategories&gt;</br>
&lt;/sentence&gt;</br>

The possible values of the polarity field are: 1 (��positive��), 2 (��neutral��), 3 (��negative��). The possible values of the category field are: "performance", "price", "quality", "appearance", "easy_to_use".

=====Contact=====</br>
min.yang1129@gmail.com
