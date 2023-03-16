### 명시적 문자열

파이썬은 명시적인 언어이다.

food = "steak"
변수 지정이 간편하다.  
human = "i\`m human" // 백슬래쉬 => ‘

줄바꾸기도 지원

```

food ="steak\ngood"
```

하지만 위 줄바꾸기는 코드가 명시적이지 않다.
그래서 """, '''를 통한 줄바꿈을 사용하기도 한다.

```
food ="""

food

good

"""
```

또는

```
food =‘’’

food

good

‘’’
```

### 문자열 인덱싱

문자열은 자동 인덱싱이 된다.

```

a = "Life is too short, You need Python"

a[0]

‘L’

```

파이썬의 특이한 점은 음수 인덱싱도 지원한다는 것이다.
원리는 문자를 처음 인덱싱할 때 한 문자에게 양수와 음수를 함께 인덱싱

```

a[-1]

’n’

```

또한 인덱싱된 문자를 따로 합성하여 새로운 문자열 생성 가능하다

```

b = a[0] + a[1] + a[2]

b

‘Lif’

```

또는 문자열 슬라이싱를 활용하여 문자열을 생성할 수 있다.

```

b = a[0:3]

b = a[:3]

b = a[0:]

```

### 문자열 포매팅

포매팅을 통해 문자열 자체의 변수를 넣어둘 수 있다.

```

a = "I eat %d apples."

print(a%5)

"I eat {0} apples".format(3)

```

이를 통해 정수나 문자에 한하지 않고 여러 타입을 포매팅할 수 있다.

심지어 다중 포매팅도 가능하다.

```

number = 10

day = "three"

I ate {0} apples. so I was sick for {1} days.".format(number, day)

'I ate 10 apples. so I was sick for three days.'

```

### 문자열 정렬과 공백

```

%10s => 오른쪽 정렬, 나머지 10개의 공백

%-10s => 왼쪽 정렬, 나머지 10개 공백

```

### 소수점 표현

```

"%0.4f" % 3.42134234

'3.4213'
```

### 문자열 관련함수

```

a.count()
a.find()
a.index()

```

cou
find와 index는 차이점 : index는 존재하지 않는 문자를 찾으면 오류가 발생한다는 점이다.

```

join => ",".join(abcd)

```

abcd 문자열 내 각각의 문자 사이 ‘,’를 집어넣기

```

lower, upper 대문자, 소문자 변환 함수

lstrip, rstrip, strip => 공백 제거 함수

replace => 문자 대체 함수

```

```

split => 문자열을 어떤 기준으로 나누기

a.split("어떤기준")

```
