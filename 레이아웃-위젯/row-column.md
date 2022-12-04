# Row, Column

## 개념 요약

Row와 Column은 Flutter가 제공하는 기본 레이아웃 위젯입니다.

여기에는 Flex 레이아웃 모델이 적용돼 있어 이를 이해하고 사용하면 좋습니다.

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption><p>W3C, Flex Box 모델 개념 및 용어, <a href="https://www.w3.org/TR/css-flexbox-1/#box-model">https://www.w3.org/TR/css-flexbox-1/#box-model</a></p></figcaption></figure>

## 특징

### Row

1. Row의 높이 = 자식 위젯의 높이

### Column

1. Column의 너비 = 자식 위젯의 너비

## 정렬 방식

|           속성명          | Row | Column |
| :--------------------: | :-: | :----: |
|  **MainAxisAlignment** | 가로축 |   세로축  |
| **CrossAxisAlignment** | 세로축 |   가로축  |

{% hint style="success" %}
**MainAxisAlignment 정렬 옵션**

1. start
2. center
3. end
4. **spaceEvenly** : 간격을 똑같이 나눕니다. 양끝에도 똑같은 간격이 들어갑니다.
5. **spaceBetween** : 간격을 똑같이 나눕니다. 양끝 간격이 없습니다.
6. **spaceAround** : 간격을 똑같이 나눕니다. 양끝에 절반 크기의 간격이 생깁니다.
{% endhint %}

{% hint style="info" %}
**CrossAxisAlignment 정렬 옵션**

1. start
2. center
3. end
4. **stretch** : 요소를 좌우로 늘립니다.
5. **baseline** : 글자의 가로(세로) 베이스라인을 기준으로 정렬합니다.
{% endhint %}
