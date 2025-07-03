# **1. Math 프로퍼티**

1. **Math.PI**

   원주율 π (3.141592653589793)를 나타낸다.

   ```jsx
   const radius = 3
   const circleArea = Math.PI * radius ** 2
   ```

# 2. Math 메서드

1. **Math.abs(value)**

   절대값을 반환한다.

   숫자로 변환 불가능한 값은 NaN 반환!

   ```jsx
   Math.abs(-10) // 10
   Math.abs('5') // 5
   Math.abs('hello') // NaN
   ```

2. **Math.round(value)**

   소수 첫째 자리에서 반올림한다.

   ```jsx
   Math.round(4.6) // 5
   Math.round(4.4) // 4
   ```

3. **Math.ceil(value)**

   소수점 올림을 수행한다.

   ```jsx
   Math.ceil(4.1) // 5
   Math.ceil(-4.1) // -4
   ```

4. **Math.floor(value)**

   소수점 내림을 수행한다.

   ```jsx
   Math.floor(4.9) // 4
   Math.floor(-4.9) // -5
   ```

5. **Math.sqrt(value)**

   제곱근을 반환한다.

   음수 입력시 NaN을 뱉는다.

   ```jsx
   Math.sqrt(9) // 3
   Math.sqrt(-1) // NaN
   ```

6. **Math.random()**

   `0 ≤ x < 1` 범위의 난수를 반환한다.

   ```jsx
   // 1~10 정수 난수
   Math.floor(Math.random() * 10) + 1
   ```

   다만,,, 보안에 적합하지 않아서 보안용 랜덤은 `crypto.getRandomValues()`를 사용해야 한다.

> 🥲 **`Math.round()`랑 `Math.ceil()`의 차이점이 뭐냠?**
>
> > 1.  `Math.round()`는
> >
> >     0.5를 기준으로 반올림을 수행하고
> >
> > 2.  `Math.ceil()`은
> >
> >     무조건 올린다.

1. **Math.pow(base, exponent)**

   거듭제곱을 반환한다.

   ES7의 `**`로 대신할 수도 있다.

   ```jsx
   Math.pow(2, 3) // 8
   2 ** 3 // 8
   ```

2. **Math.max(…args)**

   가장 큰 수를 반환한다.

   ```jsx
   Math.max(...[1, 3, 2]) // 3
   ```

3. **Math.min(…args)**

   가장 작은 수를 반환한다.

   ```jsx
   Math.min(...[1, 3, 2]) // 1
   ```
