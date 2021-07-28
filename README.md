# chojungjong
한글 초성, 중성, 종성 분리

## Copyright
©️ 2021 Sanha, all rights reserved.

## License
소스코드 파일에 표기되어있음.

## How to Use

### Get Started
```javascript
const cjj = require(PATH);
```

### separate(letter: string)
한글 한 글자를 매개변수로 받아서 초성, 중성, 종성으로 분리한 배열을 리턴.

```javascript
cjj.separate('와'); // [ "ㅇ", "ㅗ", "ㅏ" ]
cjj.separate('우'); // [ "ㅇ", "ㅜ", "" ]
```

응용: 한 글자 이상 한번에 분리하기

```javascript
'반가워'.split('').map(el => separate(el));
// [ [ "ㅂ", "ㅏ", "ㄴ" ], [ "ㄱ", "ㅏ", "" ], [ "ㅇ", "ㅝ", "" ] ]
```

