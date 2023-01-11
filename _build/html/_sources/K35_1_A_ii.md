# Perception > Sensing >  Digital Encoding
% 제목 MyST 스타일로 넣는 방법 확인해야 함
% 태그 키워드 추가하기 

## 컴퓨터가 이미지를 디지털로 인식하는 방법
```{figure} https://lh4.googleusercontent.com/3-rC8LGzAFQ5AxBdzZV4xfkfZuuGXfOwWEDkoVXdQn1io7_EFznhNDclP3wrH5tnOdVkdDwIBlyTw_Ng2aaEd16MToCKXGfkg6AM9LcemeIQwpEiPIJdTvaS7Xq-m__lfuwGXoAjMsQgUm87fRisK6Sj3NkPG5GoLNzb9ntf7mZ3vpak7Vdyb5QZFYiG6x-SWCJYrnjaQg
:alt: cat-01
:width: 400
:align: center

이미지 제목을 넣어주세요. 
```

위에 하나의 이미지([](#cat-01))가 있습니다. 제시된 이미지가 무엇으로 보이나요? 아마 많은 분이 자신 있게 고양이라 말할 것입니다. 우리 인간은 이 이미지를 보고 바로 ‘고양이'라고 이야기하지만, 컴퓨터도 인간과 마찬가지로 한 번에 고양이로 알아볼 수 있을까요? 어렵습니다. 그렇다면 과연 컴퓨터는 어떻게 이미지를 (보고 삭제) 인식하는지 알아보도록 합시다. 그러기 위해 먼저 사람이 판단한 ‘고양이’라는 표현 대신 ‘이미지 데이터’라고 불러보죠.

### 이미지 데이터란?
이미지 데이터는 디지털로 이미지를 구성하는 최소 단위인 픽셀(Pixel)들의 집합을 의미합니다. 너무 말이 어렵다고요? 미술 시간에 모자이크했던 것을 떠올려 봅시다. 모자이크 작품을 어떻게 만들었나요? 아마 여러분은 색종이를 찢고, 그 조각을 모아 붙여 하나의 큰 그림을 완성했을 것입니다. 찢긴 색종이 조각이 픽셀이고, 완성된 모자이크 작품이 이미지 데이터라고 보면 됩니다. 이처럼 이미지 데이터는 픽셀 단위의 작은 이미지들을 모아서 완성한 하나의 그림이라고 할 수 있습니다.  


```{figure} https://lh5.googleusercontent.com/iNWx1HD5aM_HISesOGJSjSvIGBK8-4aHN6dNWO9NNkvCrtLNu3f-pbmwsWntCxBjOE3d9OmqlG-t_Gwi6JOJQKQss9Lmfrq2kKq21azsgTweSuJugU7cbPBB49xG0_M__zPnBk2gQVipY6HYya2KdIuUqjfQ5Ivuo_HXkdwGo67f3pKblq3bBIbLC1NcV1hDYtXddSW53Q
:alt: image data
:width: 400
:align: center

이미지 제목을 넣어주세요. 
```


### 이미지 데이터 인식 
이제 컴퓨터에서 이미지 데이터가 어떻게 표현되고, 컴퓨터가 이를 어떻게 인식하는지 그 방법에 대해 알아보도록 하겠습니다. 

```{figure} https://lh6.googleusercontent.com/wNg0-aSKuhmrbaLdUMXq9I4YaqfHZUlNvTAkrKpkxwfzj6eTp-n2A659Q10XrD7GrCvf3xbGeZ-vZcqwTLVeqUL7NKPdCmh-dIablzb77JnvC_sSSsvB1r7WfCFIidFrUkiJBoomnDQapsprspTagTftHFquimlkNzpnGglwzuyb4OPoTVP4pdmj4VWhwk44i6gYhEMfww
:alt: image data
:width: 400
:align: center

이미지 제목을 넣어주세요. 
```

보통 이미지 데이터는 컴퓨터에서 특정한 사이즈를 가지는 2차원(평면)으로 표현됩니다. 위의 고양이 이미지를 (봐 삭제) 볼까요? 고양이 이미지를 보면 가로가 16 Pixels, 세로는 11 Pixels이라고 적혀 있습니다. 그럼 이 이미지 데이터의 사이즈는 16x11입니다. 그렇다면 어떤 이미지 데이터의 픽셀이 가로 128개, 세로 256개라면 이 이미지 데이터의 사이즈는 128x256이라고 할 수 있겠죠. 이처럼 이미지 데이터를 구성하고 있는 픽셀의 수에 따라 이미지는 컴퓨터에서 다양한 사이즈로 나타나게 됩니다.
컴퓨터가 이미지 데이터를 인식하기 위해서는 이미지 데이터를 디지털로 변환하는 작업이 필요합니다. 이미지를 데이터로 변환하는 방법(또는 이미지 데이터 변환 방법)이 여러 가지 있지만, 그 중 대표적인 방법인 gray scale 변환을 예로 들어보겠습니다. 
```{figure} https://lh5.googleusercontent.com/vNkRM3qTPQVBWbpPLXm2gqSMQTbc6_0Ir1EyICUn3XFI9E-hSYr_lm5ydjyY0syPwZFg_rZwwjIHHuf1CLboh5eqzk1Eig-ckF4PU2sRrX6xefN4JRY3-zHMchWxRG_n1jFoKkT5yPOkY48fxFd8TLyyZWk0U5vcw9mXqUYfFKqOeJtXTn0vu8p5WBkHgSApF6q_hXAsOw
:alt: image data
:width: 400
:align: center

이미지 제목을 넣어주세요. 
```

Gray scale은 흑백 이미지를 채도에 따라 0~255까지 총 256개의 단계로 나눠 숫자로 나타내는 방법입니다. 숫자가 커질수록 밝은색, 작아질수록 어두운색을 의미합니다. 예를 들어 숫자 0은 검정색, 255는 흰색을 의미합니다. 이렇게 수치화되어 있는 색상에 이미지 데이터의 각 픽셀의 색상과 매칭되는 값으로 변환되는 거죠. 
```{figure} https://lh4.googleusercontent.com/5czWHvgR-BCDOc4Rewo1LHTlj0DAW3x4hXDUIek-okFfKMMe8PDYmyeaX5QEiGQ6Bm85uga14Xp0zysAEA3wekRsVEkJcRKgwVqwccrT6ySlho3s5myFmRBzD6rbJod-wtpf83zcXNSbicKSvcyi7E0ekbQ5TdIZIx21O3W1D-WBhC8gDX2ii1WEvu74H5cRGJW_ceYYkA
:alt: image data
:width: 400
:align: center

이미지 제목을 넣어주세요. 
```


그래서 컴퓨터는 픽셀마다 변환된 숫자 데이터들을 통해 이미지를 인식하게 됩니다. 



### 컴퓨터가 이미지를 인식하기 어려운 이유
 컴퓨터와 사람은 이미지 데이터를 인식하는 데 큰 차이를 보입니다. 이를 Semantic gap이라고 부르는데, Andreas Hein은 이것을 "서로 다른 표현 시스템 내에서 형성된 구성 간의 의미 차이"로 정의했습니다. 다시 말하면 인간과 컴퓨터는 데이터를 인식하는 방식이 다르기 때문에 그 차이로 인해 인식하는 것이 달라질 수 있다는 말입니다.
사람이 이미지 데이터를 인식하는 과정이 무의식적으로 진행되기 때문에 컴퓨터가 이미지 데이터를 인식하는 과정 또한 간단할 것으로 생각할 수 있습니다. 하지만 컴퓨터는 이미지 데이터를 그 자체로 인식하지 않고, 하나의 이미지를 숫자로 인식하기 때문에 어려움이 있습니다.

```{figure} https://lh4.googleusercontent.com/qSDvtl8KBywyXVN9_TtNPkvdU2rDIWimAmv-KIl0jF3QC3pObV1IrKH5_boiMyToQqi1oJ3hEG1awKg-5RMlZ5tlupzsHkivOn52nT1zVoLTvHIJUkhUvrQLLBryIpkHxw8GJ6ABtW026-EM41CWnnZtCp9-XyGBTiRhwb9fZCa6XI1iY0h6UpvrPEBSfxH5FUi4Y1NgFA
:alt: image data
:width: 400
:align: center

이미지 제목을 넣어주세요. 
```

위의 그림에서 보면 고양이 몸통에 그려진 작은 네모 박스를 컴퓨터는 오른쪽과 같이 숫자 모음으로 표현했습니다. 그렇다면 고양이 전체를 파악하기 위해 컴퓨터는 얼마나 많은 데이터를 이해해야 할까요? 엄청난 데이터가 필요하다고 해요. 그리고 과연 컴퓨터는 한 장의 고양이 이미지 데이터로 고양이를 인식할 수 있을까요? 아니겠죠. 실제로 인공지능 역사에서 컴퓨터가 고양이를 인간만큼 인식하는데 1,000만 장의 이미지 데이터가 필요했다고 합니다. 이와 같이 컴퓨터가 사람처럼 이미지 데이터를 인식하기 위해서는 엄청난 데이터가 필요하고, 또 이를 이해해야 하므로 인식하는 데 어려움이 있습니다.


### 마무리 퀴즈
```{admonition} 픽셀 단위의 작은 이미지를 직사각 형태로 모아 놓은 것을 무엇이라고 할까요?
:class: tip dropdown

정답 : 이미지 데이터 
```


## 픽셀(Pixel)이란? 	
### 미술 작품 속 픽셀 

위 그림은 점묘화의 창시자 조르주 쇠라의 ‘Study for La Grande Jatte’라는 작품입니다. 여러분도 쇠라처럼 미술시간에 점묘화를 그려본 적이 있을텐데요. 점묘화는 선 대신 수 많은 점을 찍어 그린 그림입니다. 그런데 우리가 보는 핸드폰 혹은 태블릿과 같은 디스플레이 화면도 사실 점묘화와 같은 원리로 이미지를 표현한다는 것을 알고 있나요?  점을 하나하나 찍어 점묘화를 그렸다면, 컴퓨터는 디스플레이 화면에 ‘픽셀’이라는 점을 찍어 이미지를 완성합니다. 

### 픽셀의 정의
그렇다면 픽셀은 무엇일까요? 픽셀이란 디지털 기기에서 이미지를 구성하는 최소 단위를 뜻합니다. 아래의 사진을 확대해 봅시다. 

[픽셀로 만들어진 이미지 첨부 예정] 

그림을 계속 키워도 더 이상 늘어나지 않는 네모가 보이나요? 이렇게 이미지를 키웠을 때 더 이상 쪼개지지 않는 작은 네모를 픽셀이라고 합니다. ‘픽셀Pixel’은  사진을 뜻하는 'Picture'와 요소를 뜻하는 'Element'가 결합하여 만들어진 단어입니다. 우리는 픽셀보다 ‘핸드폰 카메라가 몇만 화소입니다’와 같이 ‘화소’란 말을  훨씬 많이 들어보았을텐데요.. 바로 이 ‘ 화소’가 영어로 하면 픽셀입니다.

### 픽셀과 해상도 
이미지는 픽셀 수에 따라 디스플레이 화면에서 얼마나 또렷하게 보일지 결정됩니다. 동일한 크기의 이미지여도 픽셀이 몇 개 있느냐에 따라 이미지의 선명도가 달라집니다.. 다시 말해 같은  공간 안에 픽셀이 많으면 많을수록 이미지는 더 또렷하게 보이는 것이죠.  아래 이미지를 볼까요?  

여러분은 오른쪽과 왼쪽 중 어느 쪽이  더 선명해보이나요?  왼쪽이 더 선명해보이죠. 왼쪽처럼 픽셀이 조밀하게 들어있으면 훨씬 선명하고 깨끗하게 이미지를 표현할 수 있습니다. 
이렇게 이미지가 화면에서 몇 개의 픽셀로 표현되는지(나타나는지)  알려주는 것을 해상도라고 하는데요. 이미지를 구성하는  픽셀의 크기가 작고, 개수가 많을수록 해상도가 높다고 하고, 픽셀의 크기가 크고 개수가 적을수록 해상도가 낮다고 합니다. 즉, 고해상도 이미지는 저해상도 이미지 보다 작고 조밀한 픽셀로 구성되어있기 때문에 더 선명한 이미지 표현이 가능합니다. 
해상도는 픽셀의 가로와 세로 구성에 따라 여러가지 규격으로 나뉩니다. TV에 보면 ‘UHD’, ‘Full HD’라고 쓰여 있는 것을 종종 볼 수 있는데요. HD는 High Definition의 줄임말로 우리말로 번역하면 ‘고화질’입니다.
UHD(Ultra High Definition, 초고화질)는 가로와 세로의 픽셀이 3840개와 2160개.  Full HD는 각각 1920개, 1080개로 이루어져있습니다.  가로와 세로의 픽셀 수를 곱해보면, 전체를 구성하는 픽셀의 개수를 알 수 있습니다. UHD는 8,294,400개의 픽셀로 Full HD는 2,073,600개의 픽셀로 구성되어 있습니다. 이를 대략적인 숫자로 바꾸어 800만 화소, 200만 화소라는 표현을 쓰기도 합니다. 더 다양한 규격은 아래 이미지를 통해 확인하세요.   


### PPI(Pixels Per Inch)
(앞에서 배운 내용(픽셀의 크기가 작고 개수가 많을수록 선명하다)을 1줄 정도로 요약 가능할까요? 그럼, 픽셀 수가 많으면 무조건 이미지가 선명하다고 할 수 있을까요? 정답은 NO! 아래 사진을 보겠습니다.

어떤 사진의 화질이 더 좋아 보이나요? 오른쪽? 왼쪽? 언뜻보면 양쪽 이미지의 화질이 비슷한 것 같은데요. 왼쪽 사진은 픽셀의 수가 100x100이고, 오른쪽은 150x150인 이미지입니다. 왼쪽 사진은 1만 화소, 오른쪽 사진은 이미지는 2.25만 화소로  표현할 수 있습니다. 왜 오른쪽 사진의 픽셀이 더 많은데 왼쪽 사진이  더 선명하게 보일까요? 아니면 픽셀의 수가 많다는 것을 알고부터는 갑자기 오른쪽이 더 선명해 보이나요? 어떤 이유에서(또는 무엇이 비슷해서) 두 사진의  해상도는 다르지만, 화질은 비슷해보일까요? 바로 픽셀 하나의 크기가 같기 때문입니다. 화질을 따질 때는 픽셀의 수도 중요하지만, 픽셀 하나의 크기도 중요합니다. 
픽셀 하나의 크기를 나타내기 위해 PPI라는 단위를 사용하는데요. PPI는 ‘Pixels Per Inch’의 줄임말로, 1인치당 픽셀이 몇 개 있는지를 의미합니다. 1인치당 픽셀 수가 많다면 픽셀 하나의 크기는 작을 것입니다. 

이미지의 사이즈가 같다면 픽셀이 많을수록 PPI도 클 것입니다. 위 이미지를 보면, 같은 사이즈의 이미지를  구성하는 픽셀의 수가 5x5에서 500x500으로 많아질수록 픽셀의 크기는 작아진 것을 알 수 있습니다. 
한편, 이미지를 구성하는 픽셀의 수는 같은데 사이즈만 점점 커진다면 픽셀의 크기는 커지고 PPI는 작아집니다.


PPI가 낮아질수록 우리는 ‘화면이 깨졌다'고 느끼게 되는 거죠. PPI를 직접 계산해 보고 싶다면 수치만 입력하면 자동으로 PPI가 계산되는 사이트에서 계산할 수 있습니다. 여러분의 컴퓨터, 핸드폰 환경설정에서 가로 세로 픽셀의 수와 함께 디스플레이 화면의 물리적 크기만 알면 PPI를  간단하게 구해볼 수 있습니다. 보통 72 PPI 정도면 화면에서 글씨가 깨지지 않고 적당히 잘 보인다고 합니다. 

### 마무리 퀴즈
```{admonition} 1인치에 몇 개의 픽셀이있는지 나타내는 단위는 무엇일까요? 
:class: tip dropdown

정답 : PPI
```