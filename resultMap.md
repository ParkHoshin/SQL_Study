```
resultMap
<resultMap> 태그를 사용 할 때 지정하는 속성 값 이다.

resultMap 사용방법
속성 = "아이디 명" / resultMap="user"

<resultMap> 사용방법
<resultMap id="태그를 구분 할 이름" class="객체 파일에 위치">
  <result property="객체 변수 명 지정" colum="변수에 값을 저장 할 컬럼 명"/>
</resultMap>

정보
데이터베이스 조회 값이 resultMap에 지정된 변수에 빠짐없이 저장 되도록 결과 값을 뽑아야 된다.
쉽게 이야기해서 데이터베이스 결과 값으로 컬럼 2개에 대한 결과 값이 나왔을 경우 resultMap 변수의 개수가 3개면 resultMap 변수 하나에는 값이 들어가지를
않아서 오류가 발생 합니다.
*데이터베이스 결과 값의 컬럼 개수 == resultMap 변수 개수 조건을 항상 유지해야한다.* 
*데이터베이스 결과 값의 컬럼 이름과 resultMap 에 지정된 컬럼의 이름이 같아야 됩니다.*(데이터베이스를 조회해서 나온 결과값의 컬럼 명칭과 비교하기 떄문)
```
