% 제목 MyST 스타일로 넣는 방법 확인해야 함
% 태그 키워드 추가하기 

# 컴퓨터가 이미지를 디지털로 인식하는 방법
```{figure} https://lh4.googleusercontent.com/3-rC8LGzAFQ5AxBdzZV4xfkfZuuGXfOwWEDkoVXdQn1io7_EFznhNDclP3wrH5tnOdVkdDwIBlyTw_Ng2aaEd16MToCKXGfkg6AM9LcemeIQwpEiPIJdTvaS7Xq-m__lfuwGXoAjMsQgUm87fRisK6Sj3NkPG5GoLNzb9ntf7mZ3vpak7Vdyb5QZFYiG6x-SWCJYrnjaQg
:alt: cat-01
:width: 400
:align: center

이미지 제목을 넣어주세요. 
```

위에 하나의 이미지([](#cat-01))가 있습니다. 제시된 이미지가 무엇으로 보이나요? 아마 많은 분이 자신 있게 고양이라 말할 것입니다. 우리 인간은 이 이미지를 보고 바로 ‘고양이'라고 이야기하지만, 컴퓨터도 인간과 마찬가지로 한 번에 고양이로 알아볼 수 있을까요? 어렵습니다. 그렇다면 과연 컴퓨터는 어떻게 이미지를 (보고 삭제) 인식하는지 알아보도록 합시다. 그러기 위해 먼저 사람이 판단한 ‘고양이’라는 표현 대신 ‘이미지 데이터’라고 불러보죠.

## 이미지 데이터란?
이미지 데이터는 디지털로 이미지를 구성하는 최소 단위인 픽셀(Pixel)들의 집합을 의미합니다. 너무 말이 어렵다고요? 미술 시간에 모자이크했던 것을 떠올려 봅시다. 모자이크 작품을 어떻게 만들었나요? 아마 여러분은 색종이를 찢고, 그 조각을 모아 붙여 하나의 큰 그림을 완성했을 것입니다. 찢긴 색종이 조각이 픽셀이고, 완성된 모자이크 작품이 이미지 데이터라고 보면 됩니다. 이처럼 이미지 데이터는 픽셀 단위의 작은 이미지들을 모아서 완성한 하나의 그림이라고 할 수 있습니다.  


```{figure} https://lh5.googleusercontent.com/iNWx1HD5aM_HISesOGJSjSvIGBK8-4aHN6dNWO9NNkvCrtLNu3f-pbmwsWntCxBjOE3d9OmqlG-t_Gwi6JOJQKQss9Lmfrq2kKq21azsgTweSuJugU7cbPBB49xG0_M__zPnBk2gQVipY6HYya2KdIuUqjfQ5Ivuo_HXkdwGo67f3pKblq3bBIbLC1NcV1hDYtXddSW53Q
:alt: image data
:width: 400
:align: center

이미지 제목을 넣어주세요. 
```


## 이미지 데이터 인식 
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



## 컴퓨터가 이미지를 인식하기 어려운 이유
 컴퓨터와 사람은 이미지 데이터를 인식하는 데 큰 차이를 보입니다. 이를 Semantic gap이라고 부르는데, Andreas Hein은 이것을 "서로 다른 표현 시스템 내에서 형성된 구성 간의 의미 차이"로 정의했습니다. 다시 말하면 인간과 컴퓨터는 데이터를 인식하는 방식이 다르기 때문에 그 차이로 인해 인식하는 것이 달라질 수 있다는 말입니다.
사람이 이미지 데이터를 인식하는 과정이 무의식적으로 진행되기 때문에 컴퓨터가 이미지 데이터를 인식하는 과정 또한 간단할 것으로 생각할 수 있습니다. 하지만 컴퓨터는 이미지 데이터를 그 자체로 인식하지 않고, 하나의 이미지를 숫자로 인식하기 때문에 어려움이 있습니다.

```{figure} https://lh4.googleusercontent.com/qSDvtl8KBywyXVN9_TtNPkvdU2rDIWimAmv-KIl0jF3QC3pObV1IrKH5_boiMyToQqi1oJ3hEG1awKg-5RMlZ5tlupzsHkivOn52nT1zVoLTvHIJUkhUvrQLLBryIpkHxw8GJ6ABtW026-EM41CWnnZtCp9-XyGBTiRhwb9fZCa6XI1iY0h6UpvrPEBSfxH5FUi4Y1NgFA
:alt: image data
:width: 400
:align: center

이미지 제목을 넣어주세요. 
```

위의 그림에서 보면 고양이 몸통에 그려진 작은 네모 박스를 컴퓨터는 오른쪽과 같이 숫자 모음으로 표현했습니다. 그렇다면 고양이 전체를 파악하기 위해 컴퓨터는 얼마나 많은 데이터를 이해해야 할까요? 엄청난 데이터가 필요하다고 해요. 그리고 과연 컴퓨터는 한 장의 고양이 이미지 데이터로 고양이를 인식할 수 있을까요? 아니겠죠. 실제로 인공지능 역사에서 컴퓨터가 고양이를 인간만큼 인식하는데 1,000만 장의 이미지 데이터가 필요했다고 합니다. 이와 같이 컴퓨터가 사람처럼 이미지 데이터를 인식하기 위해서는 엄청난 데이터가 필요하고, 또 이를 이해해야 하므로 인식하는 데 어려움이 있습니다.


## 마무리 퀴즈
```{admonition} 픽셀 단위의 작은 이미지를 직사각 형태로 모아 놓은 것을 무엇이라고 할까요?
:class: tip dropdown

정답 : 이미지 데이터 
```