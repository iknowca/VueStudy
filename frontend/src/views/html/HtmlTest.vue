<template>
    <div class="about">
        <h1>실제 코드 형태로 입력해 보기</h1>
        <h6>원래는 코드 형태가 아닌 실제 코드가 동작해야 합니다.</h6>
        <h4>chatgpt같은 것을 만든다면 필요할 지도 모르겠네요</h4>
        <!--
        강제 스타일 먹이기는 아래와 같이 style="css속성"
        여기서 css속성은 text-align으로
        글자를 정렬할 때 사용하며 디폴트로 center 정렬이었으나
        아래 function saveLocal 에 대해서는 left정렬을 적용하는 작업입니다.
        -->

        <pre style="text-align: left;">
            function saveLocalData () {
                let second = document.getElementById("second")
                let value = second.value
                localStorage.setItem(1, value)
                getLocalData()
            }
        </pre>
        <p><strong>TypeScript</strong>, <b>Javascript</b>, Python</p>
        <p><em>Rust</em>, <i>C</i>, Verilog</p>
        <h2>Python
            <mark>TensorFlow</mark>
        </h2>
        <p>Deep Learning <span style="color: green">Keras</span></p>
        <!-- ul은 Unorderd List 순서가 필요하지 않은 경우-->
        <ul style="text-align: left">
            <li>EDDI</li>
            <li>Electric Car</li>
            <li>MSA</li>
            <li>Deep Learning</li>
            <li>Distribution Server</li>
        </ul>

        <ul style="text-align: left;">
            <li>Vue
                <ol type="a" start="3">
                    <li>Vue Init</li>
                    <li>Vue Router</li>
                    <li>Vue Template</li>
                    <li>Vue Script</li>
                    <li>Vue props</li>
                    <li>Vue v-model</li>
                    <li>Vue axios</li>
                    <li>Vue Local Component</li>
                    <li>Vue Global Component</li>
                    <li>Vuetify</li>
                    <li>Image Gallery</li>
                    <li>File Upload</li>
                    <li>Login/Logout</li>
                    <li>V-Dialog</li>
                    <li>Carousel</li>
                    <li>Card</li>
                    <li>Grid</li>
                </ol>
            </li>
            <li>DDD
                <ol type="a">
                    <li>Domain Driven Development</li>
                    <li>How to write Backlog</li>
                    <li>Behavioral Domain</li>
                    <li>Value Object</li>
                    <li>Domain Service</li>
                    <li>Repository</li>
                </ol>
            </li>
            <li>Hexagonal Architecture
                <ol>
                    <li>Hexagonal Architecture</li>
                    <li>Domain Hexagon</li>
                </ol>
            </li>
        </ul>
        <table>
            <tr>
                <th>1 row 1 column</th>
                <th>1 row 2 column</th>
                <th>1 row 3 column</th>
            </tr>
            <tr>
                <td>내용이</td>
                <td>없어서</td>
                <td>안만들었니 ?</td>
            </tr>
        </table><br>
        <table style="width: 600px">
            <!-- caption을 통해서 table(표)에 제목 비스무리한 느낌을 줄 수 있음 -->
            <caption>
                <strong>Junior who pursue modern development with agile process</strong>
            </caption>
            <tr>
                <th>Name</th>
                <td>이름</td>
                <th>Contact</th>
                <td>010-1111-2222</td>
            </tr>
            <tr>
                <th>Address</th>
                <td colspan="3">주소</td>
            </tr>
        </table>

        <h2>Image</h2>
        <img src="@/assets/logo.png"><br>
        <fiure>
            <img src="@/assets/logo.png">
            <figcaption style="font-size: 32px;">Vue.Js</figcaption>
        </fiure>

        <h1>text link 생성</h1>
        <a href="https://golang.org">Golang Homepage</a>
        <h1>이미지 링크 생성</h1>
        <a href="https://google.com/">
            <img src="@/assets/logo.png">
        </a>

        <!-- form 태그는 말 그대로 format 을 지정해서 데이터를 전송합니다.
        method에 post 를 지정할 수 있고 default값은 get입니다.
        input타입에는 text, number, submit등등이 올 수 있습니다.
        text는 말 그대로 문자열 넘버는 숫자 서브밋은 등록 개념이라 보면 됩니다.
        속성값 밸류를 통해 표기되는 형태를 지정할 수 잇습니다.
        추후 이 부분의 submit을 prevent하여 vue가 axios하도록 구성하게 됩니다.
        -->
        <form action="/">
            <input type="text" value = "찾을 값">
            <input type="submit" valu="찾기">
        </form>

        <!--
        다중선택
        인풋 타입으로 체크박스를 사용하여 밸류값에 선택한 값을 볼 수 있습니다.
        자바스크립트에서 어떤 값을 선택했는지 처리할 수 있고
        이를 토대로 뷰 쪽에 맥시오스 하는 데이터를 처리할 수 있습니다.
        -->
        <h3>
            <form action="/" style="text-align: left">
                <li><input type="checkbox" value="grammar">grammar</li>
                <li><input type="checkbox" value="writing">writing</li>
                <li><input type="checkbox" value="reading">reading</li>
            </form>
        </h3>
        <!--email 및 패스워드입력이 필요한 상확 -->
        <form style="text-align: center;">
            <fieldset>
                <legend>login</legend>
                <ul>
                    <li>
                        <label for="email">email</label>
                        <input type="text" id="email">
                    </li>
                    <li>
                        <label for="pwd">password</label>
                        <input type="password" id="pwd">
                    </li>
                </ul>
            </fieldset>
        </form>

        <form style="text-align: left;">
            <fieldset>
                <legend>회원 가입</legend>
                <ul>
                    <li>
                        <label for="email">이메일: </label>
                        <input type="text" id="email">
                    </li>
                    <li>
                        <label for="pwd">비밀번호: </label>
                        <input type="password" id="pwd">
                    </li>
                </ul>
            </fieldset>

            <input type="submit" value="회원 가입">
            <!-- 입력을 잘못 했을 경우 정보를 초기화 합니다 -->
            <input type="reset" value="초기화">
        </form>
        <form action="/examples/media/action_target.php" method="get">
            여러분의 나이대를 골라보세요.<br>
            <input type="radio" name="ages" id="teen" value="teenage">
            <label for="teen">10대</label><br>
            <input type="radio" name="ages" id="twenty" value="twenties">
            <label for="twenty">20대</label><br>
            <input type="radio" name="ages" id="thirty" value="thirties">
            <label for="thirty">30대</label><br>
            <input type="radio" name="ages" id="forty" value="forties">
            <label for="forty">40대 이상</label><br>
            <input type="submit">
        </form>
        <form style="text-align: left;">
            <fieldset>
                <legend>과목 선택</legend>
                <ul>
                    <li>
                        <label for="subject">과목: </label>
                        <!--
                            select의 경우엔 드롭 다운 형태의 목록을 만들 수 있습니다.
                            multiple을 선택하여 여러 옵션들을 복수 선택 할 수 있습니다.
                            size는 눈에 보이는 리스트의 개수입니다.
                        -->
                        <select size="5" id="subject" multiple>
                            <!-- option에는 실제 배치하고 싶은 옵션 리스트를 작성합니다. -->
                            <option value="architecture">소프트웨어 아키텍처</option>
                            <option value="ddd">DDD 설계</option>
                            <option value="clean">Clean 아키텍처</option>
                            <option value="hexagonal">Hexagonal 아키텍처</option>
                            <option value="msa">MSA 설계</option>
                            <option value="rxjava">Reactive Java Programming</option>
                            <option value="r2dbc">R2DBC Reactive DB System</option>
                            <option value="jpa">Reactive에서는 사용할 수 없는 JPA</option>
                            <option value="mfe">Micro Frontend Service</option>
                            <option value="edm">Event Driven MSA</option>
                            <option value="kafka">Kafka 기반 메시지 브로커 시스템</option>
                        </select>
                    </li>
                </ul>
            </fieldset>
        </form>
        <!-- progress bar 만들기 -->
        <ul>
            <li>
                <label>10초 남았음</label>
                <progress value="50" max="60"></progress>
            </li>
            <li>
                <label>30% 채웠음</label>
                <progress value="30" max="100"></progress>
            </li>
        </ul>
        <!-- meter 만들기: 값의 크기를 표시 -->
        <ul>
            <li>
                <label>투명도 0.8</label>
                <meter value="0.8"></meter>
            </li>
            <li>
                <label>사용률 64%</label>
                <meter min="0" max="100" value="64"></meter>
            </li>
            <li>
                <label>트래픽 초과까지</label>
                <meter min="1024" max="16384" value="9277"></meter>
            </li>
        </ul>
    </div>
</template>

<style scoped>
table, th, td {
    border: 1px solid #ccc;
}
th {
    padding: 15px; /* 셀 테두리와 내용 사이의 간격(패딩) */
}
td {
    padding: 7px;
}
input {
    border: 1px solid black
}
ul li {
    list-style: none;
    margin: 15px 0;
    font-size: 16px;
}

</style>
<script setup>
</script>