����Conciseness���ϼ�Leanote����[�����г�](https://leanote.com/member/blog/theme)���������޸���[roomcar](http://roomcar.leanote.com/single/me)��pure���⡣

����Ԥ��ͼ������ʾ��

![54999990-file_1487997191856_69e5.png](https://www.tuchuang001.com/images/2017/06/13/54999990-file_1487997191856_69e5.png)

������������޸ģ�������������ܡ�     
## �޸�ͼƬ
�༭���⣬�ҵ�theme.json�ļ������ֶΣ�
```xml
...
"BlogImgName": "blogImg.jpg",
"WebImgName": "webImg.png",
"ErrorImgName": "robot.png",    
...
```
`BlogImgName`Ϊ����About MeͼƬ��`WebImgName`Ϊ��ҳСͼ�꣬`ErrorImgName`Ϊ404ҳ��ͼƬ��

�����������뽫About Me��ͼƬ��Ϊ�Լ��ϴ�����ΪhandsomeBoy.png����Ƭ��ֻ�轫theme.json�ļ���BlogImgName�ֶ�ֵ��λ��handsomeBoy.png�����ɡ�
## �޸�About Me����
�༭���⣬�ҵ�theme.json�ļ������ֶΣ�
```xml
"QQ": "123456",
"Weico": "http://weibo.com/",
"Facebook": "https://www.facebook.com/",
```
�ɽ�����ֵ��Ϊ�Լ������Ӽ��ɡ�
## �޸�����
���ֲ�����ԣ�[32�ռ�](https://32mb.space/)��

�޸�����ֻ���޸�theme.json�ļ��е�MusicUrl ���Լ��ɡ������Ե�ֵΪһ�����飬��ʽ������ʾ��
```javascript
 {"title": "musicTitle","artist":"artist","mp3": "musicUrl","cover": "musicCover"},
```
titleΪ��������artistΪ��������mp3Ϊ�������ӣ�coverΪר�����档�����⼸��ֵ�Ļ�ȡ��������������ϸ���ܣ�

1.����������������������Ī��ε�ġ��������ˡ����ɵõ���������Ϊ��http://music.163.com/#/song?id=30621954&userid=3425798������song��idΪ30621954��

2.���Ƹ�id�������ӣ�http://music.163.com/api/song/detail/?id=yourId&ids=%5ByourId%5D&csrf_token=��

3.�������е�yourId����Ϊ��һ�����Ƶ�����id��Ȼ��س����ɿ���ҳ�������һ��json��ʽ���ݣ�
```javascript
{
"songs": [
    {
    "name": "��������",
    "id": 30621954,
...
    "artists": [
        {
        "name": "Ī��ε",
        "id": 8926,
        "picId": 0,
        "img1v1Id": 0,
        "briefDesc": "",
        "picUrl": "http://p3.music.126.net/6y-UleORITEDbvrOLV0Q8A==/5639395138885805.jpg",
        "img1v1Url": "http://p4.music.126.net/6y-UleORITEDbvrOLV0Q8A==/5639395138885805.jpg",
        "albumSize": 0,
        "alias": [],
        "trans": "",
        "musicSize": 0
    }
        ],
    "album": {
        "name": "��������",
        "id": 3104146,
        "type": "EP/Single",
        "size": 1,
        "picId": 7860408627221136,
        "blurPicUrl": "http://p3.music.126.net/2nJOdPf1RlGY_tQdB5ZdPA==/7860408627221136.jpg",
        "companyId": 0,
        "pic": 7860408627221136,
        "picUrl": "http://p4.music.126.net/2nJOdPf1RlGY_tQdB5ZdPA==/7860408627221136.jpg",
        "publishTime": 1424188800007,
...        
        "mp3Url": "http://m2.music.126.net/tQ0pNmpsiHIsxEl-CnMmJg==/7897792022607979.mp3"
        }
    ],
"equalizers": {},
"code": 200
}
```
һ���json���ݣ��������йصľͼ���������`title`����������дΪ���������ˡ���`artist`Ϊ��Ī��ε����`mp3`Ϊjson�����е�mp3Url�ֶΣ�����Ϊ��[http://m2.music.126.net/tQ0pNmpsiHIsxEl-CnMmJg==/7897792022607979.mp3](http://m2.music.126.net/tQ0pNmpsiHIsxEl-CnMmJg==/7897792022607979.mp3)��`cover`Ϊjson�ļ��е�album��picUrl�ֶ�ֵ������Ϊ��[http://p4.music.126.net/2nJOdPf1RlGY_tQdB5ZdPA==/7860408627221136.jpg](http://p4.music.126.net/2nJOdPf1RlGY_tQdB5ZdPA==/7860408627221136.jpg)���������յ����׸�Ĵ���Ϊ��
```javascript
 {
    "title": "��������",
    "artist":"Ī��ε",
    "mp3": "http://m2.music.126.net/tQ0pNmpsiHIsxEl-CnMmJg==/7897792022607979.mp3",
    "cover": "http://p4.music.126.net/2nJOdPf1RlGY_tQdB5ZdPA==/7860408627221136.jpg"
},
```
����δ���ӵ�theme.json�ļ��е�musicUrl�����м��ɡ�
## ������Ч
�������Լ����ۿ��ڼ����˲��activate-power-mode.js��Ч���������Ҫ�����ҵ�0-c.html��55�У�
```javascript
<script>
    POWERMODE.colorful = true; 
    POWERMODE.shake = false; 
    document.body.addEventListener('input', POWERMODE);
</script> 
```
���⼸�д���ɾ�����ɡ�
## ������
ҳ�浯����ʹ�õ���sweetAlert.js�������ɾ�������Լ�δ��¼״���µ�����ĵ����ۺ͵��ް�ť���ɴ������磺

![67095376-file_1487997218085_ff4e.png](https://www.tuchuang001.com/images/2017/06/13/67095376-file_1487997218085_ff4e.png) 

��ӦAPI�ɲ鿴sweetAlert���������������share_comment.js�ļ��п��ҵ���ش��롣

��������ʣ���ӭ���ԡ�

**2017��3��27��**

�޸�һЩbug����ʽ������