# Todo List

- **리스트 추가, 진행중-완료 표시, 삭제 기능을 담은 Todo List입니다.**

---

## Components

### Todo.jsx

- 각각의 할 일 항목(Todo)을 렌더링하는 역할.
- props로 받은 할 일 항목 정보를 화면에 출력하고, 완료 및 삭제 버튼의 이벤트 핸들러 함수도 받아서 처리.
- Todo 항목의 제목(title), 내용(body)과 완료 여부(isDone) 정보를 출력하고, 완료/취소 버튼과 삭제 버튼이 함께 제공.

### WorkingSpace.jsx

- 작업 중인 할 일 항목들을 보여주는 역할.
- **todo** props로 전달된 할 일 항목들 중에서 **isDone** 값이 **false**인 항목들만 필터링해서, **`Todo`**컴포넌트로 전달하여 각 항목을 렌더링.

### DoneSpace.jsx

- **todo**배열에서 **isDone**값이 **true**인 항목들만을 필터링하여, **Todo**컴포넌트를 이용해 각각의 완료된 항목을 보여줌.
