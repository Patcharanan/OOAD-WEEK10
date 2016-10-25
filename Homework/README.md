# Sequance Diagram

*  รูปที่ 1 Application Line FirtsTime
```
@startuml

title "Login Line on PC FirstTime"

User-> Application : Enter Username / Password
Application ->System :Check Username - Password
System -> System : Check the accuracy 
System -[#0000FF]-> Application : invalid
Application -[#0000FF]-> User : <font color=red><b>Warning Please Try Again
System -[#0000FF]-> Application :<font color=blue><b> Valid
Application -> User : Send 4-Digit Security Code 
User -> Application : Enter Srcurity Code
Application -> System : Check 
System -> System : Check the accuracy
System -[#0000FF]-> Application :<font color=blue><b> Valid
Application -[#0000FF]-> User : <font color=blue><b> Login Success

@enduml
```

[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/hP8nJyCm48Lt_ufJcICOcAeIjGfawX0f1GR4u3f7Ui8vL_O5b7-FGo6DKg4or9lbp--zUxfb4EsbRQnIGc8HPcjN4yEQ6C4n51dav8DigC6PKey1VPB2Qh-tPBHG9ERmm88U-YVM3S8r53g4J-ShDUQIjEo2O0FpR8Vc_SWdH_w7Y0w_B1nWsI5eOrglJGS3zd9r4q-Ulvv48lxGbYO1ndZl7hd5csC1uwppTnwhTB5DdxLduXeAYpeWR7m7greJdtSTYsrjYxqQF9tc6DnBv0fkatkgIU8bZaVIGUOgXE-cuO-gIpz2fzgJvlxNwUM6ErFoyFMmPcLh38QWr39M4RVm2m00)

*  รูปที่ 2 โอนเงินผ่านตู้ ATM
```
@startuml

title "Transfer Monet at ATM"

User-> ATMmachine : Insert Card
ATMmachine -> KeyPad : Press Password
KeyPad -[#0000FF]-> ATMmachine : <font color=blue> [Valid] Access to Menu
ATMmachine -> Sceen : Open Menu
User -> Sceen : Select Menu "Transfer"
User -> KeyPad : Press Account Number - Amount Money
Sceen -[#0000FF]-> User : Show Account Name & Amount Money & Fee
User -> Sceen : Check the accuracy
User -> KeyPad : Press Enter
Sceen -[#0000FF]-> User :<font color=blue> Transfer Complete

@enduml
```
[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/TL7BQiD03BplLmWNUWlqNDeGOse8nQqXQIyX1sMjODDzX5qjmNzVsIrvE6GlYpIZqKXQHCR0oHgbk6D3aAq3khYd09Ltn80C-RhAbFgA56Rp8R2esyuHFCFIIPAXmD2e2q1exzJNs0Yb3XGZr1ZZqGlhFp_RF3p9AyljLF9bxns3ziQ7rvr9D8VDDvgksKAkzI357YfoQT9lfOcSb7yUv1lnmUybiY93caViF6HseaqCIpEVnCX7ihk10BaTus4flVhJl1fYr94khJ-UYz4IF5wLIbWItPWhMj8_m2q1Qfq2wlwUiJV75EuRk5tVwPw5jmT3J4ejo3Loyby0)


* รูปที่ 3 โอนเงินผ่านมือถือ
```
@startuml

title "Transfer Monet With Mobile"

User-> Mobile : Open Application
User -> MobileBanking : Enter User / Password
MobileBanking -> MobileBanking : Check the accuracy
MobileBanking -[#0000FF]-> Mobile : invalid
Mobile -[#0000FF]-> User : <font color=red><b>Warning Please Try Again
MobileBanking -[#0000FF]-> Mobile :<font color=blue><b> Valid
User -> MobileBanking : Access To Application
User -> MobileBanking : Check Balance
MobileBanking -[#0000FF]-> Mobile : Show Balance
User -> MobileBanking : Enter Account Number & Amount Money
MobileBanking -> MobileBanking : Check Account Name 
MobileBanking -[#0000FF]-> Mobile : Show Account Name & Money & Fee
User -> Mobile : Press OK 
MobileBanking -[#0000FF]-> User : <font color=red> Message "Success"

@enduml
```
[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/ZLF1JW8n4BttAoQOuCdecI1X8N8n20ae1-DXjZkm3TtffkrA-7kxHJU0GBQNTjBtNb_UJ8VEe_LLeONmock2pj8YkpLPc1ec3olbyt1CbQQE4E-ExCFWjuOUp4fYICfIAubU6Ou0Q10ZvAtYJG2-i0yNyVOHvkZSpjXCdA8kqCOvoItud02bh2pA_Jddy-ufhCdawzYMuc_Kwa__51GzzA2_Dkn16ctiiwLiq4y7AxHSQyureIDOsZqa6rJSvibZkLHNLEl1HpHnBP94Id8EbgPLW8SaHgYH9RKAOP6RNKEutPTWnLJ1_rjLfA7iGbB4kXw1VTikDI9O4BHtU4Bh7fuC-uJEJGV2tDQ9pLvlobzfC4m35pTXmXTLJBuZXiHP77rnlv0K9lc2ph_6GlD1ngOeDNdw0G00)

* รูปที่ 4 ซื้อสินค้าออนไลน์
```
@startuml

title "Online Shopping"

User-> Web : Open 
User -> WebShopping : Enter Site
User -> WebShopping : Enter Username - Password
WebShopping -> Database : Check Data
Database-[#0000FF]-> WebShopping :<font color=red> [Invalid] Please TryAgain
Database-[#0000FF]-> WebShopping :<font color=blue> [Valid] Show Profile
User -> WebShopping : Select Product
User -> WebShopping : Add to Cart
WebShopping -> Database : Check Product 
User -> WebShopping : Confirm & Transfer Money
WebShopping -[#0000FF]-> User : Delivery

@enduml
```

[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/bP9DQyCm38Rl_XMYW-qKsBbifILTOOVHGFPnA3quiTAQENAmrPRy-odfEhgFRCp7LuzUyKgUHjQ1TxLJYYqxXD6Id2M4VEkRnj9cfDHJn91Cu0KB6CEoGO9UWgDs0gLsHonoRXb_1ReQwHeXWKp7UF31g7DEskQQTQ4ZIa-wnVAr5zH9JLONr_8MY_NN2JUL9uRIEnzk0ve9hEvfhvqrQyWSTeQFePrjjAL_cXLkX-BsVFGIvW1Py9LrGr5pT5Xo1vbToGFGp1XW3wcSuCyDl3iDxJxrLDbGmwKar1GhOHuyOVlPzpnhxpE6EJgxnz2gAPBfFuAwoakKA_z0Vr_9nxJKrur3nZS0)


* รูปที่ 5 ตู้เติมเงินมือถือ
```
@startuml

title "Top up Mobile"

User -> TopUpMachine : Touch Sceen 
User -> TopUpMachine : Select Mobile Network
User -> TopUpMachine : Press Mobile Number
TopUpMachine -> System : Check Mobile Network/Number
System -[#0000FF]-> TopUpMachine :<font color=red> [Warning] Not Match
System -[#0000FF]-> TopUpMachine :<font color=blue> [Access grant] Match
User -> TopUpMachine : Insert Money
TopUpMachine -> System : Check the accuracy 
System -[#0000FF]-> TopUpMachine : <font color=red>[Denied] Refund 
System -[#0000FF]-> TopUpMachine : <font color=blue>[Success] Complete
TopUpMachine -> User : Top up Complete

@enduml
```
[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/bP8nQyCm48Lt_OeZ7Jg5TYvjI4a9T4WeTK87uq4-dsCHMJBIYU9_Nzbn0uanRRH9-kxTlUCjFKl7eTP2i69DCDlP1a836vihJJCXzfuSp1SGt_VDHcAb3C5Jl0Qi844Y0rDCGfgG1odO4dzRTvo2FnnvVsP3dPCJ5qWiILhFL4TuLH4UhuGVXg81cgTtZ_6irzcertDf3GDQRTsBes81wPTqHfb31biRvvMCrOqokGuKTLuHEnS79mrdWz24ttSJtxlb66h_CieLWKGCJc8B_vWChXscRsGK5HbyKXbCSRD6RozDGcylWvMj6qrCexbxhrqu-WoTiIMPei-Ok3ybvgBlgMYypLtSeY_Ztw_E3m00)
