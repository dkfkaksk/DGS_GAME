# DGS - DraGon Slayer
- 유니티 버전 - 2022.3.60f (URP)
- 플레이 기기 - PC

## 게임 소개
- 직업을 골라 게임을 시작하고 몬스터를 잡아 성장해 보스 몬스터를 사냥하는 뱀서라이크 장르의 게임
- 게임 장르 - 뱀서라이크
- 게임 모티브 - 롤 집중포화 모드
- 게임 배경 - 월드 오브 워크래프트
- 플레이어 시점 - 쿼터 뷰
### 조작법
- 플레이어 이동 - WASD
- 스킬사용 - E, Q
- 공격 위치 - 마우스 커서
- 공격 방식 전환(자동 - 수동) - **C**(가장 가까운 몬스터의 위치(자동)-마우스 위치(수동))
## :office:개발 인원
**게임공학과**
|2088002 경정찬|2088018 나정원|2288020 윤동욱|
|:--:|:--:|:--:|

 총 3인 진행
## 게임 포스터
![DGS 프로젝트 포스터](https://github.com/user-attachments/assets/9190f517-26cf-4ea8-9a64-02c371a24461)
## :alarm_clock:개발 기간
> 2025.03.06~2025.06.10

## 게임 진행
> - 타이틀 화면
>   ![DGS 타이틀](https://github.com/user-attachments/assets/e8040b0a-5292-4957-b017-9d503169b003)

> - 직업 선택
>   ![직업 선택](https://github.com/user-attachments/assets/fdd5c3c9-0c34-4785-aff2-9e18ce4dd2f7)


> - 게임 시작
>   ![게임시작 시 화면](https://github.com/user-attachments/assets/d34ee5a3-9b28-4cc0-8a26-63c1bee4cc9e)

> - 스폰되는 몬스터 사냥(경험치,골드 획득)
>   ![몬스터 사냥 및 경험치 골드 드랍](https://github.com/user-attachments/assets/451a254c-55c0-4445-95f3-35756c53c703)
<details>
        <summary>:large_blue_diamond:<strong>몬스터 종류 (Monster Types)</strong></summary>
        <ul>
            <li>근접 몬스터
                <ul>
                    <li>일반 근접 몬스터 - 기본적인 근거리 몬스터의 형태로 플레이어에게 닿았을 때 데미지를 줌<br>
                    <img src="https://github.com/user-attachments/assets/d0502ba4-327d-4de4-b279-1debdb8a6a8a" alt=""></li>
                    <li>독 몬스터 - 플레이어에게 닿았을 때 데미지 그리고 몬스터 사망 시 그 자리에 독 장판이 생기며 독 장판에 있는 플레이어에게 데미지를 줌<br>
                    <img src="https://github.com/user-attachments/assets/0da05959-1081-4223-9aff-ca8ee5b78251" alt=""></li>
                    <li>자폭 몬스터 - 해당 몬스터 사망시 주변에 있는 플레이어에게 데미지를 줌<br>
                    <img src="https://github.com/user-attachments/assets/5a43d354-9cf6-49bf-b3ab-aca1c8753228" alt=""></li>
                    <li>분열 몬스터 - 해당 몬스터가 사망 시 작은 몬스터로 분열하게 됨<br>
                    <img src="https://github.com/user-attachments/assets/09eeca35-033c-4757-8b46-8a243d417c4e" alt=""></li><br>
                </ul>
            </li>
            <li>원거리 몬스터
                <ul>
                    <li>기본 투사체 발사하는 몬스터 - 원거리에서 플레이어에게 투사체를 날려 데미지를 줌<br>
                    <img src="https://github.com/user-attachments/assets/1bbf3924-79f5-4f56-9778-445179d3699d" alt=""></li>
                    <li>플레이어의 위치에 독 장판 뿌리는 몬스터 - 원거리에서 플레이어가 있는 지점으로 독 장판을 생성시키며 독 장판에 있는 플레이어에게 데미지를 줌<br>
                    <img src="https://github.com/user-attachments/assets/a02a4144-b8f0-417d-9e2a-1fa44bc164ea" alt=""></li><br>
                </ul>
            </li>
            <li>엘리트 몬스터
                <ul>
                    <li>근거리 엘리트 몬스터
                        <ul>
                            <li>러쉬 몬스터 - 생성 시 속도는 느리지만 점점 빨라지며 플레이어에게 충돌 시 플레이어를 높게 띄우는 에어본을 발생시킴<br>
                            <img src="https://github.com/user-attachments/assets/32322523-dce3-40d2-a135-ae507fbb96a5" alt=""></li>
                            <li>대쉬 몬스터 - 플레이어가 사정거리에 들어오면 잠시 대기 후 플레이어를 향해 빠르게 돌진<br>
                            <img src="https://github.com/user-attachments/assets/024b739a-52cd-40b3-8e8b-058b767b58cd" alt=""></li>
                        </ul>
                    </li>
                    <li>원거리 엘리트 몬스터
                        <ul>
                            <li>3갈래 투사체 발사 몬스터 - 플레이어의 방향을 기준으로 3갈래로 나가는 투사체를 발사 함<br>
                            <img src="https://github.com/user-attachments/assets/98ffcbf4-e45d-47f7-a114-28302431fa39" alt=""></li>
                            <li>슬로우 투사체 발사 몬스터 - 플레이어를 향해 슬로우가 걸리게 하는 wave투사체를 발사 함<br>
                            <img src="https://github.com/user-attachments/assets/b9d429db-35f4-49a9-88ae-8142d8e222a1" alt=""></li><br>
                        </ul>
                    </li>
                    <li>엘리트 몬스터 드랍 아이템 - 자석 아이템, hp회복 아이템
                        <ul>
                            <li>자석 아이템 - <br><img src="https://github.com/user-attachments/assets/8fb863b9-daf5-408c-8144-895d921deb43" alt=""></li><br>
                            <li>HP 아이템 - <br><img src="https://github.com/user-attachments/assets/b1214883-beb9-4074-8deb-766a644c28e0" alt=""></li>
                        </ul>
                    </li>
                </ul>
            </li>
            <li>
                보스 몬스터 - <br>
                <img src="https://github.com/user-attachments/assets/556f1f0a-0f44-4576-91eb-0bba982d507a" alt="">
                <ul>
                    <li>보스 패턴
                        <ul>
                            <li>1. 브레스 - 보스 방에 들어갈 시 가장 먼저 나오는 패턴으로 브레스의 범위에 있는 플레이어는 지속적으로 데미지를 받음 <br>
                            <img src="https://github.com/user-attachments/assets/35b8e5c5-5031-462e-a29e-fe53f7fab8be" alt=""></li>
                            <li>2. 토네이도 - 어느정도의 시전 시간이 지나면 플레이어를 향해 이동하며 지속적으로 데미지를 주는 토네이도 오브젝트를 생성<br>
                            <img src="https://github.com/user-attachments/assets/cc77abb3-39ca-42c2-b48c-d43011f9541c" alt=""></li>
                            <li>3. 돌진 및 브레스 - 하늘로 날아오르는 애니메이션 이후 보스방의 대각선의 범위를 빠르게 이동하며 대미지를 줌 <br>
                            <img src="https://github.com/user-attachments/assets/c3e00bca-36df-4234-b5bd-1d71efed5db8" alt=""></li>
                            <li>4. 운석 - 보스방에 들어가고 패턴이 시작되면 지속적으로 정해놓은 시간마다 운석이 떨어지며 운석에 맞으면 데미지를 줌 <br>
                            <img src="https://github.com/user-attachments/assets/d4e8fdbd-a481-4eb9-976e-6ecffabf62de" alt=""></li>
                        </ul>
                    </li>
                </ul>
            </li>
        </ul>
    </details>

> - 레벨업 시 증강 선택으로 성장
<details>
        <summary>:large_blue_diamond:<strong>증강 종류 (Monster Types)</strong></summary>
        <ul>
            <li>스톰 - <br>
                <img src="https://github.com/user-attachments/assets/22be9130-59d0-41eb-ab74-5331b2940d3e" alt="">
            </li>
            <li>낙뢰 - <br>
                <img src="https://github.com/user-attachments/assets/40e08e46-6fe7-467c-8e79-97f255bc5a40" alt="">
            </li>
            <li>매직 미사일 - <br>
                <img src="https://github.com/user-attachments/assets/9cab85fd-50ac-4409-a590-e23dd03abc11" alt="">
            </li>
            <li>부메랑 - <br>
                <img src="https://github.com/user-attachments/assets/c3d6260c-1fd7-462b-92f7-53a14423e81a" alt="">
            </li>
            <li>빛의 화살 - <br>
                <img src="https://github.com/user-attachments/assets/a748b6af-b88d-4b1c-ae72-6cf1cd18d809" alt="">
            </li><br>
            <li>수호검 - <br>
                <img src="https://github.com/user-attachments/assets/517be042-95a2-4a00-a0b5-87c01a2a3819" alt="">
            <li>암흑 구체 - <br>
                <img src="https://github.com/user-attachments/assets/f26c860b-3508-4375-afb5-3e7cc59652e5" alt="">
            </li>
            <li>얼음 미사일 - <br>
                <img src="https://github.com/user-attachments/assets/cfabf23c-4491-4138-ba40-4c2a330c6fc4" alt="">
            </li><br>
            <li>얼음 방패 - <br>
                <img src="https://github.com/user-attachments/assets/788c53be-01ad-44b6-96a5-99d79de7ef59" alt="">
            </li>
            <li>얼음 역장 - <br>
                <img src="https://github.com/user-attachments/assets/005ce0c6-5cef-4a68-8ef8-b8e5a14a748c" alt="">
            </li>
            <li>절멸자 - <br>
                <img src="https://github.com/user-attachments/assets/132356a4-62d6-4330-97cc-b421db30fdcf" alt="">
            </li>
            <li>튕기는 수리검 - <br>
                <img src="https://github.com/user-attachments/assets/e1c8e305-751b-4ed9-8dde-816f635e5c14" alt="">
            </li>
            <li>화염 정령 - <br>
                <img src="https://github.com/user-attachments/assets/c59e4046-fa53-43bb-a771-c3a9b041f009" alt="">
            </li>
            <li>영혼 연결 - <br>
                <img src="https://github.com/user-attachments/assets/64e94bc8-ebd5-4893-9c89-c498e689e51d" alt="">
            </li>
            <li>전사 기본 무기 - <br>
                <img src="https://github.com/user-attachments/assets/4417734d-19e3-42a4-8f88-c24a1a1b0f0a" alt="">
            </li>
            <li>마법사 기본 무기 - <br>
                <img src="https://github.com/user-attachments/assets/4aaa2eb1-7e01-44f9-9636-dcc9fcea6fdc" alt="">
            </li><br>
            <li>
                각종 스텟들 - <br>
                <img src="https://github.com/user-attachments/assets/556f1f0a-0f44-4576-91eb-0bba982d507a" alt="">
            </li>
            <li>
                <table>
                 <thead>
                   <tr>
                     <th>스텟 이름</th>
                     <th>이미지</th>
                   </tr>
                 </thead>
                 <tbody>
                   <tr>
                     <td>체력 증가</td>
                     <td><img src="https://github.com/user-attachments/assets/72eafcf0-8a97-43ce-aa9e-d928351dbaad" width="64"/></td>
                   </tr>
                   <tr>
                     <td>공격력 증가</td>
                     <td><img src="https://github.com/user-attachments/assets/01b7c658-8866-4bc2-a2be-e22526066ce4" width="64"/></td>
                   </tr>
                </tbody>
              </table>
            </li>
        </ul>
    </details>



> - 보스 사냥
>   ![보스사냥](https://github.com/user-attachments/assets/aa55722b-061e-46e1-9cbf-2729dbafd17a)
> - 보스 클리어 시 게임 종료<br>
>   ![클리어 화면](https://github.com/user-attachments/assets/96b6174c-f0c0-4c02-a7b9-83ea7e972a79)

> - 플레이 후 모인 골드로 능력치 업그레이드(체력 5회 업그레이드로 체력이 1.5배로 늘어남)
>   ![능력치 업그레이드(체력)](https://github.com/user-attachments/assets/72eafcf0-8a97-43ce-aa9e-d928351dbaad)
>   ![체력 업그레이드 5회](https://github.com/user-attachments/assets/01b7c658-8866-4bc2-a2be-e22526066ce4)

