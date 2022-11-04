#Super Converter Project (useState, Set 사용하여 단위 변환기 만들기)

What I learned...

1. React.JS는 엔진과 같은 역할 즉, interactive한 ui 만들수 있게 함.
2. react-dom은 리액트 요소들을 html에 넣어주는 역할수행.
3. react application은 한번에 하나의 component만 rendering 가능함.
4. JSX 사용하여 CreateElement 대체=> 효율성 올라감.
   </br>
   이 과정에서 Babel 코드변환 이용
5. React.JS는 렌더링할때 ui에서 바뀐부분만 업데이트 함으로써 코드 효율성 증대.
6. useState를 이용해서 자동으로 렌더링 가능하게 하여 코드를 간결하게 할 수 있음.
7. Props => 부모 컴포넌트들로부터 자식 컴포넌트에 데이터를 보낼 수 있게 해주는 방법.
8. 밑 예시 코드처럼 React.memo 사용하면 컴포넌트들이 다시 그려질때 다시 그릴 필요 없는건 안바꿈.
   </br>
   // const MemorizedBtn = React.memo(Btn);
9. proptypes를 통해 prop에 적절한 타입을 적용하였는지 테스트 가능. (console창 경고메시지로 확인 가능.) 단, TypeScript 사용시에는 불필요.

#state 셋팅 과정에 관한 학습

1.  직접 값 설정하기.
    </br>
    // setCounter(5);
2.  밑 예시 코드처럼 현재 state 바탕으로 다음 state 계산해보고 싶으면 current 이용, 또한 setCounter 사용하여 자동으로 렌더링 가능.
    </br>
    // function App() {
    const [counter, setCounter] = React.useState(0);
    const onClick = () => {
    setCounter((current) => current + 1);
    };

프로젝트 설명: Minutes to hours converter 미니 프로젝트에서 힌트를 얻어 useState 활용하여 Km to miles converter 기능을 추가로 구현하였습니다.
