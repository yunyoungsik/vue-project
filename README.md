# vue를 이용한 사이트 만들기

Vue.js는 현대적인 웹 애플리케이션을 만들기 위한 프로그레시브 프레임워크입니다. Vue.js는 사용자 인터페이스를 만들기 위한 라이브러리이며, 웹 애플리케이션의 화면을 동적으로 업데이트하고 상태를 관리하는 데 사용됩니다.

Vue.js는 선언적이고 간단한 구문을 가지고 있어 쉽게 배우고 사용할 수 있습니다. 또한, 다른 프로젝트에도 적용하기 쉽습니다. Vue.js는 컴포넌트 기반 아키텍처를 기반으로 하며, 재사용 가능한 UI 요소를 만들고 조합하여 애플리케이션을 구성할 수 있습니다.

Vue.js의 주요 특징은 다음과 같습니다:
<details>
<summary>더보기</summary>

1.  반응성 (Reactivity): Vue.js는 데이터의 변화에 반응하여 화면을 자동으로 업데이트합니다. 데이터가 변경되면 해당 부분만 다시 렌더링되어 사용자 경험이 향상됩니다.
   
2. 컴포넌트 기반 설계 (Component-Based Architecture): Vue.js는 애플리케이션을 작은 컴포넌트로 나누어 개발할 수 있게 해줍니다. 각 컴포넌트는 자체적으로 상태와 뷰를 가질 수 있으며, 재사용이 가능합니다.
   
3. 가상 DOM (Virtual DOM): Vue.js는 가상 DOM을 사용하여 화면을 빠르게 업데이트합니다. 가상 DOM은 실제 DOM과 동기화되지 않고, 필요한 경우에만 실제 DOM에 업데이트를 적용합니다.
   
4. 단방향 데이터 바인딩 (One-Way Data Binding): Vue.js에서는 부모 컴포넌트에서 자식 컴포넌트로 데이터를 전달할 수 있지만, 자식 컴포넌트에서 부모 컴포넌트의 데이터를 직접 변경할 수는 없습니다. 이로써 데이터의 흐름이 예측 가능해집니다.
   
5. 이벤트 핸들링 (Event Handling): Vue.js는 이벤트 처리를 쉽게 할 수 있는 방법을 제공합니다. 이벤트를 감지하고 처리할 수 있는 기능을 제공합니다.
   
6. 라우팅 (Routing): Vue.js는 Vue Router를 통해 싱글 페이지 애플리케이션(SPA)의 라우팅을 관리할 수 있습니다.
   
7. 상태 관리 (State Management): Vue.js 애플리케이션에서 중앙 집중식 상태 관리를 위해 Vuex라는 라이브러리를 사용할 수 있습니다.
   
또한, Vue.js는 확장성이 뛰어나며 다른 라이브러리나 프레임워크와도 쉽게 통합됩니다. 개발자들은 필요에 따라 기존 프로젝트에 Vue.js를 추가하거나, Vue.js를 사용하여 새로운 프로젝트를 시작할 수 있습니다.
</details>

## 셋팅
`npm install`
√ Project name: ... vue-project
√ Add TypeScript? ... <span style="color.blue">No</span> / Yes
√ Add JSX Support? ... No /<span style="color.blue">Yes</span>
√ Add Vue Router for Single Page Application development? ... No / <span style="color.blue">Yes</span>
√ Add Pinia for state management? ... <span style="color.blue">No</span> / Yes
√ Add Vitest for Unit Testing? ... <span style="color.blue">No</span> / Yes
√ Add an End-to-End Testing Solution? » <span style="color.">No</span>
√ Add Prettier for code formatting? ... No / <span style="color.">Yes</span>