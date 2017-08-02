# Accounting_Mng
<h1>회계관리프로그램 (Java실습 최종작품)</h1>

<h2>*각 폴더 및 클래스</h2>

<pre>
biz : 회계프로그램을 실행하고 데이터를 처리하는데 필요한 각종 클래스들입니다.

excel : 지정된 엑셀파일과 연동하여 데이터를 읽어오고 저장하는 기능을 하는 클래스들입니다.

menu : 프로그램을 실행시킨 후 나타나는 메뉴와 서브메뉴에 대한 클래스들입니다.

util : 데이터를 처리하는 중 이용되는 유틸성 클래스들입니다.

vo : 엑셀파일에서 읽어온 데이터를 저장하고 데이터를 처리하는데 이용되는 vo클래스들입니다.

test.img : README.md에 사용되어 프로그램을 설명하기 위한 이미지파일들입니다.

test.xlsx : 프로그램의 작동을 test하기위해 임의로 지정한 데이터가 저장될 엑셀파일입니다.
</pre>
<br>



<h2>*프로그램 구성 및 작동</h2>

<h3>01.경로와 엑셀파일명, 각 시트명 입력</h3>
<img src="test.img/01.경로와 엑셀파일명, 각 시트명 입력.jpg"><br>
<pre>
 fileName : 데이터를 저장할 엑셀파일의 경로와 엑셀파일명.xlsx 입력
 sheet00 : 자산항목이 저장될 시트명을 지정 (지정한 시트명에 해당하는 시트가 없을 경우 자동 생성)
 sheet01 : 부채항목이 저장될 시트명을 지정 (지정한 시트명에 해당하는 시트가 없을 경우 자동 생성)
 sheet02 : 자본항목이 저장될 시트명을 지정 (지정한 시트명에 해당하는 시트가 없을 경우 자동 생성)
 sheet03 : 자산,부채,자본 항목이 모두 저장될 시트명을 지정 (지정한 시트명에 해당하는 시트가 없을 경우 자동 생성)

 해당하는 엑셀파일에 앞서 기록된 회계데이터가 존재할 경우 프로그램 내에서 vo파일로 변환 되어 사용됨
</pre>


<h3>02.입력하기(발생한 회계사건 데이터)</h3>
<img src="test.img/02.입력하기(발생한 회계사건 데이터).jpg"><br>
<pre>
회계사건 발생 시, 메인 메뉴의 1번 항목의 회계처리 입력을 선택
서브 메뉴에서 발생한 사건이 해당하는 항목을 선택
발생한 회계사건의 내용을 날짜/분류/계정명/금액(+,-)로 입력
</pre>


<h3>03.복식부기(회계원칙에 따라 프로그램에서 강제)</h3>
<img src="test.img/03.복식부기(회계원칙에 따라 프로그램에서 강제).jpg"><br>
<pre>
복식부기 회계원칙에 따라서
프로그램에서 자동으로 회계사건을 한번 더 입력할 것을 강제
</pre>


<h3>04.필요한 추가 데이터입력</h3>
<img src="test.img/04.필요한 추가 데이터입력.jpg"><br>
<pre>
테스트를 위해 임의로 부채항목과 자본항목을 추가로 입력 (복식부기 포함)
</pre>


<h3>05.목록별출력의 자산출력</h3>
<img src="test.img/05.목록별출력의 자산출력.jpg"><br>
<pre>
항목별로 입력된 회계 장부를 확인하고 싶을 때 
메인 메뉴의 2번 목록별 출력을 선택

목록별 출력의 서브메뉴에서 자산항목 출력을 선택한 모습
</pre>


<h3>06.목록별출력의 부채출력</h3>
<img src="test.img/06.목록별출력의 부채출력.jpg"><br>
<pre>
목록별 출력의 서브메뉴에서 부채항목 출력을 선택한 모습
</pre>


<h3>07.목록별출력의 자본출력</h3>
<img src="test.img/07.목록별출력의 자본출력.jpg"><br>
<pre>
목록별 출력의 서브메뉴에서 자본항목 출력을 선택한 모습
</pre>


<h3>08.목록별출력의 전부출력</h3>
<img src="test.img/08.목록별출력의 전부출력.jpg"><br>
<pre>
목록별 출력의 서브메뉴에서 모든항목 출력을 선택한 모습
</pre>


<h3>09.기간별출력의 특정날짜출력</h3>
<img src="test.img/09.기간별출력의 특정날짜출력.jpg"><br>
<pre>
날짜별로 입력된 회계 장부를 확인하고 싶을 때 
메인 메뉴의 3번 기간별 출력을 선택

기간별 출력의 서브메뉴에서 특정날짜 출력을 선택한 뒤
확인하고자 하는 날짜를 입력한 모습
</pre>


<h3>10.기간별출력의 7일간출력(2017-06-27기준)</h3>
<img src="test.img/10.기간별출력의 7일간출력(2017-06-27기준).jpg"><br>
<pre>
기간별 출력의 서브메뉴에서 지난 7일 출력을 선택한 모습
(해당 이미지를 촬영한 2017-06-27 기준으로 7일간의 내역이 나타남)
</pre>


<h3>11.기간별출력의 30일간출력(2017-06-27기준)</h3>
<img src="test.img/11.기간별출력의 30일간출력(2017-06-27기준).jpg"><br>
<pre>
기간별 출력의 서브메뉴에서 지난 30일 출력을 선택한 모습
(해당 이미지를 촬영한 2017-06-27 기준으로 30일간의 내역이 나타남)
</pre>


<h3>12.기간별출력의 전부출력</h3>
<img src="test.img/12.기간별출력의 전부출력.jpg"><br>
<pre>
기간별 출력의 서브메뉴에서 모든 기간을 선택한 모습
</pre>


<h3>13.대차대조 확인의 자산합계확인</h3>
<img src="test.img/13.대차대조 확인의 자산합계확인.jpg"><br>
<pre>
각 항목의 합계 또는 대차대조의 참/거짓을 확인하기 싶을 때
메인 메뉴의 4번 회계처리 확인을 선택

회계처리 확인의 서브메뉴에서 자산합계 확인을 선택한 모습
</pre>


<h3>14.대차대조 확인의 부채합계확인</h3>
<img src="test.img/14.대차대조 확인의 부채합계확인.jpg"><br>
<pre>
회계처리 확인의 서브메뉴에서 부채합계 확인을 선택한 모습
</pre>


<h3>15.대차대조 확인의 자본합계확인</h3>
<img src="test.img/15.대차대조 확인의 자본합계확인.jpg"><br>
<pre>
회계처리 확인의 서브메뉴에서 자본합계 확인을 선택한 모습
</pre>


<h3>16.대차대조 확인의 대차대조확인</h3>
<img src="test.img/16.대차대조 확인의 대차대조확인.jpg"><br>
<pre>
회계처리 확인의 서브메뉴에서 대차대조 확인을 선택한 모습
</pre>


<h3>17.저장 및 종료</h3>
<img src="test.img/17.저장 및 종료.jpg"><br>
<pre>
모든 입력과 출력 등의 작업이 끝난 후에는
메인메뉴 5번 저장 및 종료를 입력

입력된 데이터는 앞서 지정한 엑셀파일에 기록됨
</pre>


<h3>18.지정한 시트명의 시트생성확인</h3>
<img src="test.img/18.지정한 시트명의 시트생성확인.jpg"><br>
<pre>
01에서 지정한 것과 같은 시트명이 각각 자동으로 생성된 것을 확인
</pre>


<h3>19.자산 시트에 데이터 입력 확인</h3>
<img src="test.img/19.자산 시트에 데이터 입력 확인.jpg"><br>
<pre>
자산항목 입력으로 입력된 데이터가 지정한 자산 시트에 기록된 모습 (날짜순)
</pre>


<h3>20.부채 시트에 데이터 입력 확인</h3>
<img src="test.img/20.부채 시트에 데이터 입력 확인.jpg"><br>
<pre>
부채항목 입력으로 입력된 데이터가 지정한 부채 시트에 기록된 모습 (날짜순)
</pre>


<h3>21.자본 시트에 데이터 입력 확인</h3>
<img src="test.img/21.자본 시트에 데이터 입력 확인.jpg"><br>
<pre>
자본항목 입력으로 입력된 데이터가 지정한 자본 시트에 기록된 모습 (날짜순)
</pre>


<h3>22.통합 시트에 데이터 입력 확인</h3>
<img src="test.img/22.통합 시트에 데이터 입력 확인.jpg"><br>
<pre>
입력된 모든 데이터가 지정한 통합 시트에 전부 기록된 모습 (날짜순)
</pre>
















