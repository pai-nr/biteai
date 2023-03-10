% Source : https://docs.google.com/document/d/e/2PACX-1vTNQr4yY6v_LxUiLLae2JJtXk_6divBtn7-S_e4JPhRNnB2XxvkZxnvaCVEukXdy6-WL5y0esmsAoa0/pub

# RGB란? 	
## 빛의 삼원색
```{figure} https://lh6.googleusercontent.com/ivEXfTl5vgA0Zuo7aOaGDlsTEpzWjazC6lsdlopRsneRXf6zssmD7fic32P5chth1hMn4WQzZHxZgWn53Hqdeme4FpIXOjldN6gPMh7EcnAjsxMUZBWG9g-RDiMbio-M-cLMNdfbzuTa6T5TNLP1csd8DFnpb6zqJl6lAvs5Bf4AhSVtr3_GgLvrzwsK8w
:alt: rgb
:width: 400
:align: center

이미지 제목을 넣어주세요. 
```
여러분은 ‘빛’이라고 하면 어떤 색이 떠오르나요? 아마 대부분 흰색을 떠올렸을 텐데요. 빛의 깨끗하고 투명해서 ‘흰색’을  색 하나로 만들어진 단일 색이라고 생각하기 쉽지만, 사실 우리가 흰색 빛으로 알고 있는 백색광은 여러 빛이 더해져/합쳐져  만들어진 합성광입니다. 과학 시간에 이것을 확인하기 위해 프리즘을 이용하여 빛을 통과시키는 실험을 해보았을거예요. 강렬한 백색광인 햇빛(태양빛)을 프리즘에 통과시켰더니 알록달록 예쁜 일곱 가지 무지개색의  스펙트럼으로 분산되어 나타났다가 빼면 다시 합치니 흰색으로 돌아오지 않았나요.
다양한 색을 가진 빛들이 합쳐져 백색광이 되는 것처럼 두 가지 이상의 빛이  섞여 다른 색이 되는 현상을  빛의 합성이라고 합니다. 빛의 합성 원리를 활용하면 여러 빛깔을 표현할 수 있습니다. 미술 시간에 모든 색을 만들 수 있는'색의 삼원색', 빨강, 파랑, 노랑이 있듯이 빛에서도 모든 색을 만들 수 있는 '빛의 삼원색'이 존재합니다. 바로 빨강, 초록, 파랑인데요. 이 세 가지 색의 빛은  어떤 색의 빛을 섞어도 만들 수 없기에 ‘삼원색’으로 불리며,  삼원색의 빛을 여러 비율로 배합하면 세상의 모든 색의 빛을 만들 수 있습니다.  

## RGB의 정의
앞서 빛의 삼원색을 빨강, 초록, 파랑이라고 했죠.  RGB는 이 세 가지 색 ‘Red’,  ‘Green’, ‘Blue’의  앞 글자를 따서 만든 것입니다. . 즉 ‘RGB’는 빛의 삼원색이자 오늘날에는 그 의미가 더 확장되어 ‘디지털 이미지에서 색을 표현하는 하나의 방식’을 의미하기도 합니다.  

```{figure} https://lh4.googleusercontent.com/v-fYT_sBCuq_92UjtfibG9OhyECT5ZmTSdokNUozxKQg2FNj5jn1CDoxRjbdaSzDeY8MAzPBUD3mpmv0ntWnLFbNIEaA-1dua1okRVUbnSYrmyNQJxBEdFIlb_ENVy5eO_7JgsXBlrkOAXUr-y9d7yoSQDvmCdOGjeH6-KCx4BauHExRtoZSkYujvyWtmQ
:alt: rgb
:width: 400
:align: center

이미지 제목을 넣어주세요. 
```

RGB가 빛의 삼원색이라는 것은 알겠는데,  디지털 이미지에서 RGB로 색을 표현한다는 것은 어떤 의미일까요? 우리는 눈에  보이는 색을 개인마다 다르게 표현하곤 합니다. 누구는 개나리를 보고 ‘노랗다’고 하고, 또 누구는 ‘샛노랗다'고 할 것입니다. 그리고  개화시기에 따라 개나리의 색도 바뀌기  때문에 개나리를 표현하는노란색도 그 스펙트럼이 넓다고 할 수 있겠네요. 
하나의 색도 넓은 스펙트럼을 가질 수 있는 것처럼  복잡한 현실 세계의 다양한 색을 디지털 이미지로 변환하려면 어떤 기준이 필요할 수밖에 없습니다. 예를 들어 컴퓨터에서 노르스름한 색의 값은  136, 누르스름한 색은 82로 정하는 약속 같은게  필요한거죠. 이처럼 디지털 이미지를 표현하기 위해 색깔을 숫자들의 조합으로  지정해둔 것을 ‘색상코드’라하고,  RGB는 디지털 이미지를 표현하는데 사용되는 여러 가지 색상코드 중 하나입니다.  

## 전자제품 화면에서의 색깔 표현
우리가 자주 사용하는 핸드폰, 컴퓨터와 같은 전자제품의 화면은 RGB 색 모델을 활용해 색깔을 표현하는데요. 디지털 이미지는 픽셀 단위의 작은 이미지들의 모음이라고 들어본 적 있을 겁니다. 디지털 이미지를 이루는  픽셀 뒤에는 백라이트(backlight)라는 태양과 같이 빛을 내는 광원이 존재하고, 이 광원이 픽셀마다 들어있는 빨강, 초록, 파랑의 양과 색을 조합하여 마치 빛의 삼원색의 조합으로 여러 가지 색을 나타낼 수 있는 것처럼 다양한 색을 연출할 수 있습니다. 이런 아이디어가 없었다면 우리는 아마 1980년대 어른들이 보았던 흑백티비처럼 색깔없이 단조로운 컴퓨터, 핸드폰 화면만 보았을 것입니다. 
그럼, RGB를 디지털 숫자로 어떻게 표현하는지 한번 확인해볼까요? 먼저, RGB로 표현할 수 있는 대표적인 색부터 숫자 코드로 어떻게 나타내는지 알아봅시다. 아래 이미지를 천천히 살펴보세요. 총  몇 개의 색이 보이나요?  
```{figure} https://lh5.googleusercontent.com/aL2V4iWQ4s1abvtF8PKXyS0OXA5DfkoQbiwePyKH0JZ2jkoBR5e_92f6grfUHZFpZBqa3PHT6d7OwI8yvVGGXDA6-B-iB1ZR7UemRNNAR7z-c7-VZvg8zP5zUc3xq4tEmCW9na1qUbV5UGTA5VQGVtCCRcV69ya7SfTVbSfxWG3wWP-mZUXuCqV9JDztgQ
:alt: rgb 
:width: 400
:align: center

이미지 제목을 넣어주세요. 
```
혹시 7개라고 생각했나요? 정답은 8개입니다. 빨강, 노랑, 초록, 하늘, 파랑, 보라, 흰색 그리고 나머지하나는 무슨 색일까요? 바로 검은색입니다. RGB 중 어떤 색도 비추지 않으면 검은색이 되고. 단순한 색을 겹치는 것만으로도 8개의 색을 나타낼 수 있습니다. 위  8개의 색을 색상코드 즉, 숫자 조합으로 나타내면 아래와 같습니다. 
(000, 000, 000)
(255, 255, 255)
(255,  000, 000)
(000, 255, 000)
(000, 000, 255)
(255, 255, 000)
(000, 255, 255)
(255, 000, 255)

1번부터 8번은 각각  어떤 색을 표현하는 것일까요? 그 비밀을 풀 수 있는 열쇠는 잠시 후 알려드릴게요. 힌트를  드리자면 괄호 안에 적혀있는 세 개의 숫자 조합은순서대로 R, G, B를 뜻합니다. 우리는 RGB를 나타내는  세 숫자의 조합을 통해  디지털 기기에서 다양한 색을 표현할 수 있습니다. 어떻게 숫자 조합으로 색을 표현할  수 있을까요? 그리고 이 숫자 조합으로 몇 가지 색을표현할 수 있을까요?
디지털 이미지를 구성하는  픽셀은  빨강, 초록, 파랑 세 가지의 서브픽셀로 이루어져 있습니다. 그리고 이 서브픽셀들은 각각의 색을 256개의 단계로 표현할 수 있습니다. 그래서 한 픽셀이 나타낼 수 있는 색은 빨강의 채도별 색깔의 개수 256개 x 초록의 채도별 색깔의 개수 256개 x 파랑의 채도별 색깔의 개수 256개로 총 16,777,216가지입니다. 그래서 위 숫자 코드에 000과 255가 있었던 것입니다. 256가지 채도를 000부터 255라는 숫자로 표현한 것이죠. 
```{figure} https://lh6.googleusercontent.com/cGMfDlxzB5y8LqNDMyPtzwbnaVoTaxftXthrltCpBBRm_VXiOC6FpMCqc_M3exF5Ztd_-Fc5OczMRMtlShD_S77UVmyeiKjn6xgF22xixAlQf0zKSbpZ_Mw4RctWnLkXJuA0JNzxu149aWVptKXDd66McpK6_GhMA_xpw5YhRExfgK8Zl9-s4GAW9Y_4rQ
:alt: rgb
:width: 400
:align: center

이미지 제목을 넣어주세요. 
```



더 자세히 살펴볼까요? 위 그림에서 검은색은 R=000, G=000, B=000으로 표기되어 있는데요, 즉, 빨강, 초록, 파랑이 하나도 들어있지 않다는 것을 의미합니다. 빛의 삼원색이 모두 비치지 않으면 검은색이 된다는 것을 떠올리면 검은색을 나타내는 서브픽셀들의 값이 왜 모두 000인지 이해할 수 있을거예요. 이제 앞서 본  8가지 숫자 코드 중, 1번(000, 000, 000)은 검은색인 것을 알 수 있습니다. 만약 R=255이고, G=255, B=153이라면 무슨 색일까요? 빨간색과 초록색이 듬뿍 들어있고, 파란색은 약간 덜 들어있는 색깔이 될 텐데요. 이 색은 바로 위 그림에서 FFFF99로 표기된  연한 노란색입니다.

여기 [RGB의 각 값을 입력하면 어떤 색이 되는지 알 수 있는 사이트](https://www.rapidtables.org/ko/web/color/RGB_Color.html)가 있습니다. 앞서 본 8가지 숫자 코드를 각각 R, G, B 칸에 입력하여 각 코드가 어떤 색을 나타내는지 그 비밀을 풀어보세요. 빨강, 파랑, 초록이나 내가 좋아하는 색을 만들 수 있는 RGB 값의 조합이 무엇인지 찾아보면 재밌을 거예요.



## 마무리 퀴즈
```{admonition} RGB로 컴퓨터 화면의 색을 표현하기 위해 하나의 픽셀은 몇 개의 서브 픽셀로 나누어지나요? 
:class: tip dropdown

정답 : 3개
```