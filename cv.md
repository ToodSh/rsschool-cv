# rsschool-cv

## Oleg Shalamai

#### Contacts:
- Telegram: @bear_web
- E-mail: toddchaves010@gmail.com
- Linkedin: linkedin.com/in/oleg-shalamai-4601bb265
- Discord: Shalamai Oleg (ToodSh)

#### About me
I'm HTML developer. I'd like to be frontend developer and get more money :)

#### My skills
- HTML
- CSS
- JS 
- VUE
- PHP
- Figma
- Photoshop
- Git
- БЕМ

#### Code example
```js
const checkCorrectNumber = (value) => {
  if (!Number.isFinite(value)) {
    throw new RangeError('Числа должны быть положительными или 0.');
  }

  if (value < 0) {
    return 0;
  }

  if (value > Number.MAX_SAFE_INTEGER) {
    return Number.MAX_SAFE_INTEGER;
  }

  return value;
};

const getRandomNumber = (minNum = 0, maxNum = Number.MAX_SAFE_INTEGER, accuracy = 0) => {
  let minCheckedNum = checkCorrectNumber(minNum);
  let maxCheckedNum = checkCorrectNumber(maxNum);
  const checkedAccuracy = checkCorrectNumber(accuracy);

  [minCheckedNum, maxCheckedNum] = minCheckedNum > maxCheckedNum ? [maxCheckedNum, minCheckedNum] : [minCheckedNum, maxCheckedNum];

  const diff = maxCheckedNum - minCheckedNum;
  const random = Math.random() * 1.000000000000001; // чтобы могла выпасть единица
  const factor = Math.pow(10, checkedAccuracy);

  return Math.round((random * diff + minCheckedNum) * factor) / factor;
};

const getRandomUnsignedInteger = (minNum = 0, maxNum = Number.MAX_SAFE_INTEGER) => getRandomNumber(minNum, maxNum);

const getRandomUnsignedFloat = (minNum = 0, maxNum = Number.MAX_SAFE_INTEGER, accuracy = 0) => getRandomNumber(minNum, maxNum, accuracy);

const checkArrayEmpty = (array) => {
  if (array) {
    if (array.length) {
      return true;
    }
  }
  return false;
};

export {
  getRandomUnsignedInteger,
  getRandomUnsignedFloat,
  checkArrayEmpty,
};

```
#### Experience
- Gold Fusion
- Freelance

#### Courses 
- HTML academy: https://htmlacademy.ru/intensive/javascript

#### About my english
I have a low level english. I think about elementary +. I have a little english practice every day and I learn english lessons 2 times in a week :) 

