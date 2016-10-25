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
