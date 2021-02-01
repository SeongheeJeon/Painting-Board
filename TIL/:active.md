
> ### 의사 클래스(pseudo-class) - 선택하고자 하는 HTML 요소의 특별한 '상태(state)'를 명시할 때 사용.
> 1. 동적 의사 클래스(dynamic pseudo-classes) - :link, :visited, :hover, :active, :focus
> 2. 상태 의사 클래스(UI element states pseudo-classes) - :checked, :enabled, :disabled
> 3. 구조 의사 클래스(structural pseudo-classes) - :first-child, :nth-child, :first-of-type, :nth-of-type
> 4. 기타 의사 클래스- :not, :lang


# :active


 사용자가 활성화한 요소. 마우스를 사용하는 경우 "활성"이란 보통 마우스 버튼을 클릭한 순간부터 떼는 시점까지.

```css
.controls__btns button:active {
  transform: scale(0.98);
}
```

→ 대개 ```<a>```, ```<button>```와 함께 사용. 

→ active 의사클래스 뒤에 :link, :hover, :visited를 사용하면 덮어씌워짐. 링크를 적절히 디자인 하려면 :active 규칙을 다른 링크 규칙들보다 뒤에 배치할것. LVHA-순서(:link — :visited — :hover — :active)

→ label에 active가 적용될경우 그와 연결된 요소에도 같이 적용됨.

```html
<form>
  <label for="my-button">내 버튼: </label>
  <button id="my-button" type="button">제 라벨이나 저를 클릭해보세요!</button>
</form>
```

```css
form :active {
  color: red;
}

form button {
  background: white;
}
```

([참고-MDN](https://developer.mozilla.org/ko/docs/Web/CSS/:active))
