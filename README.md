# INTERNET
## DESCRIPTION

```mermaid

graph LR;
  LINK -->|One| C1[Laptop]
  LINK -->|Two| C2[iPhone]
  LINK -->|Three| C3[Desktop]
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
  SAN -->|One| SAN1[WWNID1]
  SAN -->|Two| SAN2[WWNID2]
  SAN -->|Three| SAN3[WWNID3]
  
  SAN -->SWITCH1;
  SW1 -->|One| SW1[SW01];
  SW2 -->|Two| SW2[SW02];
  SW3 -->|Three| SW[SW03];
  ```
