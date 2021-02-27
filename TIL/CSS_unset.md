
# 'unset' at CSS [(MDN-unset)](https://developer.mozilla.org/ko/docs/Web/CSS/unset)

- `unset` : 부모로부터 상속할 값이 존재하면 상속값을, 그렇지 않다면 초깃값을 사용함.  


    > 즉, 전자일 땐 inherit, 후자일 땐 **initial 키워드**처럼 동작.
    
- 초기값은 css 자체에 기본 속성으로 설정되있음(MDN에 initial value라고 되어있음.) 


    > 브라우저가 정하는 속성은 'user agent style' 임. ([참고](https://elad.medium.com/understanding-the-initial-inherit-and-unset-css-keywords-2d70b7121695))  
    > [MDN(CSS-initial)](https://developer.mozilla.org/ko/docs/Web/CSS/initial) 에 초기값을 브라우저가 정한다고 잘못? 번역돼있음


- **initial 키워드** 예시

    ```jsx
    <p>
      <span>This text is red.</span>
      <em>This text is in the initial color (typically black).</em>
      <span>This is red again.</span>
    </p>
    ```

    ```css
    p {
      color: red;
    }

    em {
      color: initial;
    }
    ```

  <결과 이미지>  
  ![image](https://user-images.githubusercontent.com/49744535/109388037-0bf2cd80-7948-11eb-9fdd-7556cd2f02b0.png)


- 브라우저에서 설정해둔 것들을 초기화 시킬 때 사용할 수 있음.
