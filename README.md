  <h1>다이어트 체중계</h1>
  
    <p>당신의 건강 몸무게를 알아보세요!</p>
    <ul>
        <li>현재 키 : <span class="height"></span>cm</li>
        <li>현재 몸무게 : <span class="weight"></span>kg</li>
        <li>목표 몸무게 : <span class="normal"></span>kg</li>
        <li>최종 감량 목표 : <span class="weight2"></span>kg</li>
        
        
---


//계산식) 적정체중 - (본인신장-100)*0.9
//변수명 예) userHeight, UserWeight, normal_w
//prompt 현재 키,몸무게 입력받기
//DOM객체 변수 생성하기

//1.Prompt 현재 키, 몸무게 입력받기
let userHeight = window.prompt ('현재 키를 입력하세요.') <br>
let userWeight = window.prompt ('현재 몸무게를 입력하세요.')
let normal_w = (userHeight-100)*0.9
let result = userWeight-normal_w

//2.Dom객체 변수 생성하기
const span_height = document.getElementsByClassName('height')[0]
const span_weight = document.getElementsByClassName('weight')[0]
const span_normal = document.getElementsByClassName('normal')[0]
const span_weight2 = document.getElementsByClassName('weight2')[0]

//검사

console.log(userHeight,userWeight,normal_w, result)
console.log(span_height, span_weight,span_normal,span_weight2)

//2.Dom객체 변수 생성하기
span_height.innerHTML = userHeight
span_weight.innerHTML = userWeight
span_normal.innerHTML = normal_w
span_weight2.innerHTML = result


---
