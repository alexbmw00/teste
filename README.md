# INTERNET
## DESCRIPTION

```mermaid

graph LR;
  CUSTOMER -->|One| C1[Laptop]
  CUSTOMER -->|Two| C2[iPhone]
  CUSTOMER -->|Three| C3[Desktop]
  C1 -->LB;
  C2 -->LB;
  C3 -->LB;  

  LB-->APP01; 
  LB-->APP02; 
  LB-->APP03; 
  APP01-->DB01;
  APP02-->DB01;
  APP03-->DB01;
  DB01-->STORAGE01;
  
  STORAGE01-->SAN
  SAN -->SWITCH;
    
  SWITCH -->|One| SW1[SW01];
  SWITCH -->|Two| SW2[SW02];
  SWITCH -->|Three| SW3[SW03];
  ```
